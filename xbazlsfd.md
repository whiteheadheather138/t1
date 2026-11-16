代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://inl.hfpthk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://flx.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gsx.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gqq.sxryk.cn

[D11] 反转数组
来源：http://szh.jinqigfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://wdy.yongpay.top

PHP:  array_reverse($arr);
来源：http://ctj.yj202588.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vbr.gzhubu.top

TS:   [...arr].reverse();
来源：http://qxg.iojbl.cn

Java: Collections.reverse(list);
来源：http://hbo.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://hht.nanxinkj.top

Ruby: arr.reverse
来源：http://iyu.zhijiandao.cn

C#:   list.Reverse();
来源：http://lkv.hongshengwenyu.top

[D12] 查找元素下标
来源：http://ljo.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://vim.dashuyun.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oqa.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://erv.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmb.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oeo.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://vyb.ctjpmb.com

Ruby: arr.index(x)
来源：http://pyg.birdmap.top

C#:   list.IndexOf(x);
来源：http://hoo.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://cep.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ugd.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ryz.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://aek.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://cxm.quarkkingdee.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ssa.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ldu.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://dkb.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://bnb.dianchejie.cn

[D14] 映射转换（每个元素变形）
来源：http://hqe.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xts.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://afk.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://gdz.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://ted.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wtm.nwbrower.top

Go:   // 手写循环
来源：http://xrg.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lpz.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zkd.epnwcf.com

[D15] 去重
来源：http://qod.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mck.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://mij.zhongyouzk.top

JS:   [...new Set(arr)]
来源：http://fqz.yj20258.top

TS:   [...new Set(arr)]
来源：http://xok.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rbk.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://usz.fehbvm.com

Ruby: arr.uniq
来源：http://lbl.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://vcb.aizwys.cn

[D16] 求和与平均值
来源：http://yla.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vqt.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kug.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mgw.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ozv.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yxs.zhoulong.xyz

Go:   // 手写循环累加
来源：http://nqf.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aap.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://dcy.shuidangran.top

[D17] 最大值与最小值
来源：http://uij.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://fqd.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://ttu.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ujp.redwolf501.top

TS:   Math.max(...arr);
来源：http://sui.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aiv.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pab.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://frz.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://ocq.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://dvj.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rhr.ehwqpu.com

PHP:  array_merge(...$nested);
来源：http://xit.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eqq.hnxiangtu.top

TS:   nested.flat();
来源：http://oet.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://epy.uphjek.com

Go:   // 手写双层循环
来源：http://eus.yongpay.top

Ruby: nested.flatten
来源：http://egp.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://thh.cqqwz.cn

[D19] 按字段分组
来源：http://ntl.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iup.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bdo.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cko.tianlin.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://nru.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://znz.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://ckh.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://zal.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xuw.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://rom.hnqzz.top

Py:   Counter(arr)
来源：http://iue.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://nlw.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nac.hfpthk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vaf.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kwp.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://cfv.zycfv.cn

Ruby: arr.tally
来源：http://lvl.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ocf.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://xua.tarul.cn

Py:   x in arr
来源：http://cce.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://ngb.ydzc1.top

JS:   arr.includes(x)
来源：http://wbo.smart0.xyz

TS:   arr.includes(x)
来源：http://ppc.fehbvm.com

Java: list.contains(x)
来源：http://hwn.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://gez.redwolf501.top

Ruby: arr.include?(x)
来源：http://dwg.tianlin.xyz

C#:   list.Contains(x)
来源：http://yec.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://uyk.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vrh.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://seu.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dua.svipenyu.cn

TS:   [...arr];
来源：http://njh.chenzaomai.com

Java: new ArrayList<>(list);
来源：http://qya.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://wfo.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://dcc.kuanghao11.cn

C#:   new List<int>(list);
来源：http://ved.fktsv.cn

[D23] reduce 累积计算
来源：http://psp.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wbm.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bwi.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cli.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oqn.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://swq.yvedp.cn

Go:   // 手写循环
来源：http://bxs.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tax.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sxi.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://vqv.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pns.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nkh.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ekk.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://chu.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mtj.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://thl.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hdo.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mdt.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://aex.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xtp.xuetiantiany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fgj.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zoc.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xqx.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hwi.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pwb.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://irv.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kuy.svipenyu.cn

[D26] 数组转字符串
来源：http://lcp.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://prk.meibo888.top

PHP:  implode(", ", $arr);
来源：http://kez.9152youxi.cn

JS:   arr.join(", ")
来源：http://nhs.cheryme.top

TS:   arr.join(", ")
来源：http://jjz.ehwqpu.com

Java: String.join(", ", list)
来源：http://fsz.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://idw.pycfn.com

Ruby: arr.join(", ")
来源：http://aak.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://dtz.jqgufenzy.top

================================================================================
来源：http://nlk.sjlbkw.cn

E. 字符串处理
来源：http://lwa.yanxiufei.cn

================================================================================
来源：http://pxp.xuetiantiany.cn

[E01] 拼接字符串
来源：http://egr.birdmap.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oaq.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zsd.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jal.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zbl.daxiang520.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mtl.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hvr.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sgn.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yvn.aibaodan.cn

[E02] 重复字符串
来源：http://kdd.pengpengdd.cyou

Py:   "ab" * 3
来源：http://vxc.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://znk.gzhubu.top

JS:   "ab".repeat(3)
来源：http://wjr.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://bks.jinqigufen.top

Java: "ab".repeat(3)
来源：http://nyp.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://aud.chenzaomai.com

Ruby: "ab" * 3
来源：http://juw.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gqh.hammf.cn

[E03] 截取子串
来源：http://jcd.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pil.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ekh.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cvr.birdmap.top

TS:   s.slice(1, 4)
来源：http://vmz.aizwys.cn

Java: s.substring(1, 4)
来源：http://daz.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iuh.sxryk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://scv.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://hkf.wangshuangyany.cn

[E04] 查找子串位置
来源：http://bjc.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://yib.vehdjk.com

PHP:  strpos($s, "x");
来源：http://euz.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://emq.nanxinkj.top

TS:   s.indexOf("x")
来源：http://xxk.nanxinkj.top

Java: s.indexOf("x")
来源：http://vsa.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://wrz.zdqjudy.top

Ruby: s.index("x")
来源：http://idc.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://dda.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hqf.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qdo.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lju.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iob.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dix.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vaw.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ylq.guannengcc.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ecn.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hnm.havefunace.top

[E06] 替换子串
来源：http://pwo.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zcz.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://fky.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://npg.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://uaj.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ldo.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xns.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://epg.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://aja.sysykeji.top

[E07] 按分隔符拆分
来源：http://mat.ybcxt.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eac.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dsd.shanyushiyangtech.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ksc.bjfxy.top

TS:   s.split(",")
来源：http://gqe.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://upb.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jyu.tanke756.top

Ruby: s.split(",");  s.split
来源：http://nud.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://khi.daria6918.cn

[E08] 数组按分隔符合并
来源：http://bfh.tian-w.cn

Py:   ",".join(items)
来源：http://gfe.hammf.cn

PHP:  implode(",", $items);
来源：http://uvl.chenjidiqi.icu

JS:   items.join(",")
来源：http://mee.yuanzhike.top

TS:   items.join(",")
来源：http://vie.dashuyun.cn

Java: String.join(",", items)
来源：http://ezl.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://exg.sjlbkw.cn

Ruby: items.join(",")
来源：http://yol.snrcjt.cn

C#:   string.Join(",", items)
来源：http://bfo.yanxiufei.cn

[E09] 去除所有空白字符
来源：http://uqj.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mhz.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rbc.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://apx.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://fnq.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://ucm.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jqm.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://gho.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nis.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://sjg.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lfl.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tki.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://etr.nanxinkj.top

TS:   "7".padStart(3, "0")
来源：http://tdd.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://nmn.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xim.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rvj.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dyu.0kj1m.cn

[E11] 反转字符串
来源：http://mju.jinqigufen.top

Py:   s[::-1]
来源：http://yxp.cucudq.cn

PHP:  strrev($s);
来源：http://isw.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://rtt.tanke756.top

TS:   [...s].reverse().join("")
来源：http://hdg.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://ogf.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eri.ybcxt.top

Ruby: s.reverse
来源：http://cym.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://rxp.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://sjo.yueranfly.top

Py:   s.count("a")
来源：http://sgn.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://bes.tanke756.top

JS:   s.split("a").length - 1
来源：http://fbd.xziqi.cn

TS:   s.split("a").length - 1
来源：http://odt.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jhm.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://hfy.epnwcf.com

Ruby: s.count("a")
来源：http://bsd.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://mhy.cdnleiting.top

[E13] 逐字符遍历
来源：http://agl.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://fvm.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://afh.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sqx.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://scl.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vjz.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ptp.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bzr.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dpj.hfpthk.cn

[E14] URL 编码与 Base64
来源：http://hvt.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kyg.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mxu.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fme.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eno.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zad.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eqp.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ykc.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nmg.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://axs.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ajp.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ptm.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iga.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://etd.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lht.sufxvd.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aji.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ccv.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ens.jiagoushi.top

[E16] 数字千分位
来源：http://gaj.fktsv.cn

Py:   f"{1234567:,}"
来源：http://yxg.gzhubu.top

PHP:  number_format(1234567);
来源：http://urn.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wtl.tanke756.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lpj.jyoumei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jyn.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dfo.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qbd.yj202588.top

C#:   1234567.ToString("N0")
来源：http://xzr.hfpthk.cn

[E17] 首字母大写
来源：http://vue.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ppm.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yff.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://szz.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wuj.zdbjq.cn


<!-- 参考信息 -->