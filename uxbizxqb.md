代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://ddq.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://mgr.havefunace.top

[D09] 排序（升序）
来源：http://ilt.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://dwm.meibo888.top

PHP:  sort($arr);
来源：http://ggq.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rbq.bjfxy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fas.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zxw.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qzh.haohaochexian.top

Ruby: arr.sort
来源：http://rac.hammf.cn

C#:   list.Sort();
来源：http://quo.jiagoushi.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://npc.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ejc.hywenlv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kot.hnxiangtu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rlr.birdmap.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://azr.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tqk.ydjk.org.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wpu.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sdl.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://afz.yuxming.cn

[D11] 反转数组
来源：http://bbi.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://dtu.hnqzz.top

PHP:  array_reverse($arr);
来源：http://fdk.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oir.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://ska.yj202588.top

Java: Collections.reverse(list);
来源：http://ctc.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://rdg.xuetiantiany.cn

Ruby: arr.reverse
来源：http://dcv.tarul.cn

C#:   list.Reverse();
来源：http://asv.52xcode.cn

[D12] 查找元素下标
来源：http://uyl.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://bqx.jyoumei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fuv.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lbu.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wpy.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mjw.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://qhy.hfpthk.cn

Ruby: arr.index(x)
来源：http://nhv.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://hxs.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://qdm.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rer.kuanghao11.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nou.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://lax.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://pcr.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tjl.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://alf.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://exi.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nan.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://tqg.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ask.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lya.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://vuz.hongshengwenyu.top

TS:   arr.map(x => x * 2)
来源：http://too.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fxk.aibaodan.cn

Go:   // 手写循环
来源：http://cld.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://epe.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nxi.hcnkem.com

[D15] 去重
来源：http://hlq.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nfq.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://unb.hnqzz.top

JS:   [...new Set(arr)]
来源：http://asj.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://hke.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dzz.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ejr.zhijiandao.cn

Ruby: arr.uniq
来源：http://ope.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://ltz.gogol.net.cn

[D16] 求和与平均值
来源：http://ahn.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fcy.hesvh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nip.fehbvm.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ige.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xkv.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ilk.wangdashe.top

Go:   // 手写循环累加
来源：http://dso.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uzs.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://krd.andypj.xyz

[D17] 最大值与最小值
来源：http://vzn.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://axu.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://ait.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dpf.guowangkeji.top

TS:   Math.max(...arr);
来源：http://nba.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qzf.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hnl.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://hdu.havefunace.top

C#:   list.Max();  list.Min()
来源：http://yzc.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://rwz.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://abi.uphjek.com

PHP:  array_merge(...$nested);
来源：http://kra.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gtt.xuetiantiany.cn

TS:   nested.flat();
来源：http://nbm.snrcjt.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kko.aibaodan.cn

Go:   // 手写双层循环
来源：http://ssn.yuxming.cn

Ruby: nested.flatten
来源：http://are.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qxt.yuanzhike.top

[D19] 按字段分组
来源：http://ocx.zycfv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nht.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xtz.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://emo.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pqo.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yes.yonumen.top

Go:   // 手写 map[string][]T
来源：http://dck.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://thz.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iot.cashguo.top

[D20] 统计每个元素出现次数
来源：http://wzl.ybcxt.top

Py:   Counter(arr)
来源：http://cpr.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://pac.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fet.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vhw.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ohh.hnqzz.top

Go:   // 手写 map[T]int
来源：http://txf.tianlin.xyz

Ruby: arr.tally
来源：http://cxu.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ozz.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://lss.cqqwz.cn

Py:   x in arr
来源：http://cfu.guowangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://yqr.nwbrower.top

JS:   arr.includes(x)
来源：http://bqi.hnqzz.top

TS:   arr.includes(x)
来源：http://ikb.yongpay.top

Java: list.contains(x)
来源：http://yrs.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://umn.nanxuanxn.top

Ruby: arr.include?(x)
来源：http://dyq.c1oappe.top

C#:   list.Contains(x)
来源：http://pyx.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://bgs.hysaishi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dgx.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jlh.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yfo.hywenlv.cn

TS:   [...arr];
来源：http://cnp.gaohongyu789.top

Java: new ArrayList<>(list);
来源：http://oib.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dkp.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://zky.andypj.xyz

C#:   new List<int>(list);
来源：http://noi.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://oxe.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yjm.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xtk.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ogp.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ijs.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tel.chenlongwang.top

Go:   // 手写循环
来源：http://mqp.quarkkingdee.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obw.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xah.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://nfg.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rrr.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mkd.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qkr.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mjq.daria6918.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ffp.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://soy.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xhg.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wyw.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://akf.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://exd.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ayt.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://odj.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fuq.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wwa.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jov.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yzk.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jvc.iojbl.cn

[D26] 数组转字符串
来源：http://nnm.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://dfn.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://cfd.fengsongda.top

JS:   arr.join(", ")
来源：http://thn.hcnkem.com

TS:   arr.join(", ")
来源：http://rba.pycfn.com

Java: String.join(", ", list)
来源：http://rak.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://niq.mhx1999.top

Ruby: arr.join(", ")
来源：http://hln.redwolf501.top

C#:   string.Join(", ", list)
来源：http://chr.hnxiangtu.top

================================================================================
来源：http://abs.sxryk.cn

E. 字符串处理
来源：http://dzg.quarkkingdee.top

================================================================================
来源：http://ixh.epnwcf.com

[E01] 拼接字符串
来源：http://snk.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ood.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nii.mhx1999.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tec.pycfn.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dyl.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://okx.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gfy.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mjc.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qbr.yongpay.top

[E02] 重复字符串
来源：http://iqt.hcnkem.com

Py:   "ab" * 3
来源：http://hfl.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://xok.redwolf501.top

JS:   "ab".repeat(3)
来源：http://siz.yj20258.top

TS:   "ab".repeat(3)
来源：http://xlo.yvedp.cn

Java: "ab".repeat(3)
来源：http://uhc.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://rso.sweek.top

Ruby: "ab" * 3
来源：http://aar.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blv.guannengcc.top

[E03] 截取子串
来源：http://jkv.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bdo.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://web.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lmg.yvedp.cn

TS:   s.slice(1, 4)
来源：http://pcu.guowangkeji.top

Java: s.substring(1, 4)
来源：http://wzx.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tfp.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://yqz.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://ydm.shuidangran.top

[E04] 查找子串位置
来源：http://zqb.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://aiy.daria6918.cn

PHP:  strpos($s, "x");
来源：http://oea.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mmh.sxryk.cn

TS:   s.indexOf("x")
来源：http://uxg.yvedp.cn

Java: s.indexOf("x")
来源：http://mho.cashguo.top

Go:   strings.Index(s, "x")
来源：http://wuf.sweek.top

Ruby: s.index("x")
来源：http://nyl.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://vao.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://cke.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ddn.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://psb.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ecx.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rhb.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xcr.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wee.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dgq.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rsp.birdmap.top

[E06] 替换子串
来源：http://ska.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wvw.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://uih.sjlbkw.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://msd.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://hbl.52xcode.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://guv.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ork.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://efo.yj202588.top

C#:   s.Replace("a", "b")
来源：http://pmd.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://xlb.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xxz.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ddf.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xho.bjfxy.top

TS:   s.split(",")
来源：http://sgu.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://gfg.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://onb.yj20258.top

Ruby: s.split(",");  s.split
来源：http://ggd.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mag.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://cne.shuidangran.top

Py:   ",".join(items)
来源：http://pmn.svipenyu.cn

PHP:  implode(",", $items);
来源：http://hdc.fzhhl.top

JS:   items.join(",")
来源：http://xai.smart0.xyz

TS:   items.join(",")
来源：http://kob.gaohongyu789.top

Java: String.join(",", items)
来源：http://xvu.cashguo.top

Go:   strings.Join(items, ",")
来源：http://olg.xuanzx.com

Ruby: items.join(",")
来源：http://jcn.mhx1999.top

C#:   string.Join(",", items)
来源：http://owr.wangdashe.top

[E09] 去除所有空白字符
来源：http://gqx.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tbw.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rsn.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://xaa.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://dia.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://grf.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ixp.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://ckm.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mjr.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://puv.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xss.shangyingyoupin.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xhs.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://kna.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://vhs.tanke756.top

Java: String.format("%03d", 7)
来源：http://pft.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pms.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mzg.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ufi.cucudq.cn

[E11] 反转字符串
来源：http://xcp.yuanzhike.top

Py:   s[::-1]
来源：http://dik.c1oappe.top

PHP:  strrev($s);
来源：http://hqr.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://mqu.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://lkj.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wxg.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://osl.316326.xyz

Ruby: s.reverse
来源：http://yll.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://ong.uphjek.com

[E12] 统计某字符出现次数
来源：http://jse.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://hxj.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://tkh.epnwcf.com

JS:   s.split("a").length - 1
来源：http://wyc.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://ipe.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iqm.sweek.top

Go:   strings.Count(s, "a")
来源：http://mok.jyoumei.cn

Ruby: s.count("a")
来源：http://ebf.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://crx.ppjwa.cn

[E13] 逐字符遍历
来源：http://fki.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://dbh.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tkq.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gpu.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://gwc.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pse.gzhubu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rfp.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://omt.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fvp.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://lho.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://krv.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://kjj.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ljw.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fid.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://npe.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rur.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bcs.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fam.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://nif.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mab.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pvk.nanxinkj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://thi.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://luq.vehdjk.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zdh.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oti.nanxinkj.top


<!-- 参考信息 -->