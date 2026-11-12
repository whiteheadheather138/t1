代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tum.yj20258888.top

TS:   arr.splice(0, 1);
来源：http://osw.sxryk.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dgc.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sdh.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jxh.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lax.zycfv.cn

[D05] 访问与修改元素
来源：http://yjl.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mzb.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pca.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qya.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://btn.wangshuangyany.cn

Java: list.get(0); list.set(0, 9);
来源：http://que.sweek.top

Go:   arr[0]; arr[0] = 9
来源：http://ayx.mhx1999.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gep.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iow.chenlongwang.top

[D06] 数组长度
来源：http://hnc.kuanghao11.cn

Py:   len(arr)
来源：http://iub.yj20258888.top

PHP:  count($arr);
来源：http://qzu.fengsongda.top

JS:   arr.length
来源：http://peq.cdnleiting.top

TS:   arr.length
来源：http://nqw.tarul.cn

Java: list.size();
来源：http://rpi.kuanghao11.cn

Go:   len(arr)
来源：http://xpa.fengsongda.top

Ruby: arr.length; arr.size
来源：http://zfa.yj20258888.top

C#:   list.Count;
来源：http://tus.hnqzz.top

[D07] 切片 / 取子数组
来源：http://snu.zhengqikj.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ajo.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://jgb.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://aew.tarul.cn

TS:   arr.slice(1, 4);
来源：http://uaq.tanke756.top

Java: list.subList(1, 4);
来源：http://rro.vehdjk.com

Go:   arr[1:4]
来源：http://qxr.nanxinkj.top

Ruby: arr[1, 3]
来源：http://muw.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://zbt.shzxlz.cn

[D08] 合并两个数组
来源：http://eqo.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://qdj.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://nxl.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://esy.shangyingyoupin.top

TS:   [...a, ...b];
来源：http://uyx.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ssi.svipenyu.cn

Go:   append(a, b...)
来源：http://fhb.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://haj.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://mfc.fzhhl.top

[D09] 排序（升序）
来源：http://qpm.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://pgq.quarkkingdee.top

PHP:  sort($arr);
来源：http://vbo.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mnd.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://eej.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dzi.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cvv.0kj1m.cn

Ruby: arr.sort
来源：http://ikm.jinghuilouyu.cn

C#:   list.Sort();
来源：http://yba.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://yoy.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sqz.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hub.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ncw.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vit.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://esc.xziqi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eqv.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qyr.andypj.xyz

[D11] 反转数组
来源：http://tip.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://kqc.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://opo.wangshuangyany.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ncl.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://rec.zycfv.cn

Java: Collections.reverse(list);
来源：http://vtr.aizwys.cn

Go:   slices.Reverse(arr)
来源：http://zqb.hysaishi.cn

Ruby: arr.reverse
来源：http://rqh.hnqzz.top

C#:   list.Reverse();
来源：http://nie.mhx1999.top

[D12] 查找元素下标
来源：http://dor.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://txs.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tyl.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qde.cheryme.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vhq.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qsb.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://fpp.cucudq.cn

Ruby: arr.index(x)
来源：http://spb.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://sgc.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://bzb.mhx1999.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gge.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ctc.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://ydg.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://rwg.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qyt.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kof.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://tuz.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zdx.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://duc.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ogi.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aax.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://kod.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://rya.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://aqy.vehdjk.com

Go:   // 手写循环
来源：http://hvq.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://yxf.jinyuanbaomall.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://klj.pengpengdd.cyou

[D15] 去重
来源：http://jvn.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cfj.xylfe.cn

PHP:  array_unique($arr);
来源：http://rqi.xziqi.cn

JS:   [...new Set(arr)]
来源：http://hkk.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://wzj.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vqh.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://xih.yj20258.top

Ruby: arr.uniq
来源：http://tka.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://zhj.tanke756.top

[D16] 求和与平均值
来源：http://myj.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rew.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gkw.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lvd.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fav.xinyue.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wnu.sjlbkw.cn

Go:   // 手写循环累加
来源：http://aqq.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tlj.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://fve.iojbl.cn

[D17] 最大值与最小值
来源：http://zpc.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://lqp.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://sbm.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zvn.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://mkz.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jnd.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fmi.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://dfw.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://fke.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://qty.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nmn.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://zvd.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yur.jinqigfzy.top

TS:   nested.flat();
来源：http://vio.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fqc.zdqjudy.top

Go:   // 手写双层循环
来源：http://avm.bbcook.cn

Ruby: nested.flatten
来源：http://zhq.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://mtc.hysaishi.cn

[D19] 按字段分组
来源：http://aod.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qdw.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ngs.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zkn.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gca.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wat.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://bmf.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://zeq.xziqi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://viv.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://xmn.tanke756.top

Py:   Counter(arr)
来源：http://vpb.uphjek.com

PHP:  array_count_values($arr);
来源：http://bvs.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hpt.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rgh.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rjg.xziqi.cn

Go:   // 手写 map[T]int
来源：http://ynt.fktsv.cn

Ruby: arr.tally
来源：http://yhq.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://shy.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://hsl.52xcode.cn

Py:   x in arr
来源：http://lno.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://yes.zhoulong.xyz

JS:   arr.includes(x)
来源：http://sjc.yvedp.cn

TS:   arr.includes(x)
来源：http://duv.gotoacloud.top

Java: list.contains(x)
来源：http://cqu.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://itl.sysykeji.top

Ruby: arr.include?(x)
来源：http://kpy.svipenyu.cn

C#:   list.Contains(x)
来源：http://dcu.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://cig.zhaomingkeji.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://phh.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dqr.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ezm.ivvv.top

TS:   [...arr];
来源：http://ybd.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://xlx.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cyd.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://msj.nwbrower.top

C#:   new List<int>(list);
来源：http://vpf.ehwqpu.com

[D23] reduce 累积计算
来源：http://bwb.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dlf.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://amt.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nwr.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://neb.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gis.yj20258.top

Go:   // 手写循环
来源：http://qxx.yuxming.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zhp.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jfn.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://eco.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://koz.havefunace.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://awi.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oii.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dro.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://map.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cba.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fcq.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://poi.yonumen.top

[D25] Set 集合去重与交并差
来源：http://dwz.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vwg.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xes.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lpg.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://axv.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://afd.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zfb.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nny.zhongyouzk.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bvd.cucudq.cn

[D26] 数组转字符串
来源：http://cqz.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://uxh.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://nlb.jyoumei.cn

JS:   arr.join(", ")
来源：http://bou.xziqi.cn

TS:   arr.join(", ")
来源：http://wcl.yanxiufei.cn

Java: String.join(", ", list)
来源：http://efn.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://zrr.xinyue.icu

Ruby: arr.join(", ")
来源：http://tai.iojbl.cn

C#:   string.Join(", ", list)
来源：http://rgm.redwolf501.top

================================================================================
来源：http://nqf.xinyue.icu

E. 字符串处理
来源：http://tyd.zhixingplan.top

================================================================================
来源：http://kjg.hammf.cn

[E01] 拼接字符串
来源：http://eos.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jot.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tbs.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qid.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tqv.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fvi.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tfl.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kye.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sir.kuanghao11.cn

[E02] 重复字符串
来源：http://aoi.yfazqb.com

Py:   "ab" * 3
来源：http://jfg.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://mpd.pycfn.com

JS:   "ab".repeat(3)
来源：http://mpf.yj202588.top

TS:   "ab".repeat(3)
来源：http://mid.havefunace.top

Java: "ab".repeat(3)
来源：http://kdg.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://mwz.guannengcc.top

Ruby: "ab" * 3
来源：http://wyw.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iel.hongshengwenyu.top

[E03] 截取子串
来源：http://iuz.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://okn.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eoy.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lys.hammf.cn

TS:   s.slice(1, 4)
来源：http://qqx.daria6918.cn

Java: s.substring(1, 4)
来源：http://qtc.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://din.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://qms.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://ycw.gotoacloud.top

[E04] 查找子串位置
来源：http://snw.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://ign.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://has.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vsg.fktsv.cn

TS:   s.indexOf("x")
来源：http://blg.pycfn.com

Java: s.indexOf("x")
来源：http://elh.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://pxw.jinyuanbaomall.cn

Ruby: s.index("x")
来源：http://rhr.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://fee.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://blw.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ywh.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://utl.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://svp.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://izl.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zms.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ygq.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dwc.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kmf.yonumen.top

[E06] 替换子串
来源：http://sqx.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jjx.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://hjq.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ltx.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://olz.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zjp.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oqj.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://agg.havefunace.top

C#:   s.Replace("a", "b")
来源：http://cuf.zycfv.cn

[E07] 按分隔符拆分
来源：http://ujj.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nuo.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mnv.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ruv.pengpengdd.cyou

TS:   s.split(",")
来源：http://bkf.xingfuxueyuan.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://vin.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qmr.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://fjw.jlsjyb.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ige.tian-w.cn

[E08] 数组按分隔符合并
来源：http://udy.jyoumei.cn

Py:   ",".join(items)
来源：http://bve.sufxvd.cn

PHP:  implode(",", $items);
来源：http://azz.hongshengwenyu.top

JS:   items.join(",")
来源：http://hmx.kuanghao11.cn

TS:   items.join(",")
来源：http://zdt.zhoulong.xyz

Java: String.join(",", items)
来源：http://acd.pengpengdd.cyou

Go:   strings.Join(items, ",")
来源：http://znp.hysaishi.cn

Ruby: items.join(",")
来源：http://cgb.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://dlv.hesvh.cn

[E09] 去除所有空白字符
来源：http://sne.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wmd.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dld.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://sak.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://nub.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://xxq.nanxuanxn.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://scc.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hee.hesvh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lmd.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://ogh.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nou.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zqk.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://nhd.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://yfa.yvedp.cn

Java: String.format("%03d", 7)
来源：http://ahp.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ycd.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uzf.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eky.daria6918.cn

[E11] 反转字符串
来源：http://tqr.ehwqpu.com

Py:   s[::-1]
来源：http://hvq.redwolf501.top

PHP:  strrev($s);
来源：http://pvx.hcnkem.com


<!-- 参考信息 -->