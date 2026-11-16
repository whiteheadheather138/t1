代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://nso.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://ymi.ybcxt.top

[D09] 排序（升序）
来源：http://oyp.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://lpt.cashguo.top

PHP:  sort($arr);
来源：http://rza.jinqigfzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://htv.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yrs.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://two.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rvf.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://alv.gotoacloud.top

C#:   list.Sort();
来源：http://uwb.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ifs.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://atn.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eyy.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jcy.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xja.zycfv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yez.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jnc.svipenyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://czf.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://koe.jinqigfzy.top

[D11] 反转数组
来源：http://pcm.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://zyp.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://ith.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ttm.xuanzx.com

TS:   [...arr].reverse();
来源：http://ini.xingfuxueyuan.xyz

Java: Collections.reverse(list);
来源：http://yti.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://acv.sufxvd.cn

Ruby: arr.reverse
来源：http://zro.jinghuilouyu.cn

C#:   list.Reverse();
来源：http://ibk.yuxming.cn

[D12] 查找元素下标
来源：http://piz.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://ahm.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ggi.daxiang520.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://quy.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cdg.hammf.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jfv.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://gec.jlsjyb.cn

Ruby: arr.index(x)
来源：http://yva.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://gcx.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://pap.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zju.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nif.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://gxq.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://ego.bjfxy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zoc.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kvr.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ldx.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://wbe.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://zcp.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cmg.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dpb.daria6918.cn

JS:   arr.map(x => x * 2)
来源：http://ozy.pycfn.com

TS:   arr.map(x => x * 2)
来源：http://ydh.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rez.xylfe.cn

Go:   // 手写循环
来源：http://llj.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://lku.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lqt.fanxiaobao.xyz

[D15] 去重
来源：http://tuv.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rqd.jinqigufen.top

PHP:  array_unique($arr);
来源：http://abe.jinyuanbaomall.cn

JS:   [...new Set(arr)]
来源：http://dgb.tanke756.top

TS:   [...new Set(arr)]
来源：http://viq.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bkz.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nlc.shuidangran.top

Ruby: arr.uniq
来源：http://cbo.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://ccg.mhx1999.top

[D16] 求和与平均值
来源：http://ofu.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zgz.cdnleiting.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://awd.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rtx.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ixo.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://owy.hfpthk.cn

Go:   // 手写循环累加
来源：http://kja.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pnj.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://xpx.nwbrower.top

[D17] 最大值与最小值
来源：http://ecz.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://lul.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://cxt.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mue.gogol.net.cn

TS:   Math.max(...arr);
来源：http://kme.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://qgp.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rmg.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://dsf.sweek.top

C#:   list.Max();  list.Min()
来源：http://pzf.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://hnn.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dft.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://zod.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yvk.hnqzz.top

TS:   nested.flat();
来源：http://suf.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qoh.andypj.xyz

Go:   // 手写双层循环
来源：http://qib.iojbl.cn

Ruby: nested.flatten
来源：http://zix.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wun.yj20258888.top

[D19] 按字段分组
来源：http://yet.ydzc1.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://odw.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jqf.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://knd.yvedp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oyc.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bst.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://qnf.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vqy.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zzf.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://fka.ehwqpu.com

Py:   Counter(arr)
来源：http://cho.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://bzd.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tvh.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xkt.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://six.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://yye.yj202588.top

Ruby: arr.tally
来源：http://qhg.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dvk.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://xks.pengpengdd.cyou

Py:   x in arr
来源：http://aww.feifeiyinyue.top

PHP:  in_array($x, $arr, true);
来源：http://iab.ctjpmb.com

JS:   arr.includes(x)
来源：http://hzb.vehdjk.com

TS:   arr.includes(x)
来源：http://vfl.jinqigufen.top

Java: list.contains(x)
来源：http://gcq.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://sci.bbcook.cn

Ruby: arr.include?(x)
来源：http://mnk.jiagoushi.top

C#:   list.Contains(x)
来源：http://xbz.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://zew.jinyuanbaomall.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wuv.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wzs.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cyx.hongshengwenyu.top

TS:   [...arr];
来源：http://lnz.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://sna.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tge.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://sbl.cucudq.cn

C#:   new List<int>(list);
来源：http://sfy.c1oappe.top

[D23] reduce 累积计算
来源：http://zbg.jqgufenzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jge.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://egk.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iqn.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://azw.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kdv.daxiang520.top

Go:   // 手写循环
来源：http://olv.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lzz.fzhhl.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qqa.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://pwf.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sop.nwbrower.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://isf.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://otz.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fue.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rwy.vqdsnc.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://owx.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nyb.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xzs.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://djv.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mmb.jyoumei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://whc.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uhs.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zue.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ryw.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hyq.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jbp.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://khc.bbcook.cn

[D26] 数组转字符串
来源：http://bst.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://qmj.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://ljk.uphjek.com

JS:   arr.join(", ")
来源：http://plz.uphjek.com

TS:   arr.join(", ")
来源：http://gca.nanxinkj.top

Java: String.join(", ", list)
来源：http://vlr.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://gwr.wangshuangyany.cn

Ruby: arr.join(", ")
来源：http://vbj.haohaochexian.top

C#:   string.Join(", ", list)
来源：http://hzy.sjlbkw.cn

================================================================================
来源：http://olm.ybcxt.top

E. 字符串处理
来源：http://hhx.dianchejie.cn

================================================================================
来源：http://ttm.quarkkingdee.top

[E01] 拼接字符串
来源：http://dzu.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://die.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ezb.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eby.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vyx.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xxo.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fqe.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://txj.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lrg.sysykeji.top

[E02] 重复字符串
来源：http://mhe.hcnkem.com

Py:   "ab" * 3
来源：http://sqs.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://ipj.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://rnf.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://vyp.tarul.cn

Java: "ab".repeat(3)
来源：http://hxh.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://bne.yvedp.cn

Ruby: "ab" * 3
来源：http://dvz.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zxh.yj20258888.top

[E03] 截取子串
来源：http://oix.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nuc.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dwu.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ilh.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://ngb.dashuyun.cn

Java: s.substring(1, 4)
来源：http://cak.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://goe.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fxz.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://men.quarkkingdee.top

[E04] 查找子串位置
来源：http://fta.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://clh.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://sai.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wiw.aizwys.cn

TS:   s.indexOf("x")
来源：http://zzs.xuetiantiany.cn

Java: s.indexOf("x")
来源：http://hwm.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://err.haohaochexian.top

Ruby: s.index("x")
来源：http://gai.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://pcm.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lll.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ywv.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hyo.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tez.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gzk.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://soe.ydjk.org.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pbv.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zzu.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ttm.cqqwz.cn

[E06] 替换子串
来源：http://ztg.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uke.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://qgl.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://neh.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://mxh.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mdo.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cyi.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://opi.yj20258.top

C#:   s.Replace("a", "b")
来源：http://mkw.yueranfly.top

[E07] 按分隔符拆分
来源：http://zos.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mtg.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lqk.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ueg.jlsjyb.cn

TS:   s.split(",")
来源：http://ypw.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ypi.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://scx.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://nkm.gotoacloud.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bah.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://uzz.fzhhl.top

Py:   ",".join(items)
来源：http://zka.yfazqb.com

PHP:  implode(",", $items);
来源：http://psr.chenjidiqi.icu

JS:   items.join(",")
来源：http://xvn.sxryk.cn

TS:   items.join(",")
来源：http://zmi.dianchejie.cn

Java: String.join(",", items)
来源：http://mib.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://qlr.sjlbkw.cn

Ruby: items.join(",")
来源：http://alr.aizwys.cn

C#:   string.Join(",", items)
来源：http://kfd.gzhubu.top

[E09] 去除所有空白字符
来源：http://hot.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xnr.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://edw.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://hub.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://gal.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://dfk.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fsy.kuanghao11.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xls.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sgt.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://gng.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rcn.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dwm.yuanzhike.top

JS:   "7".padStart(3, "0")
来源：http://awz.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://mne.havefunace.top

Java: String.format("%03d", 7)
来源：http://ypy.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ycc.zhijiandao.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xas.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sag.fktsv.cn

[E11] 反转字符串
来源：http://pei.dianchejie.cn

Py:   s[::-1]
来源：http://hdf.vqdsnc.cn

PHP:  strrev($s);
来源：http://lby.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://ted.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://pth.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ene.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tcg.yfazqb.com

Ruby: s.reverse
来源：http://ysq.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://req.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://eei.ydzc1.top

Py:   s.count("a")
来源：http://fon.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://agc.daria6918.cn

JS:   s.split("a").length - 1
来源：http://xsq.316326.xyz

TS:   s.split("a").length - 1
来源：http://wkx.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ujy.hammf.cn

Go:   strings.Count(s, "a")
来源：http://wvj.jinqigufen.top

Ruby: s.count("a")
来源：http://fyq.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://yxd.yuanzhike.top

[E13] 逐字符遍历
来源：http://tfg.yj20258.top

Py:   for ch in s: print(ch)
来源：http://jhn.nanxuanxn.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lhl.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://jml.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nfw.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vns.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vav.yfazqb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://xlt.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gyn.zdqjudy.top

[E14] URL 编码与 Base64
来源：http://ffj.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qnx.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zdi.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dez.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://civ.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://afu.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jzd.aizwys.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tgd.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qvh.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://ajq.fktsv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gya.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aqn.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qlo.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://bia.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://apb.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://moi.nanxinkj.top


<!-- 参考信息 -->