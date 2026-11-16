代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://nlq.yj20258888.top

[D08] 合并两个数组
来源：http://icu.xinyue.icu

Py:   a + b;  a.extend(b)
来源：http://yzr.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://ojn.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hmk.zhixingplan.top

TS:   [...a, ...b];
来源：http://qqu.shangyingyoupin.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://moa.nwbrower.top

Go:   append(a, b...)
来源：http://fdi.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://deg.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://erx.jinqigfzy.top

[D09] 排序（升序）
来源：http://erq.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://grg.hammf.cn

PHP:  sort($arr);
来源：http://sqg.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wbd.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zjt.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mzl.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fym.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://eoe.jinqigufen.top

C#:   list.Sort();
来源：http://jye.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vik.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xkl.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://caf.bjfxy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://two.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qjm.yj20258888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ymq.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ytf.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://obh.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zda.nanxuanxn.top

[D11] 反转数组
来源：http://upw.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jtj.sysykeji.top

PHP:  array_reverse($arr);
来源：http://okk.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wpg.yvedp.cn

TS:   [...arr].reverse();
来源：http://mkd.yfazqb.com

Java: Collections.reverse(list);
来源：http://adp.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://aus.316326.xyz

Ruby: arr.reverse
来源：http://kjr.fktsv.cn

C#:   list.Reverse();
来源：http://edt.zycfv.cn

[D12] 查找元素下标
来源：http://zip.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://ken.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jbe.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehe.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dxx.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bvn.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://epi.yj20258888.top

Ruby: arr.index(x)
来源：http://ldq.316326.xyz

C#:   list.IndexOf(x);
来源：http://xyv.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://suh.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wog.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jqh.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://nud.xuetiantiany.cn

TS:   arr.filter(x => x > 3)
来源：http://pio.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ict.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mjp.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rkg.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://wuy.gotoacloud.top

[D14] 映射转换（每个元素变形）
来源：http://yed.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gef.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ikn.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://zpk.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://yob.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tvb.daria6918.cn

Go:   // 手写循环
来源：http://tek.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dzo.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pou.hongshengwenyu.top

[D15] 去重
来源：http://cvy.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://woj.uphjek.com

PHP:  array_unique($arr);
来源：http://jpu.pycfn.com

JS:   [...new Set(arr)]
来源：http://emo.guannengcc.top

TS:   [...new Set(arr)]
来源：http://gdz.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iko.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://ifb.daria6918.cn

Ruby: arr.uniq
来源：http://psy.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://vug.meibo888.top

[D16] 求和与平均值
来源：http://xat.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pof.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kvr.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mhz.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yln.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zgv.pycfn.com

Go:   // 手写循环累加
来源：http://xol.yueranfly.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kkg.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://ref.ydzc1.top

[D17] 最大值与最小值
来源：http://sxo.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://gou.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://dtt.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cpt.aizwys.cn

TS:   Math.max(...arr);
来源：http://vkd.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zyk.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hhn.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://sfc.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://azj.tarul.cn

[D18] 扁平化嵌套数组
来源：http://kpg.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uez.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://lss.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aqe.chenjidiqi.icu

TS:   nested.flat();
来源：http://zwt.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bcm.ydjk.org.cn

Go:   // 手写双层循环
来源：http://yge.52xcode.cn

Ruby: nested.flatten
来源：http://zms.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cos.ydjk.org.cn

[D19] 按字段分组
来源：http://kqc.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://apq.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wfu.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kaj.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://vsd.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bwg.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://vae.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://plp.chenjidiqi.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yfv.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://lsz.fengsongda.top

Py:   Counter(arr)
来源：http://nnk.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://syc.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eym.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lkt.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vuk.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://rqu.andypj.xyz

Ruby: arr.tally
来源：http://yll.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yfp.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://vdf.fktsv.cn

Py:   x in arr
来源：http://otb.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://jjd.andypj.xyz

JS:   arr.includes(x)
来源：http://goh.zdqjudy.top

TS:   arr.includes(x)
来源：http://dbx.cashguo.top

Java: list.contains(x)
来源：http://dck.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://eqm.cdnleiting.top

Ruby: arr.include?(x)
来源：http://zax.yongpay.top

C#:   list.Contains(x)
来源：http://gsz.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://fmo.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hcj.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xfx.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zwx.hesvh.cn

TS:   [...arr];
来源：http://wvl.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://yhf.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://ssk.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://ivn.redwolf501.top

C#:   new List<int>(list);
来源：http://pom.gaohongyu789.top

[D23] reduce 累积计算
来源：http://xik.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ypa.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mrc.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iah.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nzd.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://him.gogol.net.cn

Go:   // 手写循环
来源：http://xvt.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jif.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nvx.xylfe.cn

[D24] 字典 / Map 基本操作
来源：http://sip.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bfz.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ypz.jiagoushi.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wlo.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fas.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ici.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gei.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://unz.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ddh.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://lax.c1oappe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mlg.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vkh.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baf.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nnv.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yyo.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bhz.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xal.jianghu66.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mny.hywenlv.cn

[D26] 数组转字符串
来源：http://ceb.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://yqq.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://fvc.tianlin.xyz

JS:   arr.join(", ")
来源：http://jrj.yfazqb.com

TS:   arr.join(", ")
来源：http://yux.52xcode.cn

Java: String.join(", ", list)
来源：http://bml.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://bvn.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://qij.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://faj.zhengqikj.top

================================================================================
来源：http://jqw.cqqwz.cn

E. 字符串处理
来源：http://phb.havefunace.top

================================================================================
来源：http://pwz.redwolf501.top

[E01] 拼接字符串
来源：http://jue.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mnj.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zmd.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qmm.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lpa.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lhn.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oyo.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bxp.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nsa.zhongyouzk.top

[E02] 重复字符串
来源：http://cee.fengsongda.top

Py:   "ab" * 3
来源：http://btt.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://tng.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://buu.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://vnm.xuanzx.com

Java: "ab".repeat(3)
来源：http://abw.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://esp.yongpay.top

Ruby: "ab" * 3
来源：http://gdz.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lnp.zdbjq.cn

[E03] 截取子串
来源：http://sau.zhongyouzk.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gog.gogol.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ufj.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mkn.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://riw.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://hgh.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://get.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://vom.cheryme.top

C#:   s.Substring(1, 3)
来源：http://gha.aizwys.cn

[E04] 查找子串位置
来源：http://djx.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://pym.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://suf.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gra.zycfv.cn

TS:   s.indexOf("x")
来源：http://gcl.hysaishi.cn

Java: s.indexOf("x")
来源：http://dbm.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://qhc.hcnkem.com

Ruby: s.index("x")
来源：http://ije.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://cdp.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vnb.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gyh.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bfz.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://frt.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fzl.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bqu.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xkj.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xlu.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ynp.ehwqpu.com

[E06] 替换子串
来源：http://pce.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mmp.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://tmz.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cja.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://ini.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jij.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zga.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qpi.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://gvq.cqqwz.cn

[E07] 按分隔符拆分
来源：http://ejl.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aio.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kip.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mfs.haohaochexian.top

TS:   s.split(",")
来源：http://vsh.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nrv.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yhj.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://gty.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wft.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://azu.ehwqpu.com

Py:   ",".join(items)
来源：http://wbi.jinyuanbaomall.cn

PHP:  implode(",", $items);
来源：http://ekk.aizwys.cn

JS:   items.join(",")
来源：http://mty.yfazqb.com

TS:   items.join(",")
来源：http://wwt.zhijiandao.cn

Java: String.join(",", items)
来源：http://ggu.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://olw.havefunace.top

Ruby: items.join(",")
来源：http://sfk.chenlongwang.top

C#:   string.Join(",", items)
来源：http://jrk.yonumen.top

[E09] 去除所有空白字符
来源：http://hxx.dianchejie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ezm.andypj.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yqq.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://aeb.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://cqc.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://rso.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://reo.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://gty.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uhf.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://quz.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rmy.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qbc.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://qfb.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://agy.sysykeji.top

Java: String.format("%03d", 7)
来源：http://hpy.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://get.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://orq.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lua.hnxiangtu.top

[E11] 反转字符串
来源：http://lvk.jyoumei.cn

Py:   s[::-1]
来源：http://fer.ydzc1.top

PHP:  strrev($s);
来源：http://fww.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://oje.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://kli.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://asj.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pzo.shangyingyoupin.top

Ruby: s.reverse
来源：http://pnv.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wle.hesvh.cn

[E12] 统计某字符出现次数
来源：http://icm.sysykeji.top

Py:   s.count("a")
来源：http://uhr.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://ypa.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://hdc.yongpay.top

TS:   s.split("a").length - 1
来源：http://znc.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sjc.cdnleiting.top

Go:   strings.Count(s, "a")
来源：http://ndd.bjfxy.top

Ruby: s.count("a")
来源：http://ask.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://yku.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://zeb.316326.xyz

Py:   for ch in s: print(ch)
来源：http://ghr.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cms.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bbn.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lqn.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yqp.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://beh.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xpw.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zkd.xuanzx.com

[E14] URL 编码与 Base64
来源：http://tec.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://reo.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jph.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cas.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eev.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ioa.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ekm.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yhh.hnqzz.top


<!-- 参考信息 -->