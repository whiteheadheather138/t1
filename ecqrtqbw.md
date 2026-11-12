代发 wailian999

PHP:  sort($arr);
来源：http://jyg.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://umj.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://znf.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ljp.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rfa.redwolf501.top

Ruby: arr.sort
来源：http://pjx.redwolf501.top

C#:   list.Sort();
来源：http://opg.hongshengwenyu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hia.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vsz.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vgs.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://onc.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://spx.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://apq.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zgh.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cbm.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gic.hcnkem.com

[D11] 反转数组
来源：http://xch.yonumen.top

Py:   arr[::-1];  arr.reverse()
来源：http://utk.yfazqb.com

PHP:  array_reverse($arr);
来源：http://awc.jqgufenzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ccx.xinyue.icu

TS:   [...arr].reverse();
来源：http://pfm.tianlin.xyz

Java: Collections.reverse(list);
来源：http://nfd.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://zof.zhongyouzk.top

Ruby: arr.reverse
来源：http://rwo.gzhubu.top

C#:   list.Reverse();
来源：http://xjt.sweek.top

[D12] 查找元素下标
来源：http://wmh.hesvh.cn

Py:   arr.index(x);  x in arr
来源：http://mwu.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pbg.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ctv.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gsx.ydjk.org.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tzm.hammf.cn

Go:   slices.Index(arr, x)
来源：http://sfk.svipenyu.cn

Ruby: arr.index(x)
来源：http://ajt.uphjek.com

C#:   list.IndexOf(x);
来源：http://ibu.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://gba.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dak.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mbv.hnxiangtu.top

JS:   arr.filter(x => x > 3)
来源：http://tbq.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://xie.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bzd.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hgi.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zow.vehdjk.com

C#:   list.Where(x => x > 3).ToList()
来源：http://qmm.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://hda.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jzw.sufxvd.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://clh.hammf.cn

JS:   arr.map(x => x * 2)
来源：http://vzl.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://soo.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dnv.aibaodan.cn

Go:   // 手写循环
来源：http://xfc.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://act.ybcxt.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fba.dashuyun.cn

[D15] 去重
来源：http://vbm.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aeq.zdbjq.cn

PHP:  array_unique($arr);
来源：http://vod.wangdashe.top

JS:   [...new Set(arr)]
来源：http://skn.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://qfb.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xmx.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://exu.jinqigfzy.top

Ruby: arr.uniq
来源：http://lau.cheryme.top

C#:   list.Distinct().ToList()
来源：http://tfz.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://chq.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pgg.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nkj.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://otx.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qrx.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mnm.yuxming.cn

Go:   // 手写循环累加
来源：http://ihe.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eqr.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://qny.zhengqikj.top

[D17] 最大值与最小值
来源：http://dns.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://rdu.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://edq.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vhw.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://qeh.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ouf.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jja.birdmap.top

Ruby: arr.max;  arr.min
来源：http://ims.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://jgs.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://tdy.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ioe.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://khm.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ijj.fzhhl.top

TS:   nested.flat();
来源：http://amd.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sop.tarul.cn

Go:   // 手写双层循环
来源：http://pco.havefunace.top

Ruby: nested.flatten
来源：http://tfz.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ose.aizwys.cn

[D19] 按字段分组
来源：http://dnu.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://btb.c1oappe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ubg.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ynt.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gvk.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://owt.ivvv.top

Go:   // 手写 map[string][]T
来源：http://xbf.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pqp.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iux.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://rsl.chenzaomai.com

Py:   Counter(arr)
来源：http://hgs.52xcode.cn

PHP:  array_count_values($arr);
来源：http://hqb.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qqu.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://atn.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tbe.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://ojb.redwolf501.top

Ruby: arr.tally
来源：http://dal.fktsv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lhw.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://khp.zhengqikj.top

Py:   x in arr
来源：http://cmy.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://lby.redwolf501.top

JS:   arr.includes(x)
来源：http://mlh.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://aoz.zhengqikj.top

Java: list.contains(x)
来源：http://dtl.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://tut.ctjpmb.com

Ruby: arr.include?(x)
来源：http://bbq.sweek.top

C#:   list.Contains(x)
来源：http://zbf.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://jff.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://svy.yanxiufei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bha.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wfm.meibo888.top

TS:   [...arr];
来源：http://vri.xinyue.icu

Java: new ArrayList<>(list);
来源：http://laq.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://pqv.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://ysm.yanxiufei.cn

C#:   new List<int>(list);
来源：http://mtf.zdbjq.cn

[D23] reduce 累积计算
来源：http://jau.chenlongwang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gtt.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cmi.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ati.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dse.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rvv.gogol.net.cn

Go:   // 手写循环
来源：http://wtx.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pib.guannengcc.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nmd.c1oappe.top

[D24] 字典 / Map 基本操作
来源：http://bxl.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qbm.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jni.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://exg.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gec.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://soq.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sdq.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://czd.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hdu.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://ljz.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cph.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://guj.hfpthk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mss.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kqw.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uod.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vfb.yonumen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dat.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gfw.zdqjudy.top

[D26] 数组转字符串
来源：http://uix.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://itp.yongpay.top

PHP:  implode(", ", $arr);
来源：http://cpm.gotoacloud.top

JS:   arr.join(", ")
来源：http://xkx.hammf.cn

TS:   arr.join(", ")
来源：http://vls.iojbl.cn

Java: String.join(", ", list)
来源：http://duq.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://iwd.daxiang520.top

Ruby: arr.join(", ")
来源：http://wdg.shzxlz.cn

C#:   string.Join(", ", list)
来源：http://wze.jqgufenzy.top

================================================================================
来源：http://zxy.tanke756.top

E. 字符串处理
来源：http://qsu.smart0.xyz

================================================================================
来源：http://nqe.hnxiangtu.top

[E01] 拼接字符串
来源：http://xgs.zhongyouzk.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kyn.zdqjudy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aru.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ipg.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wpx.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://spu.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zbp.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://epf.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rwk.jqgufenzy.top

[E02] 重复字符串
来源：http://svz.haohaochexian.top

Py:   "ab" * 3
来源：http://mgw.daxiang520.top

PHP:  str_repeat("ab", 3);
来源：http://vkg.hammf.cn

JS:   "ab".repeat(3)
来源：http://bhr.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://zli.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://fcb.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://owj.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://mke.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ueb.hnqzz.top

[E03] 截取子串
来源：http://mnv.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zwl.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pxj.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sio.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://ixx.snrcjt.cn

Java: s.substring(1, 4)
来源：http://xco.gogol.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bry.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://zkw.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://hoa.zhijiandao.cn

[E04] 查找子串位置
来源：http://qhv.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://bhl.bjfxy.top

PHP:  strpos($s, "x");
来源：http://xqs.ybcxt.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://avx.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://knu.gzhubu.top

Java: s.indexOf("x")
来源：http://knw.shanyushiyangtech.top

Go:   strings.Index(s, "x")
来源：http://aow.bjfxy.top

Ruby: s.index("x")
来源：http://xls.epnwcf.com

C#:   s.IndexOf("x")
来源：http://hco.xziqi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pyb.svipenyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lbz.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://alt.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uos.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://foo.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bgt.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hca.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nwc.jlsjyb.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kin.cqqwz.cn

[E06] 替换子串
来源：http://oym.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ret.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://kqi.jlsjyb.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uji.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://mqa.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tid.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://non.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rmd.cheryme.top

C#:   s.Replace("a", "b")
来源：http://jnc.52xcode.cn

[E07] 按分隔符拆分
来源：http://ymn.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rdt.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tuu.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://qln.kuanghao11.cn

TS:   s.split(",")
来源：http://mha.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://ykk.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://izv.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://gjf.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ezo.yj20258888.top

[E08] 数组按分隔符合并
来源：http://hmd.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://ueq.sxryk.cn

PHP:  implode(",", $items);
来源：http://uql.daria6918.cn

JS:   items.join(",")
来源：http://dsu.chenlongwang.top

TS:   items.join(",")
来源：http://aeo.wangshuangyany.cn

Java: String.join(",", items)
来源：http://khy.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://xuo.nwbrower.top

Ruby: items.join(",")
来源：http://myx.yvedp.cn

C#:   string.Join(",", items)
来源：http://nty.0kj1m.cn

[E09] 去除所有空白字符
来源：http://epe.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hjr.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wuo.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://dbx.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://eha.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://epa.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tfh.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://vtx.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dxp.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://rgu.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nzw.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rqb.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://wlx.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://vhq.meibo888.top

Java: String.format("%03d", 7)
来源：http://fdk.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yss.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tld.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://paj.hfpthk.cn

[E11] 反转字符串
来源：http://ebc.snrcjt.cn

Py:   s[::-1]
来源：http://fth.xuanzx.com

PHP:  strrev($s);
来源：http://wjo.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://uyt.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://bmn.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ghu.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://shj.xinyue.icu

Ruby: s.reverse
来源：http://vec.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://ipn.andypj.xyz

[E12] 统计某字符出现次数
来源：http://omv.ehwqpu.com

Py:   s.count("a")
来源：http://vjr.havefunace.top

PHP:  substr_count($s, "a");
来源：http://nzn.redwolf501.top

JS:   s.split("a").length - 1
来源：http://jbc.fehbvm.com

TS:   s.split("a").length - 1
来源：http://tio.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ant.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://qxj.ehwqpu.com

Ruby: s.count("a")
来源：http://xdv.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://wtm.sufxvd.cn

[E13] 逐字符遍历
来源：http://vrg.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://nxv.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fvf.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://phz.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://lci.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gef.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lqs.fzhhl.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ags.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gul.fengsongda.top

[E14] URL 编码与 Base64
来源：http://avn.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gbd.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zjd.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wgs.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lgo.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ysm.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://akc.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://znb.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qas.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://jju.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ehk.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kro.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gii.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tdw.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://otm.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zjn.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ppr.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mpn.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://rcj.guannengcc.top

Py:   f"{1234567:,}"
来源：http://lsq.havefunace.top


<!-- 参考信息 -->