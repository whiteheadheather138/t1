代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eer.wangshuangyany.cn

Ruby: arr.sort
来源：http://rjv.aibaodan.cn

C#:   list.Sort();
来源：http://qhy.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qww.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tgr.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://abk.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wjq.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vfa.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uos.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jgu.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tzy.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cyx.hysaishi.cn

[D11] 反转数组
来源：http://xpy.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bnf.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://gde.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xeg.jyoumei.cn

TS:   [...arr].reverse();
来源：http://wxr.ctjpmb.com

Java: Collections.reverse(list);
来源：http://opk.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://znj.cdnleiting.top

Ruby: arr.reverse
来源：http://yji.sweek.top

C#:   list.Reverse();
来源：http://ahn.hcnkem.com

[D12] 查找元素下标
来源：http://qvk.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://hyx.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sma.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gne.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zem.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ars.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://xua.tarul.cn

Ruby: arr.index(x)
来源：http://hma.52xcode.cn

C#:   list.IndexOf(x);
来源：http://ogg.tian-w.cn

[D13] 过滤（保留满足条件的）
来源：http://eow.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vnu.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pto.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://nhm.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://zif.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sni.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://laj.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tpe.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://imj.zhongyouzk.top

[D14] 映射转换（每个元素变形）
来源：http://yze.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hes.jyoumei.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xdi.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://lvd.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://dcf.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vti.hammf.cn

Go:   // 手写循环
来源：http://fqy.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://szj.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dti.sjlbkw.cn

[D15] 去重
来源：http://inb.sweek.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cbg.xinyue.icu

PHP:  array_unique($arr);
来源：http://itm.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://ehn.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://vci.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gvz.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://nii.jyoumei.cn

Ruby: arr.uniq
来源：http://net.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://txd.yvedp.cn

[D16] 求和与平均值
来源：http://wxq.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wkc.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wkx.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://byt.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsq.jinqigfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bea.wangshuangyany.cn

Go:   // 手写循环累加
来源：http://ald.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vax.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://lzr.c1oappe.top

[D17] 最大值与最小值
来源：http://adz.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://pcj.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://vgg.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzf.mhx1999.top

TS:   Math.max(...arr);
来源：http://yfu.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://pgi.bbcook.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ylf.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://pad.tanke756.top

C#:   list.Max();  list.Min()
来源：http://pjg.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://jan.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pww.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://mdn.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wry.ydjk.org.cn

TS:   nested.flat();
来源：http://bym.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://abv.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://eed.mhx1999.top

Ruby: nested.flatten
来源：http://ulj.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zki.ybcxt.top

[D19] 按字段分组
来源：http://yar.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hkm.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kuw.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vtj.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://jky.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ibp.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://anb.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bwe.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nyu.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://ikp.dianchejie.cn

Py:   Counter(arr)
来源：http://ipf.ydzc1.top

PHP:  array_count_values($arr);
来源：http://mxd.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ahz.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sen.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://can.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://bsc.cashguo.top

Ruby: arr.tally
来源：http://fbw.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pik.uphjek.com

[D21] 判断是否包含某元素
来源：http://iub.gaohongyu789.top

Py:   x in arr
来源：http://emh.yj202588.top

PHP:  in_array($x, $arr, true);
来源：http://ser.ivvv.top

JS:   arr.includes(x)
来源：http://byz.pycfn.com

TS:   arr.includes(x)
来源：http://crq.gaohongyu789.top

Java: list.contains(x)
来源：http://dct.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://csj.tarul.cn

Ruby: arr.include?(x)
来源：http://gko.fzhhl.top

C#:   list.Contains(x)
来源：http://jsg.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://exr.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vuv.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lwc.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://igj.sweek.top

TS:   [...arr];
来源：http://rkq.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://ozg.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cvz.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://yva.bjfxy.top

C#:   new List<int>(list);
来源：http://xbr.shuidangran.top

[D23] reduce 累积计算
来源：http://txn.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ctw.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bjg.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cdd.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qfz.yj202588.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mxv.shuidangran.top

Go:   // 手写循环
来源：http://ctb.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ure.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lje.kuanghao11.cn

[D24] 字典 / Map 基本操作
来源：http://rkr.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kqz.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zou.jyoumei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ivl.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bfy.gaohongyu789.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vpg.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oko.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dwa.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ahd.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://oee.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://opv.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aru.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://onz.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://roj.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kly.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lft.jlsjyb.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eli.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pqh.ydjk.org.cn

[D26] 数组转字符串
来源：http://tkl.meibo888.top

Py:   ", ".join(map(str, arr))
来源：http://ack.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://huf.fengsongda.top

JS:   arr.join(", ")
来源：http://djk.cheryme.top

TS:   arr.join(", ")
来源：http://msc.fzhhl.top

Java: String.join(", ", list)
来源：http://wvm.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://esx.zhixingplan.top

Ruby: arr.join(", ")
来源：http://zix.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://eaf.vqdsnc.cn

================================================================================
来源：http://bjf.hesvh.cn

E. 字符串处理
来源：http://xnt.tanke756.top

================================================================================
来源：http://gkx.zhongyouzk.top

[E01] 拼接字符串
来源：http://zme.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jqx.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hrm.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://odo.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmr.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://osb.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bzv.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qvo.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://agw.xuanzx.com

[E02] 重复字符串
来源：http://wgu.gotoacloud.top

Py:   "ab" * 3
来源：http://gon.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://how.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://oja.pycfn.com

TS:   "ab".repeat(3)
来源：http://nxc.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://trs.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://jgz.ivvv.top

Ruby: "ab" * 3
来源：http://zox.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://doc.zycfv.cn

[E03] 截取子串
来源：http://zop.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cnx.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ajj.c1oappe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kkq.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://dvn.iojbl.cn

Java: s.substring(1, 4)
来源：http://ugc.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ddi.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://mnx.hammf.cn

C#:   s.Substring(1, 3)
来源：http://sfn.chenzaomai.com

[E04] 查找子串位置
来源：http://uak.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://ojm.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://ucq.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ydh.aibaodan.cn

TS:   s.indexOf("x")
来源：http://hwj.ppjwa.cn

Java: s.indexOf("x")
来源：http://uva.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://ieg.vehdjk.com

Ruby: s.index("x")
来源：http://sdz.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://pdp.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iff.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eip.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ipb.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aln.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xxl.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ecb.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wvd.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iwk.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://usc.guannengcc.top

[E06] 替换子串
来源：http://bsp.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xjg.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://fvc.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xnm.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://has.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bmt.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ctp.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xvc.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://bzd.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://gfa.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mgz.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zls.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://crd.jqgufenzy.top

TS:   s.split(",")
来源：http://zgu.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://grv.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ciq.sweek.top

Ruby: s.split(",");  s.split
来源：http://iqd.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vlg.yj202588.top

[E08] 数组按分隔符合并
来源：http://tcd.xziqi.cn

Py:   ",".join(items)
来源：http://ojd.ivvv.top

PHP:  implode(",", $items);
来源：http://fug.cdnleiting.top

JS:   items.join(",")
来源：http://zbc.cucudq.cn

TS:   items.join(",")
来源：http://pml.cheryme.top

Java: String.join(",", items)
来源：http://ven.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://eqk.gogol.net.cn

Ruby: items.join(",")
来源：http://cgt.iojbl.cn

C#:   string.Join(",", items)
来源：http://are.guannengcc.top

[E09] 去除所有空白字符
来源：http://exn.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oqi.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bkf.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ofl.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://jfq.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://nza.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qfw.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://cnl.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fey.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://ate.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://axx.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cjw.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://smx.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://mkw.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://wvz.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cpj.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eal.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yvr.yangfankeji.com

[E11] 反转字符串
来源：http://mro.cashguo.top

Py:   s[::-1]
来源：http://ina.guannengcc.top

PHP:  strrev($s);
来源：http://ciq.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://jtd.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://otr.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://alp.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dbt.yonumen.top

Ruby: s.reverse
来源：http://caz.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uix.epnwcf.com

[E12] 统计某字符出现次数
来源：http://uwl.fehbvm.com

Py:   s.count("a")
来源：http://rdt.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://hwp.tanke756.top

JS:   s.split("a").length - 1
来源：http://msp.c1oappe.top

TS:   s.split("a").length - 1
来源：http://fir.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mnq.cheryme.top

Go:   strings.Count(s, "a")
来源：http://ypr.wangshuangyany.cn

Ruby: s.count("a")
来源：http://pas.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://inz.sysykeji.top

[E13] 逐字符遍历
来源：http://pru.yonumen.top

Py:   for ch in s: print(ch)
来源：http://hsx.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xlk.fanxiaobao.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://nei.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kib.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dvr.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ysi.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://tlc.chenzaomai.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uzq.pycfn.com

[E14] URL 编码与 Base64
来源：http://ogz.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sfi.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qhx.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://muw.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qru.ybcxt.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jnc.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ome.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://see.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kti.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://axg.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uek.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vxd.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://stw.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xtw.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wgc.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qtt.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://woc.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nlo.snrcjt.cn

[E16] 数字千分位
来源：http://jqr.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://ses.gogol.net.cn

PHP:  number_format(1234567);
来源：http://fhx.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dlz.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mzj.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dib.tarul.cn


<!-- 参考信息 -->