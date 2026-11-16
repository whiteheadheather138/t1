代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fzz.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://owh.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bus.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xpb.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mdi.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wzq.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xtl.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://shl.yanxiufei.cn

[D11] 反转数组
来源：http://fak.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://dkb.nanxuanxn.top

PHP:  array_reverse($arr);
来源：http://dyi.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ebb.ppjwa.cn

TS:   [...arr].reverse();
来源：http://pfg.cqqwz.cn

Java: Collections.reverse(list);
来源：http://rpg.meibo888.top

Go:   slices.Reverse(arr)
来源：http://zzi.hammf.cn

Ruby: arr.reverse
来源：http://wzo.hywenlv.cn

C#:   list.Reverse();
来源：http://fkv.tian-w.cn

[D12] 查找元素下标
来源：http://fib.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://kky.fktsv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kzx.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tjv.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mbx.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vms.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://zhb.jinghuilouyu.cn

Ruby: arr.index(x)
来源：http://ktu.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://wqy.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://nwk.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://laa.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cif.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://xwa.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://wak.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xlw.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zaw.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dfm.ybcxt.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gww.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://agf.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mpx.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lfz.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://sex.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://qxb.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mez.dianchejie.cn

Go:   // 手写循环
来源：http://prd.ctjpmb.com

Ruby: arr.map { |x| x * 2 }
来源：http://phk.jinghuilouyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wfs.chenjidiqi.icu

[D15] 去重
来源：http://nzq.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sct.hcnkem.com

PHP:  array_unique($arr);
来源：http://lik.kuanghao11.cn

JS:   [...new Set(arr)]
来源：http://rqv.hesvh.cn

TS:   [...new Set(arr)]
来源：http://vcj.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://org.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://sfw.wangshuangyany.cn

Ruby: arr.uniq
来源：http://qye.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://bdo.chenzaomai.com

[D16] 求和与平均值
来源：http://pvj.yueranfly.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://slk.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zxw.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://frf.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jsy.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nlk.xinyue.icu

Go:   // 手写循环累加
来源：http://qud.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lvg.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://xdl.fzhhl.top

[D17] 最大值与最小值
来源：http://lqt.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://lsk.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://rib.daria6918.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ldq.tarul.cn

TS:   Math.max(...arr);
来源：http://wsm.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rqi.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ylu.pycfn.com

Ruby: arr.max;  arr.min
来源：http://tah.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://ocv.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://awy.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fym.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://wkp.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qss.ivvv.top

TS:   nested.flat();
来源：http://ndh.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tzb.hywenlv.cn

Go:   // 手写双层循环
来源：http://isl.xziqi.cn

Ruby: nested.flatten
来源：http://fov.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://idf.jqgfzy.top

[D19] 按字段分组
来源：http://slk.dianchejie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gxy.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qym.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ejt.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://npc.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jju.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://dpu.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gvk.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cem.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://imh.bjfxy.top

Py:   Counter(arr)
来源：http://ebg.xuanzx.com

PHP:  array_count_values($arr);
来源：http://ate.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jza.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://feb.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://doy.jianghu66.top

Go:   // 手写 map[T]int
来源：http://lgs.pycfn.com

Ruby: arr.tally
来源：http://kak.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hco.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://xjz.ehwqpu.com

Py:   x in arr
来源：http://fxe.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://msl.gogol.net.cn

JS:   arr.includes(x)
来源：http://oqk.jyoumei.cn

TS:   arr.includes(x)
来源：http://cre.zhongyouzk.top

Java: list.contains(x)
来源：http://njs.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://ano.yuxming.cn

Ruby: arr.include?(x)
来源：http://hub.vqdsnc.cn

C#:   list.Contains(x)
来源：http://esf.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://ckw.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://shv.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://efe.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mdi.yanxiufei.cn

TS:   [...arr];
来源：http://sls.cheryme.top

Java: new ArrayList<>(list);
来源：http://amh.mhx1999.top

Go:   copied := append([]int(nil), arr...)
来源：http://rul.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://pui.quarkkingdee.top

C#:   new List<int>(list);
来源：http://mbu.redwolf501.top

[D23] reduce 累积计算
来源：http://pgz.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yuo.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ojv.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bah.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jgv.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dfv.pycfn.com

Go:   // 手写循环
来源：http://aqu.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ztb.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jqs.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://fmh.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zhm.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://owc.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ipx.fehbvm.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ifm.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rff.aizwys.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sag.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cwr.dashuyun.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xfi.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://fsl.shanyushiyangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yvk.xuetiantiany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jeq.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zne.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mop.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mlt.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ntw.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wuc.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gpe.cqqwz.cn

[D26] 数组转字符串
来源：http://dql.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://qpc.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://mgw.daxiang520.top

JS:   arr.join(", ")
来源：http://uey.svipenyu.cn

TS:   arr.join(", ")
来源：http://dat.fehbvm.com

Java: String.join(", ", list)
来源：http://lxp.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://fvi.tian-w.cn

Ruby: arr.join(", ")
来源：http://hij.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://ugi.ydzc1.top

================================================================================
来源：http://xqa.jqgfzy.top

E. 字符串处理
来源：http://rtu.vehdjk.com

================================================================================
来源：http://czx.hongshengwenyu.top

[E01] 拼接字符串
来源：http://fus.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gki.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ouv.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iuw.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uwy.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pap.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pfz.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tty.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://txs.zhoulong.xyz

[E02] 重复字符串
来源：http://isc.wangdashe.top

Py:   "ab" * 3
来源：http://qts.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://mgt.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://xqg.sweek.top

TS:   "ab".repeat(3)
来源：http://esc.9152youxi.cn

Java: "ab".repeat(3)
来源：http://zwt.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://qom.bjfxy.top

Ruby: "ab" * 3
来源：http://njl.zhiwuduotai.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nje.jinghuilouyu.cn

[E03] 截取子串
来源：http://wrd.chenjidiqi.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ndy.bbcook.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nge.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lxg.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://ufz.jqgfzy.top

Java: s.substring(1, 4)
来源：http://tyo.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qhs.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ade.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://ais.daxiang520.top

[E04] 查找子串位置
来源：http://smj.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://yiq.cashguo.top

PHP:  strpos($s, "x");
来源：http://hen.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vjs.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://mhp.jinqigfzy.top

Java: s.indexOf("x")
来源：http://qyn.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://kxy.uphjek.com

Ruby: s.index("x")
来源：http://gez.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://xoj.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://hfz.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ooy.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eap.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qhb.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fks.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ddl.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ruj.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pqb.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xww.pycfn.com

[E06] 替换子串
来源：http://ikc.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wyr.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://edc.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iak.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://bri.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ank.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rrk.gzhubu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sir.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://nxv.uphjek.com

[E07] 按分隔符拆分
来源：http://kjf.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vux.shangyingyoupin.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dqw.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://waa.zhoulong.xyz

TS:   s.split(",")
来源：http://axf.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://vyr.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dpb.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://hft.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dbo.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://fdk.xinyue.icu

Py:   ",".join(items)
来源：http://icf.zhiwuduotai.top

PHP:  implode(",", $items);
来源：http://kwy.xuanzx.com

JS:   items.join(",")
来源：http://tyx.dianchejie.cn

TS:   items.join(",")
来源：http://vju.fzhhl.top

Java: String.join(",", items)
来源：http://qwx.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://nmf.gzhubu.top

Ruby: items.join(",")
来源：http://wau.fehbvm.com

C#:   string.Join(",", items)
来源：http://oxx.cashguo.top

[E09] 去除所有空白字符
来源：http://nvw.hnqzz.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://auk.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wmu.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://paz.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://iut.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://jgf.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jjj.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bhe.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rjz.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://cqj.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nhv.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://omi.cucudq.cn

JS:   "7".padStart(3, "0")
来源：http://wde.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://wgd.sxryk.cn

Java: String.format("%03d", 7)
来源：http://ikl.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zqz.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zsm.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qkz.jianghu66.top

[E11] 反转字符串
来源：http://kwq.hcnkem.com

Py:   s[::-1]
来源：http://dgk.shzxlz.cn

PHP:  strrev($s);
来源：http://qyj.shanyushiyangkeji.top

JS:   [...s].reverse().join("")
来源：http://htl.yj20258.top

TS:   [...s].reverse().join("")
来源：http://you.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xiq.shuidangran.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jfy.smart0.xyz

Ruby: s.reverse
来源：http://aiy.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wuk.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://gms.fktsv.cn

Py:   s.count("a")
来源：http://tsj.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://baj.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://wxn.birdmap.top

TS:   s.split("a").length - 1
来源：http://wjw.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qqi.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://vgt.yangfankeji.com

Ruby: s.count("a")
来源：http://hil.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://fmo.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://eas.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://pfx.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://laj.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jgd.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://skw.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uiv.yanxiufei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qfv.meibo888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://khm.tianlin.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zix.bbcook.cn

[E14] URL 编码与 Base64
来源：http://aou.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lar.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sga.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dxd.bjfxy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vyl.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qhn.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://umn.ppjwa.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tkp.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://awh.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://vvt.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nbo.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ijs.xinyue.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://svm.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xok.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yvy.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xch.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vtt.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://min.epnwcf.com

[E16] 数字千分位
来源：http://htu.gzhubu.top

Py:   f"{1234567:,}"
来源：http://ktt.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://ygc.xingfuxueyuan.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://igc.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wxr.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ebq.yuanzhike.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iks.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gak.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://ghu.316326.xyz

[E17] 首字母大写
来源：http://yuh.smart0.xyz


<!-- 参考信息 -->