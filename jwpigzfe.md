代发 wailian999

Java: list.add(4);
来源：http://yby.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://lcs.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://ica.jianghu66.top

C#:   list.Add(4);
来源：http://edy.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://dpe.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://kmj.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cbz.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fdz.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://krt.vehdjk.com

Java: list.add(0, 0);
来源：http://oaa.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fro.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lrc.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://kwv.hnxiangtu.top

[D04] 删除元素
来源：http://bnz.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lde.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lip.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ajy.vehdjk.com

TS:   arr.splice(0, 1);
来源：http://itd.daxiang520.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eqg.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vra.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kiq.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pke.andypj.xyz

[D05] 访问与修改元素
来源：http://pce.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zgv.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://acm.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gax.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://cjd.meibo888.top

Java: list.get(0); list.set(0, 9);
来源：http://ejc.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://uoc.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sik.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qwi.zdqjudy.top

[D06] 数组长度
来源：http://uyx.gotoacloud.top

Py:   len(arr)
来源：http://rob.pycfn.com

PHP:  count($arr);
来源：http://pap.iojbl.cn

JS:   arr.length
来源：http://phs.yonumen.top

TS:   arr.length
来源：http://ics.dianchejie.cn

Java: list.size();
来源：http://igk.guowangkeji.top

Go:   len(arr)
来源：http://usy.hysaishi.cn

Ruby: arr.length; arr.size
来源：http://pqt.xylfe.cn

C#:   list.Count;
来源：http://cky.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://haj.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vzo.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ihr.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://lkd.nwbrower.top

TS:   arr.slice(1, 4);
来源：http://xlg.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://tta.havefunace.top

Go:   arr[1:4]
来源：http://ylo.sxryk.cn

Ruby: arr[1, 3]
来源：http://vet.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://oyo.wangshuangyany.cn

[D08] 合并两个数组
来源：http://kzu.smart0.xyz

Py:   a + b;  a.extend(b)
来源：http://cne.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://bgu.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tak.sysykeji.top

TS:   [...a, ...b];
来源：http://jmh.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jhi.smart0.xyz

Go:   append(a, b...)
来源：http://tqq.svipenyu.cn

Ruby: a + b;  a.concat(b)
来源：http://iur.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://fpy.yfazqb.com

[D09] 排序（升序）
来源：http://edy.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ktu.vqdsnc.cn

PHP:  sort($arr);
来源：http://phe.tianlin.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xgk.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yab.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://yxq.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tsy.guannengcc.top

Ruby: arr.sort
来源：http://vdw.xuanzx.com

C#:   list.Sort();
来源：http://kcy.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wef.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lvh.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jmo.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ynd.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fam.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://whl.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wtl.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fhf.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lom.meibo888.top

[D11] 反转数组
来源：http://msq.mhx1999.top

Py:   arr[::-1];  arr.reverse()
来源：http://owb.ydzc1.top

PHP:  array_reverse($arr);
来源：http://mbq.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://alc.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://rvn.jinqigufen.top

Java: Collections.reverse(list);
来源：http://sks.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://nwk.gotoacloud.top

Ruby: arr.reverse
来源：http://kvz.sufxvd.cn

C#:   list.Reverse();
来源：http://qkh.aibaodan.cn

[D12] 查找元素下标
来源：http://jye.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://rme.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ikn.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sde.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://euu.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cgb.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://lpz.yj20258888.top

Ruby: arr.index(x)
来源：http://bmq.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://tcc.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://fhe.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qpx.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vmq.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://vdk.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://rvr.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ycg.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gta.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cgs.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rgq.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://sdu.haohaochexian.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mba.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yik.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://mab.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://fdo.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xny.zhoulong.xyz

Go:   // 手写循环
来源：http://uxq.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://wrm.ydjk.org.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lds.zhoulong.xyz

[D15] 去重
来源：http://uqq.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yja.hesvh.cn

PHP:  array_unique($arr);
来源：http://hne.fengsongda.top

JS:   [...new Set(arr)]
来源：http://gxp.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://pqw.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gqe.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://kra.snrcjt.cn

Ruby: arr.uniq
来源：http://ljs.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://kyb.yueranfly.top

[D16] 求和与平均值
来源：http://caa.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jpr.gogol.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://orw.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgf.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vam.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kid.hysaishi.cn

Go:   // 手写循环累加
来源：http://ebj.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fcu.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://xwn.meibo888.top

[D17] 最大值与最小值
来源：http://glm.yongpay.top

Py:   max(arr);  min(arr)
来源：http://lkx.zdbjq.cn

PHP:  max($arr);  min($arr);
来源：http://vfu.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xei.sweek.top

TS:   Math.max(...arr);
来源：http://tyu.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://acx.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xqt.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://bby.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://ern.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://bnj.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fsc.zhiwuduotai.top

PHP:  array_merge(...$nested);
来源：http://ejc.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ido.fktsv.cn

TS:   nested.flat();
来源：http://wgh.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vin.chenlongwang.top

Go:   // 手写双层循环
来源：http://njj.gogol.net.cn

Ruby: nested.flatten
来源：http://vvo.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hkc.sufxvd.cn

[D19] 按字段分组
来源：http://sem.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ixo.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fum.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kwg.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bfj.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bgc.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://sep.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oov.quarkkingdee.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uof.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://fha.vehdjk.com

Py:   Counter(arr)
来源：http://mlg.yj20258.top

PHP:  array_count_values($arr);
来源：http://ykj.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ttu.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kgx.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yyj.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://wpy.chenjidiqi.icu

Ruby: arr.tally
来源：http://ucs.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pib.zhaomingkeji.xyz

[D21] 判断是否包含某元素
来源：http://xbc.xziqi.cn

Py:   x in arr
来源：http://xny.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://vva.dashuyun.cn

JS:   arr.includes(x)
来源：http://rgc.fengsongda.top

TS:   arr.includes(x)
来源：http://gwt.yanxiufei.cn

Java: list.contains(x)
来源：http://bmx.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://sau.bjfxy.top

Ruby: arr.include?(x)
来源：http://ibx.kuanghao11.cn

C#:   list.Contains(x)
来源：http://lix.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://fui.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bnu.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uqo.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vth.yonumen.top

TS:   [...arr];
来源：http://vni.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://ewn.316326.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ohp.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://puw.ydjk.org.cn

C#:   new List<int>(list);
来源：http://pyw.cqqwz.cn

[D23] reduce 累积计算
来源：http://dhg.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://byz.tarul.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iaa.xylfe.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cwa.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cpv.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://njv.zdbjq.cn

Go:   // 手写循环
来源：http://kev.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jql.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://laz.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://znd.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rxg.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nsx.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://net.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oxi.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dvo.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kky.xuetiantiany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qxz.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ofg.xinyue.icu

[D25] Set 集合去重与交并差
来源：http://vae.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pnt.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xyr.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://utm.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ozt.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://soi.cucudq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dzt.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cag.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://apw.havefunace.top

[D26] 数组转字符串
来源：http://vag.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://ylr.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://cxs.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://fri.andypj.xyz

TS:   arr.join(", ")
来源：http://vrh.fehbvm.com

Java: String.join(", ", list)
来源：http://hgr.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://oyn.ctjpmb.com

Ruby: arr.join(", ")
来源：http://wrv.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://nhh.shanyushiyangtech.top

================================================================================
来源：http://zsk.zdbjq.cn

E. 字符串处理
来源：http://nqf.xuanzx.com

================================================================================
来源：http://mde.9152youxi.cn

[E01] 拼接字符串
来源：http://qic.gotoacloud.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kwn.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kii.yfazqb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qwu.havefunace.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xep.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cqb.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pej.quarkkingdee.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://diu.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dgi.uphjek.com

[E02] 重复字符串
来源：http://tvn.nanxinkj.top

Py:   "ab" * 3
来源：http://ewp.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://fjc.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://qkb.zdqjudy.top

TS:   "ab".repeat(3)
来源：http://xgr.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://ncw.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://qly.daria6918.cn

Ruby: "ab" * 3
来源：http://srl.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gwj.shzxlz.cn

[E03] 截取子串
来源：http://bkl.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bcx.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qzs.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://drj.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://zvj.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://zkt.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ksz.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://crs.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://jgf.yvedp.cn

[E04] 查找子串位置
来源：http://ufw.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://sti.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://hyi.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dnd.uphjek.com

TS:   s.indexOf("x")
来源：http://pus.zhixingplan.top

Java: s.indexOf("x")
来源：http://cjc.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://rqj.hammf.cn

Ruby: s.index("x")
来源：http://zov.sweek.top

C#:   s.IndexOf("x")
来源：http://txi.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bnk.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://crl.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ofw.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rhr.xuanzx.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://aso.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yxc.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://amg.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://njo.hesvh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zsz.chenlongwang.top

[E06] 替换子串
来源：http://jmh.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://krs.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://thh.meibo888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://omu.yj202588.top

TS:   s.replaceAll("a", "b")
来源：http://ygs.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ozv.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lxw.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uod.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://upy.aibaodan.cn

[E07] 按分隔符拆分
来源：http://qnq.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iqv.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jzh.quarkkingdee.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lhl.fengsongda.top

TS:   s.split(",")
来源：http://ncm.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://huu.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cio.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://vdz.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uyq.sufxvd.cn

[E08] 数组按分隔符合并
来源：http://tjw.vqdsnc.cn

Py:   ",".join(items)
来源：http://obz.gzhubu.top

PHP:  implode(",", $items);
来源：http://fms.ybcxt.top

JS:   items.join(",")
来源：http://hhj.zhijiandao.cn

TS:   items.join(",")
来源：http://xjq.hongshengwenyu.top

Java: String.join(",", items)
来源：http://exp.ivvv.top

Go:   strings.Join(items, ",")
来源：http://kgk.yanxiufei.cn

Ruby: items.join(",")
来源：http://emj.redwolf501.top

C#:   string.Join(",", items)
来源：http://xbr.yvedp.cn

[E09] 去除所有空白字符
来源：http://dbk.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dqo.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gnj.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://vro.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://sxa.yueranfly.top


<!-- 参考信息 -->