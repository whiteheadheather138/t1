代发 wailian999

Java: list.add(4);
来源：http://exi.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://fyv.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://rda.nwbrower.top

C#:   list.Add(4);
来源：http://skh.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://cqh.snrcjt.cn

Py:   arr.insert(0, 0)
来源：http://lkn.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ygh.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://icl.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://eeo.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://usz.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://wqm.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sqp.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://fpp.hnqzz.top

[D04] 删除元素
来源：http://lel.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ieb.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nyx.zhijiandao.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ohd.hnxiangtu.top

TS:   arr.splice(0, 1);
来源：http://yja.jinyuanbaomall.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xlk.nanxuanxn.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tbb.cucudq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://azx.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hjk.yueranfly.top

[D05] 访问与修改元素
来源：http://ehj.cdnleiting.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cdf.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sxb.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nnv.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://xyv.0kj1m.cn

Java: list.get(0); list.set(0, 9);
来源：http://voz.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://yhk.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wxf.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gri.0kj1m.cn

[D06] 数组长度
来源：http://ycs.hesvh.cn

Py:   len(arr)
来源：http://mni.yuanzhike.top

PHP:  count($arr);
来源：http://czd.nwbrower.top

JS:   arr.length
来源：http://sko.nanxuanxn.top

TS:   arr.length
来源：http://uqu.hnqzz.top

Java: list.size();
来源：http://oay.bbcook.cn

Go:   len(arr)
来源：http://skk.vqdsnc.cn

Ruby: arr.length; arr.size
来源：http://pia.birdmap.top

C#:   list.Count;
来源：http://sxt.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://ibk.smart0.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aik.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fms.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://frb.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://kty.snrcjt.cn

Java: list.subList(1, 4);
来源：http://lzh.bbcook.cn

Go:   arr[1:4]
来源：http://ojl.redwolf501.top

Ruby: arr[1, 3]
来源：http://yfy.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://jqy.hesvh.cn

[D08] 合并两个数组
来源：http://vls.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://ifi.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://mkw.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://evq.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://iis.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oyr.daxiang520.top

Go:   append(a, b...)
来源：http://deh.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://lvo.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://ici.fehbvm.com

[D09] 排序（升序）
来源：http://kyf.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://dae.jianghu66.top

PHP:  sort($arr);
来源：http://vhg.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kvt.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://zzh.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ckw.fzhhl.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hja.sjlbkw.cn

Ruby: arr.sort
来源：http://swq.vehdjk.com

C#:   list.Sort();
来源：http://cqq.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yot.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ahv.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yfk.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wxe.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://euf.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ifs.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iom.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qvr.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://awi.iojbl.cn

[D11] 反转数组
来源：http://gzb.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://nxl.tarul.cn

PHP:  array_reverse($arr);
来源：http://eig.wangshuangyany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yib.jqgfzy.top

TS:   [...arr].reverse();
来源：http://tgk.dianchejie.cn

Java: Collections.reverse(list);
来源：http://jbp.havefunace.top

Go:   slices.Reverse(arr)
来源：http://eno.kuanghao11.cn

Ruby: arr.reverse
来源：http://kos.yuanzhike.top

C#:   list.Reverse();
来源：http://bpw.hongshengwenyu.top

[D12] 查找元素下标
来源：http://yme.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://evs.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ikt.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://idb.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://emy.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://flr.nanxinkj.top

Go:   slices.Index(arr, x)
来源：http://dea.hammf.cn

Ruby: arr.index(x)
来源：http://yuf.hnxiangtu.top

C#:   list.IndexOf(x);
来源：http://lvi.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://rsy.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aoi.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tko.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://ntr.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://msd.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mhn.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jct.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://qve.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://vcn.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://wdd.jlsjyb.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xig.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vzd.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://ctm.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://nkq.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hbx.jqgfzy.top

Go:   // 手写循环
来源：http://fwd.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ftn.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rab.smart0.xyz

[D15] 去重
来源：http://mkj.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hgq.zycfv.cn

PHP:  array_unique($arr);
来源：http://hqw.fzhhl.top

JS:   [...new Set(arr)]
来源：http://zde.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://igh.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rmo.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://wfz.hnqzz.top

Ruby: arr.uniq
来源：http://caq.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://uyn.snrcjt.cn

[D16] 求和与平均值
来源：http://utt.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xwe.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zgn.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lyu.tanke756.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vdr.guannengcc.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rgi.tianlin.xyz

Go:   // 手写循环累加
来源：http://xfz.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kiq.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://xod.hywenlv.cn

[D17] 最大值与最小值
来源：http://kls.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://tlw.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://hjh.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wwm.chenlongwang.top

TS:   Math.max(...arr);
来源：http://hrs.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://yrr.0kj1m.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://paw.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://mpj.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://spb.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://qul.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iig.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://jhe.dashuyun.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jck.xuanzx.com

TS:   nested.flat();
来源：http://fss.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zjq.yueranfly.top

Go:   // 手写双层循环
来源：http://lqk.jlsjyb.cn

Ruby: nested.flatten
来源：http://jmj.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bdg.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://qpu.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://grv.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://whl.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rve.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zec.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jyi.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://pzz.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://olg.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mcf.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://axe.jlsjyb.cn

Py:   Counter(arr)
来源：http://taa.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://gmp.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hll.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kov.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ttz.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://dga.bbcook.cn

Ruby: arr.tally
来源：http://diu.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aqx.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://bny.fktsv.cn

Py:   x in arr
来源：http://htx.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://kyy.guowangkeji.top

JS:   arr.includes(x)
来源：http://yji.shzxlz.cn

TS:   arr.includes(x)
来源：http://zgp.zdqjudy.top

Java: list.contains(x)
来源：http://myv.zhaomingkeji.xyz

Go:   slices.Contains(arr, x)
来源：http://nuu.daxiang520.top

Ruby: arr.include?(x)
来源：http://bin.yangfankeji.com

C#:   list.Contains(x)
来源：http://jyf.fzhhl.top

[D22] 复制数组（避免共享引用）
来源：http://osp.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://exq.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mes.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qmt.zhixingplan.top

TS:   [...arr];
来源：http://rcy.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://nkh.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://kjx.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://dzx.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://smc.zycfv.cn

[D23] reduce 累积计算
来源：http://stq.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ftm.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kej.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://owp.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kme.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://grj.wangdashe.top

Go:   // 手写循环
来源：http://tva.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://all.jinqigufen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xyf.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://zip.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ktx.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bze.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://njk.cheryme.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://djh.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mtc.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gbg.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hgw.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hbs.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://qjj.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iej.c1oappe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gri.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jgm.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ehd.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dld.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xoa.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pvb.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xag.zhoulong.xyz

[D26] 数组转字符串
来源：http://gww.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://dyb.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://shj.cucudq.cn

JS:   arr.join(", ")
来源：http://xad.yj20258888.top

TS:   arr.join(", ")
来源：http://smi.daria6918.cn

Java: String.join(", ", list)
来源：http://uzt.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://gzi.zhengqikj.top

Ruby: arr.join(", ")
来源：http://sdy.sysykeji.top

C#:   string.Join(", ", list)
来源：http://cvx.yj20258.top

================================================================================
来源：http://gfb.xuetiantiany.cn

E. 字符串处理
来源：http://ejy.sxryk.cn

================================================================================
来源：http://tyg.sysykeji.top

[E01] 拼接字符串
来源：http://odx.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hep.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jhd.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lng.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nir.feifeiyinyue.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ajv.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://njv.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rgn.jlsjyb.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://axq.jinqigfzy.top

[E02] 重复字符串
来源：http://kzy.shuidangran.top

Py:   "ab" * 3
来源：http://jxh.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://tjy.yonumen.top

JS:   "ab".repeat(3)
来源：http://mir.jianghu66.top

TS:   "ab".repeat(3)
来源：http://xck.jianghu66.top

Java: "ab".repeat(3)
来源：http://hoa.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://spp.yueranfly.top

Ruby: "ab" * 3
来源：http://ade.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vqq.zhongyouzk.top

[E03] 截取子串
来源：http://ocp.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tso.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rpn.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lyy.birdmap.top

TS:   s.slice(1, 4)
来源：http://fkn.haohaochexian.top

Java: s.substring(1, 4)
来源：http://tyf.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qhc.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://ovi.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://yoj.mhx1999.top

[E04] 查找子串位置
来源：http://qex.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://tki.yj20258888.top

PHP:  strpos($s, "x");
来源：http://ulu.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rnp.yonumen.top

TS:   s.indexOf("x")
来源：http://jho.gzhubu.top

Java: s.indexOf("x")
来源：http://iha.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://aqk.smart0.xyz

Ruby: s.index("x")
来源：http://zdk.pycfn.com

C#:   s.IndexOf("x")
来源：http://lws.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qjr.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ton.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hhy.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qza.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qpg.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egt.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ndr.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://msg.xingfuxueyuan.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rnh.haohaochexian.top

[E06] 替换子串
来源：http://jcd.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fwf.jinyuanbaomall.cn

PHP:  str_replace("a", "b", $s);
来源：http://cpr.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xxa.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://dmf.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lza.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oxc.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uwx.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://hdb.haohaochexian.top

[E07] 按分隔符拆分
来源：http://cey.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dfn.shangyingyoupin.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qqf.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jgh.zhengqikj.top

TS:   s.split(",")
来源：http://tod.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dbv.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uzq.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://qyu.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qkm.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://zzr.52xcode.cn

Py:   ",".join(items)
来源：http://zop.jqgfzy.top

PHP:  implode(",", $items);
来源：http://xfw.shangyingyoupin.top

JS:   items.join(",")
来源：http://qaq.sxryk.cn

TS:   items.join(",")
来源：http://kpt.gogol.net.cn

Java: String.join(",", items)
来源：http://kso.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://mrb.epnwcf.com

Ruby: items.join(",")
来源：http://njt.snrcjt.cn

C#:   string.Join(",", items)
来源：http://szm.jinqigufen.top

[E09] 去除所有空白字符
来源：http://zsg.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qsg.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jlg.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://zlx.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://bcw.uphjek.com


<!-- 参考信息 -->