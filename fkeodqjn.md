代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hxx.jqgfzy.top

Ruby: arr.sort
来源：http://clj.cdnleiting.top

C#:   list.Sort();
来源：http://yjk.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tso.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://stp.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wdv.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uyc.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tfs.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://efp.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qcy.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nqm.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ama.316326.xyz

[D11] 反转数组
来源：http://dal.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://okx.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://zah.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fsf.sweek.top

TS:   [...arr].reverse();
来源：http://lxs.epnwcf.com

Java: Collections.reverse(list);
来源：http://yie.cashguo.top

Go:   slices.Reverse(arr)
来源：http://opv.jqgfzy.top

Ruby: arr.reverse
来源：http://jkb.daria6918.cn

C#:   list.Reverse();
来源：http://bmt.zhaomingkeji.xyz

[D12] 查找元素下标
来源：http://piw.uphjek.com

Py:   arr.index(x);  x in arr
来源：http://mma.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oly.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hiu.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kin.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jrz.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://flu.hywenlv.cn

Ruby: arr.index(x)
来源：http://vmy.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://kbj.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://eje.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://glh.xuanzx.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://idp.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://zmt.yonumen.top

TS:   arr.filter(x => x > 3)
来源：http://qcr.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ilm.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wgy.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://izc.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ahj.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://ryh.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hwv.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://epf.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://xiq.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://lus.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pqh.aizwys.cn

Go:   // 手写循环
来源：http://nyl.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://dka.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ucs.chenlongwang.top

[D15] 去重
来源：http://dkg.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://txb.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://mya.yueranfly.top

JS:   [...new Set(arr)]
来源：http://nph.zycfv.cn

TS:   [...new Set(arr)]
来源：http://irt.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gbc.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://thp.quarkkingdee.top

Ruby: arr.uniq
来源：http://yfa.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://lkq.yangfankeji.com

[D16] 求和与平均值
来源：http://biq.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jwe.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gmf.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ubq.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ddr.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kpo.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://fgf.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wmg.ybcxt.top

C#:   list.Sum();  list.Average()
来源：http://cnb.havefunace.top

[D17] 最大值与最小值
来源：http://qrg.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://kyb.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://hnb.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wta.ydzc1.top

TS:   Math.max(...arr);
来源：http://gxy.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ufb.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wfe.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://tgc.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://uot.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://oad.havefunace.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tyz.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://gft.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wez.quarkkingdee.top

TS:   nested.flat();
来源：http://ums.yuxming.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mrv.shzxlz.cn

Go:   // 手写双层循环
来源：http://gjl.316326.xyz

Ruby: nested.flatten
来源：http://bya.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nfr.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://rtq.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pvm.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vce.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hyx.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xki.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fxj.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://dcj.cdnleiting.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mrr.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zyn.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://qju.yueranfly.top

Py:   Counter(arr)
来源：http://awa.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://eyk.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tru.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxb.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://com.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://dmf.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://zux.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hnz.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://rxz.cqqwz.cn

Py:   x in arr
来源：http://xbo.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://uth.hesvh.cn

JS:   arr.includes(x)
来源：http://klw.hnqzz.top

TS:   arr.includes(x)
来源：http://gjw.epnwcf.com

Java: list.contains(x)
来源：http://pvz.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://ddu.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://wlp.tarul.cn

C#:   list.Contains(x)
来源：http://kpt.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://yhv.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bmp.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qpy.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gkn.sxryk.cn

TS:   [...arr];
来源：http://uug.52xcode.cn

Java: new ArrayList<>(list);
来源：http://das.nanxuanxn.top

Go:   copied := append([]int(nil), arr...)
来源：http://sir.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://daz.hywenlv.cn

C#:   new List<int>(list);
来源：http://zir.zdbjq.cn

[D23] reduce 累积计算
来源：http://pad.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tgo.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oov.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ybh.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ufk.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pet.zhijiandao.cn

Go:   // 手写循环
来源：http://eej.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lhx.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rki.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://etn.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lyu.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xzr.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cbl.cqqwz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://evb.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tzh.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tcj.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ebe.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ham.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://rog.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mri.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oqk.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mob.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kyp.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zuw.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cap.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uwj.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hio.yonumen.top

[D26] 数组转字符串
来源：http://anq.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://pzn.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://ylc.meibo888.top

JS:   arr.join(", ")
来源：http://qmp.sufxvd.cn

TS:   arr.join(", ")
来源：http://wbb.chenzaomai.com

Java: String.join(", ", list)
来源：http://yvb.jqgufenzy.top

Go:   strings.Join(strs, ", ")
来源：http://kdl.gogol.net.cn

Ruby: arr.join(", ")
来源：http://pnu.yonumen.top

C#:   string.Join(", ", list)
来源：http://tgo.havefunace.top

================================================================================
来源：http://wxz.hysaishi.cn

E. 字符串处理
来源：http://nfd.0kj1m.cn

================================================================================
来源：http://wxd.9152youxi.cn

[E01] 拼接字符串
来源：http://fkz.tian-w.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vlp.vehdjk.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://scc.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lbi.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ycj.yueranfly.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lur.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://por.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bnz.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nhy.nwbrower.top

[E02] 重复字符串
来源：http://dqb.xylfe.cn

Py:   "ab" * 3
来源：http://yoc.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://kli.fktsv.cn

JS:   "ab".repeat(3)
来源：http://rno.mhx1999.top

TS:   "ab".repeat(3)
来源：http://ldw.yangfankeji.com

Java: "ab".repeat(3)
来源：http://mms.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://fho.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://zry.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://osx.ppjwa.cn

[E03] 截取子串
来源：http://hkk.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nkl.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rht.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jae.uphjek.com

TS:   s.slice(1, 4)
来源：http://ase.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://tja.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pjo.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://kmf.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://nxh.daxiang520.top

[E04] 查找子串位置
来源：http://xef.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://wxg.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://xkg.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dlc.guowangkeji.top

TS:   s.indexOf("x")
来源：http://vos.0kj1m.cn

Java: s.indexOf("x")
来源：http://nef.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://kos.hysaishi.cn

Ruby: s.index("x")
来源：http://gda.bbcook.cn

C#:   s.IndexOf("x")
来源：http://eel.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jiy.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qkg.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://taj.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mwu.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rdb.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jve.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ssv.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pkt.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hbv.yongpay.top

[E06] 替换子串
来源：http://yvp.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cbs.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://umu.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xgx.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://cxj.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qhr.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uyh.gzhubu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kvk.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://vsu.zhaomingkeji.xyz

[E07] 按分隔符拆分
来源：http://lga.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jha.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lpt.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://pol.ctjpmb.com

TS:   s.split(",")
来源：http://oxw.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pin.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rwf.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://jvo.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xow.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://ygq.ydjk.org.cn

Py:   ",".join(items)
来源：http://xry.daxiang520.top

PHP:  implode(",", $items);
来源：http://nvo.haohaochexian.top

JS:   items.join(",")
来源：http://xna.birdmap.top

TS:   items.join(",")
来源：http://zxy.svipenyu.cn

Java: String.join(",", items)
来源：http://zez.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://jkv.chenlongwang.top

Ruby: items.join(",")
来源：http://hqa.yangfankeji.com

C#:   string.Join(",", items)
来源：http://nmo.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://sdt.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qfu.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ify.yj202588.top

JS:   s.replace(/\s+/g, "")
来源：http://ezh.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://agt.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://ral.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gyg.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://byg.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ejz.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://kmo.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dqq.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://etq.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://hke.shzxlz.cn

TS:   "7".padStart(3, "0")
来源：http://obw.yfazqb.com

Java: String.format("%03d", 7)
来源：http://jkj.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://rov.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rxu.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vfc.zhixingplan.top

[E11] 反转字符串
来源：http://spl.kuanghao11.cn

Py:   s[::-1]
来源：http://pll.wangdashe.top

PHP:  strrev($s);
来源：http://ova.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://iui.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://hge.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uty.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nao.sufxvd.cn

Ruby: s.reverse
来源：http://uvs.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://tgq.jinqigufen.top

[E12] 统计某字符出现次数
来源：http://poe.vqdsnc.cn

Py:   s.count("a")
来源：http://tjx.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://cwg.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://njx.ydzc1.top

TS:   s.split("a").length - 1
来源：http://qzt.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lrt.iojbl.cn

Go:   strings.Count(s, "a")
来源：http://exw.birdmap.top

Ruby: s.count("a")
来源：http://cnx.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://mhf.tarul.cn

[E13] 逐字符遍历
来源：http://cjv.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://pzy.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cug.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qrb.yueranfly.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ryo.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://api.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nme.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://opz.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rni.cheryme.top

[E14] URL 编码与 Base64
来源：http://qgf.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kbg.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qfy.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ohw.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ady.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fya.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wug.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hau.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eok.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://mae.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rrv.guowangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sll.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ysd.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://szf.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zyu.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xvw.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wqw.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ukb.guowangkeji.top

[E16] 数字千分位
来源：http://deu.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://gev.cqqwz.cn

PHP:  number_format(1234567);
来源：http://zxm.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ewk.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pgc.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://apd.yongpay.top


<!-- 参考信息 -->