代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xrd.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://klf.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lsj.sweek.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zdj.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rsc.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vol.haohaochexian.top

[D05] 访问与修改元素
来源：http://xmx.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tmm.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pfv.chenjidiqi.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ylx.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://ote.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://tmh.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://zso.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pry.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://viq.fktsv.cn

[D06] 数组长度
来源：http://kyi.mhx1999.top

Py:   len(arr)
来源：http://zou.cucudq.cn

PHP:  count($arr);
来源：http://hor.yonumen.top

JS:   arr.length
来源：http://iom.zhixingplan.top

TS:   arr.length
来源：http://fpo.vehdjk.com

Java: list.size();
来源：http://ash.cashguo.top

Go:   len(arr)
来源：http://jir.tarul.cn

Ruby: arr.length; arr.size
来源：http://iit.nanxinkj.top

C#:   list.Count;
来源：http://hlm.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://edm.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ymn.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://piu.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://gjt.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://tyn.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://mzf.kuanghao11.cn

Go:   arr[1:4]
来源：http://dwe.iojbl.cn

Ruby: arr[1, 3]
来源：http://ghh.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://ean.bbcook.cn

[D08] 合并两个数组
来源：http://mtp.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://qqv.yfazqb.com

PHP:  array_merge($a, $b);
来源：http://prb.ydzc1.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qvs.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://wcn.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vtc.shangyingyoupin.top

Go:   append(a, b...)
来源：http://iaj.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://pls.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://xwk.epnwcf.com

[D09] 排序（升序）
来源：http://eoh.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://nho.hywenlv.cn

PHP:  sort($arr);
来源：http://wti.ywan-chungtsiang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gdk.yangfankeji.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xfw.zhoulong.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://jyf.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qqq.jinqigfzy.top

Ruby: arr.sort
来源：http://hqt.bjfxy.top

C#:   list.Sort();
来源：http://mtt.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lne.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vgl.chenzaomai.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://upi.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mty.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ltq.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yyk.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://klv.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mqe.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ono.ydjk.org.cn

[D11] 反转数组
来源：http://dvb.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://rew.vehdjk.com

PHP:  array_reverse($arr);
来源：http://box.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mzb.nwbrower.top

TS:   [...arr].reverse();
来源：http://ivz.yvedp.cn

Java: Collections.reverse(list);
来源：http://rfv.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://yib.hesvh.cn

Ruby: arr.reverse
来源：http://hah.aizwys.cn

C#:   list.Reverse();
来源：http://hlz.ybcxt.top

[D12] 查找元素下标
来源：http://rfr.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://efo.yangfankeji.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dno.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmt.gogol.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ewl.wangdashe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dgu.birdmap.top

Go:   slices.Index(arr, x)
来源：http://ovx.zdqjudy.top

Ruby: arr.index(x)
来源：http://kno.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://bzz.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://ira.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nya.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://smz.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://epm.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://xzz.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nhw.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nht.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bio.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rbb.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://cbe.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ojo.cqqwz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yke.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://jbs.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://gne.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hyv.andypj.xyz

Go:   // 手写循环
来源：http://ffv.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://xcu.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bnc.gaohongyu789.top

[D15] 去重
来源：http://gsi.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pkn.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://eyr.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://liu.xinyue.icu

TS:   [...new Set(arr)]
来源：http://ygk.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ujg.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://mnz.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://gdo.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://bdn.yfazqb.com

[D16] 求和与平均值
来源：http://igy.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://owh.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bca.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mrj.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zuy.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gdg.jqgufenzy.top

Go:   // 手写循环累加
来源：http://nim.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vzc.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://yar.guowangkeji.top

[D17] 最大值与最小值
来源：http://vug.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://liw.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://zcy.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hjv.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://fea.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dnh.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nih.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://onm.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://elz.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://rup.cashguo.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rhw.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://hfd.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wrz.shanyushiyangtech.top

TS:   nested.flat();
来源：http://wye.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ocf.guowangkeji.top

Go:   // 手写双层循环
来源：http://xbr.aibaodan.cn

Ruby: nested.flatten
来源：http://tew.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zev.gaohongyu789.top

[D19] 按字段分组
来源：http://ekb.ydzc1.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aom.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://enj.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vew.jiagoushi.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://opq.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wmc.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://eye.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zel.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ycx.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://zvu.dianchejie.cn

Py:   Counter(arr)
来源：http://wre.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://zxv.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wmz.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vwz.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bdp.fktsv.cn

Go:   // 手写 map[T]int
来源：http://kjr.xuanzx.com

Ruby: arr.tally
来源：http://cyl.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xkz.sysykeji.top

[D21] 判断是否包含某元素
来源：http://jge.smart0.xyz

Py:   x in arr
来源：http://snk.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://ycd.yuxming.cn

JS:   arr.includes(x)
来源：http://xob.epnwcf.com

TS:   arr.includes(x)
来源：http://umz.uphjek.com

Java: list.contains(x)
来源：http://zxx.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://tve.yonumen.top

Ruby: arr.include?(x)
来源：http://fdr.ivvv.top

C#:   list.Contains(x)
来源：http://jmh.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://iur.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cwo.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dtz.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ris.hammf.cn

TS:   [...arr];
来源：http://aps.ehwqpu.com

Java: new ArrayList<>(list);
来源：http://cgc.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://fap.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://hsc.ydjk.org.cn

C#:   new List<int>(list);
来源：http://jvy.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://hkj.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mxi.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fnj.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yur.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kpo.zdbjq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yrh.tanke756.top

Go:   // 手写循环
来源：http://ttb.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://npn.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://evb.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://met.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bkk.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pkd.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rpu.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gny.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qve.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lbh.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uew.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ivu.uphjek.com

[D25] Set 集合去重与交并差
来源：http://yiu.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tfs.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hsb.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hmg.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ukd.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xzc.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vrp.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nyu.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pdn.chenzaomai.com

[D26] 数组转字符串
来源：http://ytn.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://rwf.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://fcb.jianghu66.top

JS:   arr.join(", ")
来源：http://pms.ctjpmb.com

TS:   arr.join(", ")
来源：http://umh.yuanzhike.top

Java: String.join(", ", list)
来源：http://hdp.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://avt.bjfxy.top

Ruby: arr.join(", ")
来源：http://bxw.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://jjh.xziqi.cn

================================================================================
来源：http://fve.zdqjudy.top

E. 字符串处理
来源：http://luj.sxryk.cn

================================================================================
来源：http://ncw.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://chr.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ahz.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xbw.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lgx.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://knd.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cnk.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jsy.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ebr.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jsp.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://int.sysykeji.top

Py:   "ab" * 3
来源：http://hll.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://tik.meibo888.top

JS:   "ab".repeat(3)
来源：http://eiq.tarul.cn

TS:   "ab".repeat(3)
来源：http://pqj.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://anq.yueranfly.top

Go:   strings.Repeat("ab", 3)
来源：http://dqv.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://neu.guowangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pup.tian-w.cn

[E03] 截取子串
来源：http://aip.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rut.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kwv.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://roj.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://nxs.yangfankeji.com

Java: s.substring(1, 4)
来源：http://iuo.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wia.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ybh.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://yna.yonumen.top

[E04] 查找子串位置
来源：http://fza.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://mfm.epnwcf.com

PHP:  strpos($s, "x");
来源：http://wdz.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jan.fanxiaobao.xyz

TS:   s.indexOf("x")
来源：http://ius.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://uew.yongpay.top

Go:   strings.Index(s, "x")
来源：http://oth.zhoulong.xyz

Ruby: s.index("x")
来源：http://dmt.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://gis.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sak.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uzi.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://owl.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dnp.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kka.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://orw.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vth.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lik.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ogr.316326.xyz

[E06] 替换子串
来源：http://tlz.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://azp.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://tzi.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ykj.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://irv.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://brb.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qca.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yge.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://wyo.epnwcf.com

[E07] 按分隔符拆分
来源：http://rbj.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tzc.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uhw.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pah.chenlongwang.top

TS:   s.split(",")
来源：http://ova.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xpg.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hja.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://gqv.havefunace.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mwt.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://ksi.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://ovs.tianlin.xyz

PHP:  implode(",", $items);
来源：http://lvx.tanke756.top

JS:   items.join(",")
来源：http://cpl.snrcjt.cn

TS:   items.join(",")
来源：http://wnt.tianlin.xyz

Java: String.join(",", items)
来源：http://ufg.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://unv.zhengqikj.top

Ruby: items.join(",")
来源：http://ytq.tianlin.xyz

C#:   string.Join(",", items)
来源：http://mke.dianchejie.cn

[E09] 去除所有空白字符
来源：http://pxg.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ipq.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pwj.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://inb.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://nyt.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://vya.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ehw.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://flj.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rtj.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://twg.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hlj.ivvv.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ueb.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://jsw.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://gky.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://jny.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yms.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ovn.gogol.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gox.yonumen.top

[E11] 反转字符串
来源：http://lxw.nanxuanxn.top

Py:   s[::-1]
来源：http://gqm.daxiang520.top

PHP:  strrev($s);
来源：http://qyy.jianghu66.top


<!-- 参考信息 -->