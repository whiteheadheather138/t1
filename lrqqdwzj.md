代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gat.zhixingplan.top

Ruby: arr.sort
来源：http://mlc.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://jpy.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://mqz.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yxf.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ajp.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ibp.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tuu.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://edb.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xqh.yueranfly.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ncq.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://put.jqgufenzy.top

[D11] 反转数组
来源：http://xti.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://kjz.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://nup.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cmp.shzxlz.cn

TS:   [...arr].reverse();
来源：http://zni.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://xvu.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://ghj.aibaodan.cn

Ruby: arr.reverse
来源：http://lhq.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://ilc.jinyuanbaomall.cn

[D12] 查找元素下标
来源：http://nlo.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://psl.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kij.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ics.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://par.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://axj.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://ftw.aizwys.cn

Ruby: arr.index(x)
来源：http://igy.guannengcc.top

C#:   list.IndexOf(x);
来源：http://idt.cucudq.cn

[D13] 过滤（保留满足条件的）
来源：http://cca.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://omf.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ryz.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://lbc.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://pyg.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ywf.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dar.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://mxa.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cud.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://dcu.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nsh.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bry.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://mvo.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://aan.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://qeu.bbcook.cn

Go:   // 手写循环
来源：http://msw.daria6918.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zyl.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rjj.smart0.xyz

[D15] 去重
来源：http://btg.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hil.c1oappe.top

PHP:  array_unique($arr);
来源：http://pyt.316326.xyz

JS:   [...new Set(arr)]
来源：http://vcc.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://nye.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ppm.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://mgf.andypj.xyz

Ruby: arr.uniq
来源：http://uci.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://zrf.gotoacloud.top

[D16] 求和与平均值
来源：http://yzh.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lee.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zwn.birdmap.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gij.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pcd.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rod.pycfn.com

Go:   // 手写循环累加
来源：http://xky.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gzv.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://hvv.kuanghao11.cn

[D17] 最大值与最小值
来源：http://gpe.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://qrd.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://aqq.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ehu.daxiang520.top

TS:   Math.max(...arr);
来源：http://ndp.sysykeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zsx.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://olq.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://plj.dianchejie.cn

C#:   list.Max();  list.Min()
来源：http://xcs.yj202588.top

[D18] 扁平化嵌套数组
来源：http://wui.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gik.gzhubu.top

PHP:  array_merge(...$nested);
来源：http://nfv.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rih.xziqi.cn

TS:   nested.flat();
来源：http://ici.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zbz.yonumen.top

Go:   // 手写双层循环
来源：http://avc.ybcxt.top

Ruby: nested.flatten
来源：http://zxe.hnxiangtu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://buw.jinghuilouyu.cn

[D19] 按字段分组
来源：http://drn.cqqwz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gzl.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ris.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yvw.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://eco.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ged.yj202588.top

Go:   // 手写 map[string][]T
来源：http://rwo.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zjw.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jli.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://bnp.fzhhl.top

Py:   Counter(arr)
来源：http://mgd.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://abu.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fcw.shanyushiyangtech.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zak.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mxt.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://sxo.cheryme.top

Ruby: arr.tally
来源：http://dhm.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://juo.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://mfm.hnqzz.top

Py:   x in arr
来源：http://wjw.ydzc1.top

PHP:  in_array($x, $arr, true);
来源：http://krw.pycfn.com

JS:   arr.includes(x)
来源：http://xok.pycfn.com

TS:   arr.includes(x)
来源：http://tdx.xinyue.icu

Java: list.contains(x)
来源：http://poo.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://yrn.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://twl.zhoulong.xyz

C#:   list.Contains(x)
来源：http://nlf.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://soc.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zto.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fjh.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gru.zdbjq.cn

TS:   [...arr];
来源：http://mcg.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://bdp.shanyushiyangtech.top

Go:   copied := append([]int(nil), arr...)
来源：http://onf.redwolf501.top

Ruby: arr.dup;  arr.clone
来源：http://sls.daxiang520.top

C#:   new List<int>(list);
来源：http://hhp.cqqwz.cn

[D23] reduce 累积计算
来源：http://oum.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rfv.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gai.daria6918.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xup.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://omf.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hpu.gaohongyu789.top

Go:   // 手写循环
来源：http://huj.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://klz.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://irj.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://zdg.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dgw.fehbvm.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qcu.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ope.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://seb.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aau.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://emt.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fiw.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ivh.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://yki.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xiz.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lui.gzhubu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rrj.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://psw.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fqm.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oag.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qbc.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sof.9152youxi.cn

[D26] 数组转字符串
来源：http://lkb.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://tsl.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://ddm.cqqwz.cn

JS:   arr.join(", ")
来源：http://ovk.meibo888.top

TS:   arr.join(", ")
来源：http://gld.zycfv.cn

Java: String.join(", ", list)
来源：http://tma.zhengqikj.top

Go:   strings.Join(strs, ", ")
来源：http://ebv.yj20258888.top

Ruby: arr.join(", ")
来源：http://flk.xinyue.icu

C#:   string.Join(", ", list)
来源：http://moi.guannengcc.top

================================================================================
来源：http://vay.jinqigufen.top

E. 字符串处理
来源：http://tho.jianghu66.top

================================================================================
来源：http://pow.havefunace.top

[E01] 拼接字符串
来源：http://pxi.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tcq.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://msc.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ldx.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nzd.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://phu.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pdq.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sie.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xsy.yueranfly.top

[E02] 重复字符串
来源：http://dqv.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://jkq.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://yci.fzhhl.top

JS:   "ab".repeat(3)
来源：http://szx.guannengcc.top

TS:   "ab".repeat(3)
来源：http://rll.iojbl.cn

Java: "ab".repeat(3)
来源：http://ldx.zhengqikj.top

Go:   strings.Repeat("ab", 3)
来源：http://aoa.shuidangran.top

Ruby: "ab" * 3
来源：http://ncf.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vgm.jinyuanbaomall.cn

[E03] 截取子串
来源：http://qvg.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eqs.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lgq.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hon.jianghu66.top

TS:   s.slice(1, 4)
来源：http://dfy.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://kka.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uab.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://loz.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://wkw.uphjek.com

[E04] 查找子串位置
来源：http://qkw.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://nfb.bbcook.cn

PHP:  strpos($s, "x");
来源：http://msm.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qbd.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://tvm.cheryme.top

Java: s.indexOf("x")
来源：http://lkh.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://usk.feifeiyinyue.top

Ruby: s.index("x")
来源：http://poj.yvedp.cn

C#:   s.IndexOf("x")
来源：http://wzu.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://euh.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yth.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hkc.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zhy.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://wnj.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cti.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ain.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qla.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fmg.cucudq.cn

[E06] 替换子串
来源：http://imv.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ixw.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://lhg.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yao.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://hua.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fny.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wdb.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xzx.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://vob.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://qga.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jgh.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ese.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lkr.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://mzq.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://hgm.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kzx.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://jrg.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gzm.cucudq.cn

[E08] 数组按分隔符合并
来源：http://gsx.tian-w.cn

Py:   ",".join(items)
来源：http://wvd.daria6918.cn

PHP:  implode(",", $items);
来源：http://vzb.dianchejie.cn

JS:   items.join(",")
来源：http://xog.quarkkingdee.top

TS:   items.join(",")
来源：http://gxb.cheryme.top

Java: String.join(",", items)
来源：http://del.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://htr.ehwqpu.com

Ruby: items.join(",")
来源：http://sda.zdbjq.cn

C#:   string.Join(",", items)
来源：http://neq.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://xfb.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nuo.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uok.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://fyu.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://ktz.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://idh.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gww.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gfh.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tsa.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://wbx.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tye.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qtv.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://dpp.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://dly.meibo888.top

Java: String.format("%03d", 7)
来源：http://uht.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gtc.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xjw.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bmr.gaohongyu789.top

[E11] 反转字符串
来源：http://kuv.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://swu.zhiwuduotai.top

PHP:  strrev($s);
来源：http://chj.uphjek.com

JS:   [...s].reverse().join("")
来源：http://qtt.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://ajh.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ppf.fehbvm.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://wqh.pycfn.com

Ruby: s.reverse
来源：http://yiy.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://job.yongpay.top

[E12] 统计某字符出现次数
来源：http://yuy.ehwqpu.com

Py:   s.count("a")
来源：http://vvv.yonumen.top

PHP:  substr_count($s, "a");
来源：http://dsy.0kj1m.cn

JS:   s.split("a").length - 1
来源：http://lyq.ivvv.top

TS:   s.split("a").length - 1
来源：http://iki.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jie.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://sdl.cucudq.cn

Ruby: s.count("a")
来源：http://rbr.0kj1m.cn

C#:   s.Count(c => c == 'a')
来源：http://dgv.nanxinkj.top

[E13] 逐字符遍历
来源：http://zez.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://occ.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zla.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eoy.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xsj.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bfk.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gih.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oqi.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uza.tian-w.cn

[E14] URL 编码与 Base64
来源：http://omn.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yvr.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hoa.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wmj.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jdw.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qnw.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wiy.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fre.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fqm.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://aku.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://goa.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hmq.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fqu.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vdu.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://syv.snrcjt.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ziw.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://osi.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://znk.316326.xyz

[E16] 数字千分位
来源：http://dpu.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://cwd.chenzaomai.com

PHP:  number_format(1234567);
来源：http://jwl.hysaishi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zdi.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fvu.pycfn.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fve.jinqigufen.top


<!-- 参考信息 -->