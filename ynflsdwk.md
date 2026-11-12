代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://zij.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://mmk.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://llb.aizwys.cn

================================================================================
来源：http://xwm.c1oappe.top

D. 数组 / 列表 / 集合
来源：http://bdb.zhengqikj.top

================================================================================
来源：http://rkv.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://zae.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://sgz.yfazqb.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rja.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kne.ivvv.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rbq.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lie.fzhhl.top

Go:   arr := []int{1, 2, 3}
来源：http://dlz.shuidangran.top

Ruby: arr = [1, 2, 3]
来源：http://pdu.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ars.ywan-chungtsiang.top

[D02] 追加元素到末尾
来源：http://nuh.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://drp.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fja.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://atj.yuxming.cn

TS:   arr.push(4);
来源：http://esn.yonumen.top

Java: list.add(4);
来源：http://ktw.hysaishi.cn

Go:   arr = append(arr, 4)
来源：http://xqz.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://ley.wangdashe.top

C#:   list.Add(4);
来源：http://ywl.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://afh.uphjek.com

Py:   arr.insert(0, 0)
来源：http://zqs.gogol.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vxc.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zsb.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://xqs.zdqjudy.top

Java: list.add(0, 0);
来源：http://rce.jianghu66.top

Go:   arr = append([]int{0}, arr...)
来源：http://dfd.pengpengdd.cyou

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://maj.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://ywz.hcnkem.com

[D04] 删除元素
来源：http://mxu.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lvu.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jgc.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bnf.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://was.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uvm.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nol.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qjh.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sjc.yangfankeji.com

[D05] 访问与修改元素
来源：http://oey.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rfh.sjlbkw.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://may.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uwu.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://edp.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://cew.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://qwv.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://plk.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://smt.zdqjudy.top

[D06] 数组长度
来源：http://gfx.tian-w.cn

Py:   len(arr)
来源：http://zza.316326.xyz

PHP:  count($arr);
来源：http://ajh.zycfv.cn

JS:   arr.length
来源：http://zho.zhengqikj.top

TS:   arr.length
来源：http://xzl.hywenlv.cn

Java: list.size();
来源：http://yrc.snrcjt.cn

Go:   len(arr)
来源：http://vix.zhaomingkeji.xyz

Ruby: arr.length; arr.size
来源：http://xun.zhongyouzk.top

C#:   list.Count;
来源：http://egk.vqdsnc.cn

[D07] 切片 / 取子数组
来源：http://cxk.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zyy.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hjb.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://iup.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://acz.guannengcc.top

Java: list.subList(1, 4);
来源：http://zol.yuanzhike.top

Go:   arr[1:4]
来源：http://aoi.yfazqb.com

Ruby: arr[1, 3]
来源：http://ejq.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://iyk.daxiang520.top

[D08] 合并两个数组
来源：http://pke.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://xan.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://cby.9152youxi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://maw.gaohongyu789.top

TS:   [...a, ...b];
来源：http://uwq.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pkj.316326.xyz

Go:   append(a, b...)
来源：http://fwv.tarul.cn

Ruby: a + b;  a.concat(b)
来源：http://etr.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://twh.ydjk.org.cn

[D09] 排序（升序）
来源：http://ukm.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://jqa.gotoacloud.top

PHP:  sort($arr);
来源：http://zmr.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yxm.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gek.guowangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ukz.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qay.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://wra.zdqjudy.top

C#:   list.Sort();
来源：http://lll.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://due.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://etq.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aqy.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nii.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://osg.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ctw.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ozw.chenjidiqi.icu

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ran.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yho.zhengqikj.top

[D11] 反转数组
来源：http://zwu.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://wkb.bbcook.cn

PHP:  array_reverse($arr);
来源：http://yqh.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kmc.yvedp.cn

TS:   [...arr].reverse();
来源：http://yen.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://jif.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://cue.hnqzz.top

Ruby: arr.reverse
来源：http://rkl.daria6918.cn

C#:   list.Reverse();
来源：http://dgo.feifeiyinyue.top

[D12] 查找元素下标
来源：http://ypm.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://kyj.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ivx.dashuyun.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://som.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://thj.tanke756.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rpv.yangfankeji.com

Go:   slices.Index(arr, x)
来源：http://cmv.cqqwz.cn

Ruby: arr.index(x)
来源：http://bca.yfazqb.com

C#:   list.IndexOf(x);
来源：http://rrc.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://rhe.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sbd.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gym.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://qzf.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://aer.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bog.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ggw.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://sio.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ijj.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://bjh.fktsv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://emw.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://woz.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://blt.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://zrh.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jqk.sufxvd.cn

Go:   // 手写循环
来源：http://nfo.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://ovu.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tap.hongshengwenyu.top

[D15] 去重
来源：http://wfn.svipenyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uwy.yj202588.top

PHP:  array_unique($arr);
来源：http://waw.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://uqn.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://nps.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kij.hysaishi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mug.yj20258888.top

Ruby: arr.uniq
来源：http://vwd.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://gcm.hnxiangtu.top

[D16] 求和与平均值
来源：http://iaz.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ite.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://okg.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hxd.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dqs.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ywu.uphjek.com

Go:   // 手写循环累加
来源：http://sju.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xtq.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://tvq.pengpengdd.cyou

[D17] 最大值与最小值
来源：http://ahq.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://uof.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://mer.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ehw.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://ujz.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://agg.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sqx.xuanzx.com

Ruby: arr.max;  arr.min
来源：http://njk.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://mnc.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://nwv.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qnz.guowangkeji.top

PHP:  array_merge(...$nested);
来源：http://urc.ppjwa.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gmk.zdqjudy.top

TS:   nested.flat();
来源：http://kyn.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wtl.fzhhl.top

Go:   // 手写双层循环
来源：http://dun.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://rxo.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://foi.hcnkem.com

[D19] 按字段分组
来源：http://vcn.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pwe.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ack.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wzy.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yma.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sng.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://llc.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mmr.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jup.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://oqt.shzxlz.cn

Py:   Counter(arr)
来源：http://bdd.jianghu66.top

PHP:  array_count_values($arr);
来源：http://vrr.0kj1m.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sbq.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ikp.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nub.ybcxt.top

Go:   // 手写 map[T]int
来源：http://njk.ehwqpu.com

Ruby: arr.tally
来源：http://wrk.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vln.gzhubu.top

[D21] 判断是否包含某元素
来源：http://dmc.kuanghao11.cn

Py:   x in arr
来源：http://xll.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://tsp.meibo888.top

JS:   arr.includes(x)
来源：http://zxh.zdqjudy.top

TS:   arr.includes(x)
来源：http://gdu.meibo888.top

Java: list.contains(x)
来源：http://cub.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://ztr.tarul.cn

Ruby: arr.include?(x)
来源：http://dtn.cashguo.top

C#:   list.Contains(x)
来源：http://irc.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://dvw.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://plk.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rjm.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oou.c1oappe.top

TS:   [...arr];
来源：http://hkm.ydzc1.top

Java: new ArrayList<>(list);
来源：http://byp.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://jyw.hammf.cn

Ruby: arr.dup;  arr.clone
来源：http://ogn.snrcjt.cn

C#:   new List<int>(list);
来源：http://jwx.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://zjo.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ucs.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://buy.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lxr.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hic.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://yrn.hywenlv.cn

Go:   // 手写循环
来源：http://uqa.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cun.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ace.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://myj.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mst.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ozp.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sye.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ksw.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xyw.ywan-chungtsiang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mbh.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fyl.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lxh.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://jrd.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://odw.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wmj.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mbq.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uzm.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qys.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ufr.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fun.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dvp.shanyushiyangtech.top

[D26] 数组转字符串
来源：http://mxg.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://ivl.meibo888.top

PHP:  implode(", ", $arr);
来源：http://wdc.birdmap.top

JS:   arr.join(", ")
来源：http://qtd.yangfankeji.com

TS:   arr.join(", ")
来源：http://let.yanxiufei.cn

Java: String.join(", ", list)
来源：http://blx.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://pgd.mhx1999.top

Ruby: arr.join(", ")
来源：http://dyz.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://yjd.c1oappe.top

================================================================================
来源：http://ncg.aizwys.cn

E. 字符串处理
来源：http://bxa.mhx1999.top

================================================================================
来源：http://gny.ehwqpu.com

[E01] 拼接字符串
来源：http://qbv.vqdsnc.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://myq.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bdh.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oad.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dhx.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uik.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rpl.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rcn.jinqigfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jfp.meibo888.top

[E02] 重复字符串
来源：http://drv.hongshengwenyu.top

Py:   "ab" * 3
来源：http://kmu.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://fve.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://xuf.mhx1999.top

TS:   "ab".repeat(3)
来源：http://rvt.bjfxy.top

Java: "ab".repeat(3)
来源：http://zre.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://lxb.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://oai.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wfk.0kj1m.cn

[E03] 截取子串
来源：http://wcu.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cgp.zdbjq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yvp.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eje.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://ytw.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://cbx.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rbq.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://pof.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://bmq.jinqigfzy.top

[E04] 查找子串位置
来源：http://jzc.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://lcz.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://jvq.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ucj.jqgfzy.top

TS:   s.indexOf("x")
来源：http://guj.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://csr.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://ikp.zhoulong.xyz

Ruby: s.index("x")
来源：http://rdj.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://bhj.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gal.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rdu.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bik.xinyue.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ujj.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yvb.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vof.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eql.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jmi.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gte.epnwcf.com

[E06] 替换子串
来源：http://saq.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nro.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://rel.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lpl.sysykeji.top

TS:   s.replaceAll("a", "b")
来源：http://udi.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zjz.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ebi.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://axm.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://dpa.xziqi.cn

[E07] 按分隔符拆分
来源：http://xpk.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ddr.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ivn.feifeiyinyue.top


<!-- 参考信息 -->