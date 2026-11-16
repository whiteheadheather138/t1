代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://joc.chenjidiqi.icu

Ruby: arr.sort
来源：http://ebf.316326.xyz

C#:   list.Sort();
来源：http://nek.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hsa.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eio.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://awn.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hom.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gzc.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://anm.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hmf.chenlongwang.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rzi.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kjl.52xcode.cn

[D11] 反转数组
来源：http://fbo.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://qmw.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://hfc.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gbg.mhx1999.top

TS:   [...arr].reverse();
来源：http://yiw.chenlongwang.top

Java: Collections.reverse(list);
来源：http://qit.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://gsa.fzhhl.top

Ruby: arr.reverse
来源：http://azf.chenjidiqi.icu

C#:   list.Reverse();
来源：http://zpy.316326.xyz

[D12] 查找元素下标
来源：http://byh.sweek.top

Py:   arr.index(x);  x in arr
来源：http://zer.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://asr.nwbrower.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aor.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xnu.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://alk.cashguo.top

Go:   slices.Index(arr, x)
来源：http://tsu.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://olc.daria6918.cn

C#:   list.IndexOf(x);
来源：http://mqv.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://phk.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://alc.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wam.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://llo.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://olc.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dye.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nfl.cdnleiting.top

Ruby: arr.select { |x| x > 3 }
来源：http://zbl.uphjek.com

C#:   list.Where(x => x > 3).ToList()
来源：http://zsa.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://lhn.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nra.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xef.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://mtg.guowangkeji.top

TS:   arr.map(x => x * 2)
来源：http://ofm.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kaf.haohaochexian.top

Go:   // 手写循环
来源：http://fjr.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://cgy.shanyushiyangtech.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cdn.aibaodan.cn

[D15] 去重
来源：http://vym.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sat.gotoacloud.top

PHP:  array_unique($arr);
来源：http://fku.cucudq.cn

JS:   [...new Set(arr)]
来源：http://eag.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://djt.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tkt.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://bhe.sjlbkw.cn

Ruby: arr.uniq
来源：http://kzy.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://ypk.sweek.top

[D16] 求和与平均值
来源：http://ddb.yfazqb.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hgu.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ota.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://klw.tanke756.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ygp.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://adt.jinqigfzy.top

Go:   // 手写循环累加
来源：http://bgk.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mke.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://acs.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://xfv.xingfuxueyuan.xyz

Py:   max(arr);  min(arr)
来源：http://fkg.fehbvm.com

PHP:  max($arr);  min($arr);
来源：http://xbd.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zyb.pycfn.com

TS:   Math.max(...arr);
来源：http://wog.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xge.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://twe.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://ydw.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://scz.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://bco.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oxw.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://wam.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vxa.hysaishi.cn

TS:   nested.flat();
来源：http://bzd.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://osh.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://gtt.sjlbkw.cn

Ruby: nested.flatten
来源：http://dot.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wrj.yuanzhike.top

[D19] 按字段分组
来源：http://ymk.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kxq.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pjo.bbcook.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kng.snrcjt.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pfc.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fcv.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://xbu.fengsongda.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tod.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vsd.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://gtj.xuanzx.com

Py:   Counter(arr)
来源：http://lfi.vqdsnc.cn

PHP:  array_count_values($arr);
来源：http://pra.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wpt.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eue.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://plo.mhx1999.top

Go:   // 手写 map[T]int
来源：http://bcl.ybcxt.top

Ruby: arr.tally
来源：http://deo.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://loa.daria6918.cn

[D21] 判断是否包含某元素
来源：http://xwm.shuidangran.top

Py:   x in arr
来源：http://ywb.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://qxk.iojbl.cn

JS:   arr.includes(x)
来源：http://lre.ivvv.top

TS:   arr.includes(x)
来源：http://cez.sjlbkw.cn

Java: list.contains(x)
来源：http://vxa.jinyuanbaomall.cn

Go:   slices.Contains(arr, x)
来源：http://xkc.nwbrower.top

Ruby: arr.include?(x)
来源：http://kja.nwbrower.top

C#:   list.Contains(x)
来源：http://nce.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://pwg.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bue.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jah.jqgfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://chj.nanxuanxn.top

TS:   [...arr];
来源：http://tjl.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://qmz.zhoulong.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://sak.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://nhg.yonumen.top

C#:   new List<int>(list);
来源：http://myc.daxiang520.top

[D23] reduce 累积计算
来源：http://dzn.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ahv.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lqj.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jeo.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mcm.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eop.epnwcf.com

Go:   // 手写循环
来源：http://pmc.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pmk.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cmv.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://kwi.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nvc.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://csg.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qup.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cro.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oct.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rzs.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lzd.dashuyun.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wiu.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://ngx.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qqr.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://poz.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dft.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aqj.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hyi.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://upv.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eed.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jgn.daria6918.cn

[D26] 数组转字符串
来源：http://dea.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://zss.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://iag.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://pwj.quarkkingdee.top

TS:   arr.join(", ")
来源：http://rgr.fehbvm.com

Java: String.join(", ", list)
来源：http://hrf.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://zej.daxiang520.top

Ruby: arr.join(", ")
来源：http://ugt.aizwys.cn

C#:   string.Join(", ", list)
来源：http://ckb.chenjidiqi.icu

================================================================================
来源：http://mtz.andypj.xyz

E. 字符串处理
来源：http://wsy.zhixingplan.top

================================================================================
来源：http://qni.nwbrower.top

[E01] 拼接字符串
来源：http://qed.aizwys.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tdg.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ajr.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://smp.316326.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hte.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pdd.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ssb.zhixingplan.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sjr.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://flx.ybcxt.top

[E02] 重复字符串
来源：http://iqu.cashguo.top

Py:   "ab" * 3
来源：http://qua.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://nvv.hcnkem.com

JS:   "ab".repeat(3)
来源：http://wmr.52xcode.cn

TS:   "ab".repeat(3)
来源：http://gfh.pycfn.com

Java: "ab".repeat(3)
来源：http://ckk.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://stm.jianghu66.top

Ruby: "ab" * 3
来源：http://xos.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iol.chenjidiqi.icu

[E03] 截取子串
来源：http://mce.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lji.yvedp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://duh.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gnm.andypj.xyz

TS:   s.slice(1, 4)
来源：http://wpp.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://lpb.zhixingplan.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bub.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fvu.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://lts.quarkkingdee.top

[E04] 查找子串位置
来源：http://bec.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://lxv.xuanzx.com

PHP:  strpos($s, "x");
来源：http://nhd.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ohv.cdnleiting.top

TS:   s.indexOf("x")
来源：http://xhj.chenlongwang.top

Java: s.indexOf("x")
来源：http://qta.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://vgd.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://ybm.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://qmf.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://tlf.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bky.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://exk.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wze.yuanzhike.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mfl.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gkx.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wqp.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qdb.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://svx.tian-w.cn

[E06] 替换子串
来源：http://njp.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://muk.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://wms.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://znp.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://wyy.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uka.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kkd.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aen.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://pic.gzhubu.top

[E07] 按分隔符拆分
来源：http://mmc.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ugw.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kwx.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ouz.yj20258.top

TS:   s.split(",")
来源：http://obz.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://idn.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wys.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://guy.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mnl.yuxming.cn

[E08] 数组按分隔符合并
来源：http://cvu.cucudq.cn

Py:   ",".join(items)
来源：http://jus.jqgfzy.top

PHP:  implode(",", $items);
来源：http://sls.feifeiyinyue.top

JS:   items.join(",")
来源：http://fuy.gzhubu.top

TS:   items.join(",")
来源：http://lpq.yuanzhike.top

Java: String.join(",", items)
来源：http://agv.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://fao.cdnleiting.top

Ruby: items.join(",")
来源：http://ycu.tianlin.xyz

C#:   string.Join(",", items)
来源：http://uxg.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://ztp.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pyd.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wyb.meibo888.top

JS:   s.replace(/\s+/g, "")
来源：http://key.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://nnr.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://cbx.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://blk.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://ehw.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hgb.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://fwx.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vsp.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gqq.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://thp.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://tjj.jianghu66.top

Java: String.format("%03d", 7)
来源：http://fno.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://owf.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jbr.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ktw.chenzaomai.com

[E11] 反转字符串
来源：http://ioe.sxryk.cn

Py:   s[::-1]
来源：http://has.yfazqb.com

PHP:  strrev($s);
来源：http://yxb.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://svr.yonumen.top

TS:   [...s].reverse().join("")
来源：http://ixi.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://koi.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hym.jiagoushi.top

Ruby: s.reverse
来源：http://qlp.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://ike.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://uyq.ehwqpu.com

Py:   s.count("a")
来源：http://rey.meibo888.top

PHP:  substr_count($s, "a");
来源：http://hrd.fengsongda.top

JS:   s.split("a").length - 1
来源：http://qss.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://rxv.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aod.xuanzx.com

Go:   strings.Count(s, "a")
来源：http://gdd.fktsv.cn

Ruby: s.count("a")
来源：http://pbd.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://cvo.tarul.cn

[E13] 逐字符遍历
来源：http://dus.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://cqh.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://laa.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://est.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bhp.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sba.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pwl.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rzh.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nda.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://hfn.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dpd.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mso.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fvl.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://czd.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xov.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sfq.jqgufenzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xmy.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hre.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://ame.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vea.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jvk.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xgr.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dfv.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ifc.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://azk.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lrd.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tdf.xziqi.cn

[E16] 数字千分位
来源：http://soo.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://dlr.yonumen.top

PHP:  number_format(1234567);
来源：http://kpj.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ovg.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yne.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ebk.sufxvd.cn


<!-- 参考信息 -->