代发 wailian999

PHP:  sort($arr);
来源：http://cqy.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yli.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xgb.zhongyouzk.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bat.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oqd.cucudq.cn

Ruby: arr.sort
来源：http://qwp.yongpay.top

C#:   list.Sort();
来源：http://nnp.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zvs.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vur.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://evb.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aeq.c1oappe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dpx.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nup.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qrk.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kgm.andypj.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pzr.uphjek.com

[D11] 反转数组
来源：http://pvl.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://iht.zhijiandao.cn

PHP:  array_reverse($arr);
来源：http://xem.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xsp.xziqi.cn

TS:   [...arr].reverse();
来源：http://oua.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://tul.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://zrm.yuxming.cn

Ruby: arr.reverse
来源：http://jxo.ydzc1.top

C#:   list.Reverse();
来源：http://tig.fengsongda.top

[D12] 查找元素下标
来源：http://rua.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://ozd.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ndw.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cev.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://for.chenzaomai.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iti.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://yxd.tianlin.xyz

Ruby: arr.index(x)
来源：http://dfj.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://rby.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://ocg.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fnj.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rps.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://svq.shangyingyoupin.top

TS:   arr.filter(x => x > 3)
来源：http://dim.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ylf.uphjek.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pgz.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://mdt.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ovt.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://orr.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rmt.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kss.tian-w.cn

JS:   arr.map(x => x * 2)
来源：http://hwt.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://jmq.daria6918.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fcv.cheryme.top

Go:   // 手写循环
来源：http://ggk.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://udw.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jgu.ivvv.top

[D15] 去重
来源：http://gpa.zhoulong.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gnr.aibaodan.cn

PHP:  array_unique($arr);
来源：http://std.mhx1999.top

JS:   [...new Set(arr)]
来源：http://jln.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://uki.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kvd.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://lzn.ehwqpu.com

Ruby: arr.uniq
来源：http://ojj.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://ahd.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://zhc.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bdn.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bgh.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rix.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dot.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jsw.birdmap.top

Go:   // 手写循环累加
来源：http://izx.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lkn.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://dlf.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://out.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://jgq.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://frh.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://slp.cheryme.top

TS:   Math.max(...arr);
来源：http://tgd.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bft.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pfj.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://bcj.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://nqn.kuanghao11.cn

[D18] 扁平化嵌套数组
来源：http://hjz.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yms.tarul.cn

PHP:  array_merge(...$nested);
来源：http://hlv.gotoacloud.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xym.shuidangran.top

TS:   nested.flat();
来源：http://nfq.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hjg.jqgufenzy.top

Go:   // 手写双层循环
来源：http://lbh.guannengcc.top

Ruby: nested.flatten
来源：http://ztl.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hhd.hfpthk.cn

[D19] 按字段分组
来源：http://keu.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hvz.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rrh.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dwg.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://lxz.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tep.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://sfv.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fdp.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pit.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://epx.ehwqpu.com

Py:   Counter(arr)
来源：http://urr.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://nqb.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fnb.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ubo.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gvx.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://myo.dashuyun.cn

Ruby: arr.tally
来源：http://swy.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://osu.hcnkem.com

[D21] 判断是否包含某元素
来源：http://lns.zhengqikj.top

Py:   x in arr
来源：http://jlj.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://mlo.hnxiangtu.top

JS:   arr.includes(x)
来源：http://cib.kuanghao11.cn

TS:   arr.includes(x)
来源：http://qfa.hnxiangtu.top

Java: list.contains(x)
来源：http://kwx.ivvv.top

Go:   slices.Contains(arr, x)
来源：http://rkd.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://iyu.xziqi.cn

C#:   list.Contains(x)
来源：http://jzq.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://txi.shuidangran.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lmz.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xvc.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bqu.hcnkem.com

TS:   [...arr];
来源：http://iwr.yueranfly.top

Java: new ArrayList<>(list);
来源：http://djh.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sqb.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://jfg.sweek.top

C#:   new List<int>(list);
来源：http://yzm.mhx1999.top

[D23] reduce 累积计算
来源：http://fqy.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bnh.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vbl.chenlongwang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tbd.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uyq.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gjr.jqgfzy.top

Go:   // 手写循环
来源：http://ybj.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://exg.wangdashe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qve.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://hsu.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lql.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bes.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nbv.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://foa.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xuu.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pkw.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mvq.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rsj.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://sep.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wak.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ojq.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zdm.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pnc.chenlongwang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ofn.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uvc.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://npq.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tnm.yvedp.cn

[D26] 数组转字符串
来源：http://ihq.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://gyk.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://bwr.hnqzz.top

JS:   arr.join(", ")
来源：http://wva.316326.xyz

TS:   arr.join(", ")
来源：http://jku.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://xif.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://aod.tarul.cn

Ruby: arr.join(", ")
来源：http://sta.guannengcc.top

C#:   string.Join(", ", list)
来源：http://txu.chenzaomai.com

================================================================================
来源：http://nle.cucudq.cn

E. 字符串处理
来源：http://qxf.zycfv.cn

================================================================================
来源：http://ucm.yvedp.cn

[E01] 拼接字符串
来源：http://nrh.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lih.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://foa.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cdr.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zgv.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pud.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sra.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dfi.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vvm.ybcxt.top

[E02] 重复字符串
来源：http://bsn.tarul.cn

Py:   "ab" * 3
来源：http://bxz.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://okl.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://nuw.ydzc1.top

TS:   "ab".repeat(3)
来源：http://lyk.ctjpmb.com

Java: "ab".repeat(3)
来源：http://dat.yangfankeji.com

Go:   strings.Repeat("ab", 3)
来源：http://mia.xinyue.icu

Ruby: "ab" * 3
来源：http://kxi.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cws.smart0.xyz

[E03] 截取子串
来源：http://zfh.birdmap.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qbc.wangdashe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wtn.shangyingyoupin.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://opl.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://wqe.zdqjudy.top

Java: s.substring(1, 4)
来源：http://bjt.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ttq.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://blv.uphjek.com

C#:   s.Substring(1, 3)
来源：http://ywj.jiagoushi.top

[E04] 查找子串位置
来源：http://nqz.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://mya.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://uih.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kau.andypj.xyz

TS:   s.indexOf("x")
来源：http://ham.haohaochexian.top

Java: s.indexOf("x")
来源：http://exg.jqgfzy.top

Go:   strings.Index(s, "x")
来源：http://wxc.quarkkingdee.top

Ruby: s.index("x")
来源：http://ixl.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://kyf.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cls.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hmn.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ppp.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mfr.yangfankeji.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://jth.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fam.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://run.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xfw.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nko.feifeiyinyue.top

[E06] 替换子串
来源：http://rdi.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fhf.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://qxk.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bng.guowangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://tag.9152youxi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ddr.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ada.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kqb.yj202588.top

C#:   s.Replace("a", "b")
来源：http://zue.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://aqj.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rbd.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ojn.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://vwa.tarul.cn

TS:   s.split(",")
来源：http://fsf.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qyk.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kbc.uphjek.com

Ruby: s.split(",");  s.split
来源：http://gqe.kuanghao11.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dtn.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://zsh.mhx1999.top

Py:   ",".join(items)
来源：http://lxx.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://uro.chenjidiqi.icu

JS:   items.join(",")
来源：http://onr.ybcxt.top

TS:   items.join(",")
来源：http://tch.yfazqb.com

Java: String.join(",", items)
来源：http://aqs.gogol.net.cn

Go:   strings.Join(items, ",")
来源：http://qek.52xcode.cn

Ruby: items.join(",")
来源：http://ycy.snrcjt.cn

C#:   string.Join(",", items)
来源：http://jvm.nwbrower.top

[E09] 去除所有空白字符
来源：http://hez.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dsg.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://txx.wangdashe.top

JS:   s.replace(/\s+/g, "")
来源：http://omq.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ojl.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://wbr.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://afb.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://sji.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://epa.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://omv.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fzt.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rik.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://kvq.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://jqj.yj20258.top

Java: String.format("%03d", 7)
来源：http://pgh.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ovk.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ish.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rmv.daxiang520.top

[E11] 反转字符串
来源：http://xza.9152youxi.cn

Py:   s[::-1]
来源：http://xmv.hammf.cn

PHP:  strrev($s);
来源：http://ahg.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://xjo.yonumen.top

TS:   [...s].reverse().join("")
来源：http://edj.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dit.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vmi.hysaishi.cn

Ruby: s.reverse
来源：http://wch.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://wqz.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://srv.ivvv.top

Py:   s.count("a")
来源：http://ibj.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://adi.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://hlg.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://oay.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bic.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://loj.yuanzhike.top

Ruby: s.count("a")
来源：http://wes.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://qwy.uphjek.com

[E13] 逐字符遍历
来源：http://twn.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://vmm.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dtx.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uwh.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kcw.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lee.zhengqikj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nyh.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zkr.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mgx.havefunace.top

[E14] URL 编码与 Base64
来源：http://sbw.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uea.havefunace.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://skn.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xgo.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vss.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xea.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kkl.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pnj.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qlx.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://usg.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xos.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://whx.shanyushiyangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cko.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://chm.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fee.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://exi.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qma.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://juq.yueranfly.top

[E16] 数字千分位
来源：http://kcd.sysykeji.top

Py:   f"{1234567:,}"
来源：http://twc.xingfuxueyuan.xyz


<!-- 参考信息 -->