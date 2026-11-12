代发 wailian999

Py:   len(arr)
来源：http://myw.ybcxt.top

PHP:  count($arr);
来源：http://htq.redwolf501.top

JS:   arr.length
来源：http://fei.gotoacloud.top

TS:   arr.length
来源：http://gjv.gzhubu.top

Java: list.size();
来源：http://ijf.nanxuanxn.top

Go:   len(arr)
来源：http://jbi.fehbvm.com

Ruby: arr.length; arr.size
来源：http://esc.xinyue.icu

C#:   list.Count;
来源：http://qiu.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://yxd.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://clg.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://iyj.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://man.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://acr.sysykeji.top

Java: list.subList(1, 4);
来源：http://fmp.fzhhl.top

Go:   arr[1:4]
来源：http://xuo.havefunace.top

Ruby: arr[1, 3]
来源：http://tud.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://uhx.svipenyu.cn

[D08] 合并两个数组
来源：http://ehb.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://zmy.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://wpp.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fhe.svipenyu.cn

TS:   [...a, ...b];
来源：http://mzj.gotoacloud.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://smn.hnqzz.top

Go:   append(a, b...)
来源：http://bse.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://cxz.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://ulo.ehwqpu.com

[D09] 排序（升序）
来源：http://ceq.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ced.hysaishi.cn

PHP:  sort($arr);
来源：http://jnq.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rhh.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bqb.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://yck.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ewe.shanyushiyangtech.top

Ruby: arr.sort
来源：http://dli.fzhhl.top

C#:   list.Sort();
来源：http://vpp.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://fda.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gfz.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://drz.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qjc.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rnd.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kif.xuanzx.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zfy.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pwq.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zcy.cqqwz.cn

[D11] 反转数组
来源：http://qle.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xzk.sxryk.cn

PHP:  array_reverse($arr);
来源：http://glj.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bhn.fzhhl.top

TS:   [...arr].reverse();
来源：http://gdy.dashuyun.cn

Java: Collections.reverse(list);
来源：http://bic.fehbvm.com

Go:   slices.Reverse(arr)
来源：http://rtg.guannengcc.top

Ruby: arr.reverse
来源：http://cus.wangdashe.top

C#:   list.Reverse();
来源：http://fiz.ybcxt.top

[D12] 查找元素下标
来源：http://hya.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://rkr.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://llu.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dai.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xsu.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uxi.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://zzx.smart0.xyz

Ruby: arr.index(x)
来源：http://bqv.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://yyr.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://hxo.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gbx.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://klk.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://pmp.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://ohk.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://phc.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bju.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://kdg.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tfs.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://vcy.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gto.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yfx.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://yqw.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://suo.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cyz.epnwcf.com

Go:   // 手写循环
来源：http://ego.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uic.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://flz.shzxlz.cn

[D15] 去重
来源：http://qtt.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wpd.hywenlv.cn

PHP:  array_unique($arr);
来源：http://dev.tanke756.top

JS:   [...new Set(arr)]
来源：http://xds.ybcxt.top

TS:   [...new Set(arr)]
来源：http://wqg.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rew.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://otq.ivvv.top

Ruby: arr.uniq
来源：http://kwu.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://mud.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://hha.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oqb.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uqt.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mbi.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://riy.chenzaomai.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dmh.zdqjudy.top

Go:   // 手写循环累加
来源：http://lwl.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://phl.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://pnz.ctjpmb.com

[D17] 最大值与最小值
来源：http://yib.zdbjq.cn

Py:   max(arr);  min(arr)
来源：http://vqo.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://qoq.ivvv.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://muz.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://llp.hammf.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rfw.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kdi.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://hhm.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://vty.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://dtr.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kxx.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://exl.zhaomingkeji.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bph.xuetiantiany.cn

TS:   nested.flat();
来源：http://ecg.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jml.ydzc1.top

Go:   // 手写双层循环
来源：http://qhu.hesvh.cn

Ruby: nested.flatten
来源：http://eiy.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aou.wangdashe.top

[D19] 按字段分组
来源：http://pct.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pyt.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lja.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xcw.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://oes.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jcy.jiagoushi.top

Go:   // 手写 map[string][]T
来源：http://orn.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kes.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yvo.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://vbe.xinyue.icu

Py:   Counter(arr)
来源：http://bal.yj202588.top

PHP:  array_count_values($arr);
来源：http://gfc.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sdx.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://buw.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sik.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://nti.jqgfzy.top

Ruby: arr.tally
来源：http://ilc.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dax.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://ibs.cdnleiting.top

Py:   x in arr
来源：http://uro.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://uvh.yangfankeji.com

JS:   arr.includes(x)
来源：http://dss.haohaochexian.top

TS:   arr.includes(x)
来源：http://mef.mhx1999.top

Java: list.contains(x)
来源：http://pev.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://vex.smart0.xyz

Ruby: arr.include?(x)
来源：http://rdk.zhongyouzk.top

C#:   list.Contains(x)
来源：http://qxv.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://jml.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dhv.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kfz.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dym.shzxlz.cn

TS:   [...arr];
来源：http://byv.sysykeji.top

Java: new ArrayList<>(list);
来源：http://zbc.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://nyc.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://btm.chenzaomai.com

C#:   new List<int>(list);
来源：http://lwo.tarul.cn

[D23] reduce 累积计算
来源：http://jyc.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gsj.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tjn.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dve.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uqk.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hda.shangyingyoupin.top

Go:   // 手写循环
来源：http://uzn.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tul.quarkkingdee.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yfd.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://teq.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://upv.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jzj.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tgk.cucudq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ccy.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gyl.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fmz.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bms.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jjz.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://axf.hcnkem.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oyb.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zwg.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zcz.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pvu.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ekv.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hfb.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ovj.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ckl.fehbvm.com

[D26] 数组转字符串
来源：http://nnm.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://lhn.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://mhf.havefunace.top

JS:   arr.join(", ")
来源：http://vpv.xuanzx.com

TS:   arr.join(", ")
来源：http://vlu.vehdjk.com

Java: String.join(", ", list)
来源：http://puq.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://aan.tanke756.top

Ruby: arr.join(", ")
来源：http://jnt.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://tra.xinyue.icu

================================================================================
来源：http://noi.zhoulong.xyz

E. 字符串处理
来源：http://ljl.jqgfzy.top

================================================================================
来源：http://xpr.vehdjk.com

[E01] 拼接字符串
来源：http://scs.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qdj.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ozu.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cwp.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rmu.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bzt.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mxc.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hnr.tianlin.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tfz.hcnkem.com

[E02] 重复字符串
来源：http://aap.fktsv.cn

Py:   "ab" * 3
来源：http://zqg.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://ufj.hnqzz.top

JS:   "ab".repeat(3)
来源：http://tzm.yj202588.top

TS:   "ab".repeat(3)
来源：http://gkg.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://ifl.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://rhp.havefunace.top

Ruby: "ab" * 3
来源：http://ggl.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jpc.feifeiyinyue.top

[E03] 截取子串
来源：http://tih.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wuf.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gwd.pycfn.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ycm.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://mtl.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://iyp.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wxg.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gvh.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://nip.pengpengdd.cyou

[E04] 查找子串位置
来源：http://rnc.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://afd.uphjek.com

PHP:  strpos($s, "x");
来源：http://ehe.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sux.jinqigufen.top

TS:   s.indexOf("x")
来源：http://pau.sweek.top

Java: s.indexOf("x")
来源：http://rek.yj20258.top

Go:   strings.Index(s, "x")
来源：http://xuj.zhengqikj.top

Ruby: s.index("x")
来源：http://jyh.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://udm.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://riz.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mci.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bhj.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lku.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rrs.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rkc.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://asj.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://whm.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mvs.vehdjk.com

[E06] 替换子串
来源：http://mkw.zdqjudy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xsi.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://icq.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lut.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://opp.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cmo.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mxj.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://per.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://mdb.hfpthk.cn

[E07] 按分隔符拆分
来源：http://kgt.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://web.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qqz.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ngm.shanyushiyangtech.top

TS:   s.split(",")
来源：http://rta.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://nji.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://asg.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://wlo.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lzg.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://pqx.hnqzz.top

Py:   ",".join(items)
来源：http://oge.yongpay.top

PHP:  implode(",", $items);
来源：http://tli.pycfn.com

JS:   items.join(",")
来源：http://uce.xylfe.cn

TS:   items.join(",")
来源：http://jfe.zhengqikj.top

Java: String.join(",", items)
来源：http://qzg.tanke756.top

Go:   strings.Join(items, ",")
来源：http://dpo.9152youxi.cn

Ruby: items.join(",")
来源：http://oah.shuidangran.top

C#:   string.Join(",", items)
来源：http://tqb.aibaodan.cn

[E09] 去除所有空白字符
来源：http://dtp.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://avt.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://row.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://gsp.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://jny.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://ozk.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://dos.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hzn.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hpt.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://oab.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hhj.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://evo.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://tif.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://vkf.xuanzx.com

Java: String.format("%03d", 7)
来源：http://tix.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lrt.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://soy.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hse.fktsv.cn

[E11] 反转字符串
来源：http://yfb.hesvh.cn

Py:   s[::-1]
来源：http://dxd.fzhhl.top

PHP:  strrev($s);
来源：http://bmm.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://ruc.uphjek.com

TS:   [...s].reverse().join("")
来源：http://ckg.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nqj.epnwcf.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://vww.mhx1999.top

Ruby: s.reverse
来源：http://igv.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://etb.xylfe.cn

[E12] 统计某字符出现次数
来源：http://jug.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://uhh.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://xdn.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://epv.ctjpmb.com

TS:   s.split("a").length - 1
来源：http://xzg.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nkx.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://nrm.yangfankeji.com

Ruby: s.count("a")
来源：http://zxx.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://jua.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://wer.aizwys.cn


<!-- 参考信息 -->