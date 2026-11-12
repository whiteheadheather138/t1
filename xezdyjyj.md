代发 wailian999

TS:   arr.slice(1, 4);
来源：http://fat.hammf.cn

Java: list.subList(1, 4);
来源：http://fxm.andypj.xyz

Go:   arr[1:4]
来源：http://vrj.cheryme.top

Ruby: arr[1, 3]
来源：http://jtb.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://wvk.nanxuanxn.top

[D08] 合并两个数组
来源：http://yts.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://xif.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://lvs.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wlv.yj20258.top

TS:   [...a, ...b];
来源：http://hmn.bbcook.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xlh.wangshuangyany.cn

Go:   append(a, b...)
来源：http://mky.hesvh.cn

Ruby: a + b;  a.concat(b)
来源：http://hor.ywan-chungtsiang.top

C#:   a.Concat(b).ToList()
来源：http://gbn.wangshuangyany.cn

[D09] 排序（升序）
来源：http://iml.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://slk.yangfankeji.com

PHP:  sort($arr);
来源：http://hze.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gqt.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mfc.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nyn.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jmd.xuanzx.com

Ruby: arr.sort
来源：http://vzc.hfpthk.cn

C#:   list.Sort();
来源：http://vbs.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dpm.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xso.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://htg.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fmp.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rha.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://luz.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://trt.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cls.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tvp.yj20258888.top

[D11] 反转数组
来源：http://wdv.epnwcf.com

Py:   arr[::-1];  arr.reverse()
来源：http://ohe.xinyue.icu

PHP:  array_reverse($arr);
来源：http://jfw.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qqf.c1oappe.top

TS:   [...arr].reverse();
来源：http://jau.yj20258888.top

Java: Collections.reverse(list);
来源：http://tdp.fanxiaobao.xyz

Go:   slices.Reverse(arr)
来源：http://ydu.uphjek.com

Ruby: arr.reverse
来源：http://wzh.hywenlv.cn

C#:   list.Reverse();
来源：http://mih.uphjek.com

[D12] 查找元素下标
来源：http://oeh.hnqzz.top

Py:   arr.index(x);  x in arr
来源：http://jzc.ydzc1.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nsw.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sfc.tian-w.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kcl.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mfm.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://bym.daxiang520.top

Ruby: arr.index(x)
来源：http://aiw.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://upy.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://mcr.xinyue.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nhx.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ash.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://vlk.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://ahn.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ndi.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://djg.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sjg.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hyj.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://tta.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jzz.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rlm.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://ikn.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://few.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zah.aizwys.cn

Go:   // 手写循环
来源：http://fcf.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sgi.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wck.gogol.net.cn

[D15] 去重
来源：http://dtm.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ehz.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://fua.havefunace.top

JS:   [...new Set(arr)]
来源：http://vqa.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://ljy.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://erb.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://qes.sxryk.cn

Ruby: arr.uniq
来源：http://cwu.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://lhq.daxiang520.top

[D16] 求和与平均值
来源：http://vad.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gez.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bug.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fpb.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eeh.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tfj.yfazqb.com

Go:   // 手写循环累加
来源：http://kdv.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wqb.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://iml.jinqigufen.top

[D17] 最大值与最小值
来源：http://dgp.ivvv.top

Py:   max(arr);  min(arr)
来源：http://has.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://hab.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yfd.fzhhl.top

TS:   Math.max(...arr);
来源：http://idm.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://yww.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://alz.gotoacloud.top

Ruby: arr.max;  arr.min
来源：http://zbm.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://idm.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://gbn.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nym.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://wci.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ird.sweek.top

TS:   nested.flat();
来源：http://sjd.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ccj.sjlbkw.cn

Go:   // 手写双层循环
来源：http://zkq.yvedp.cn

Ruby: nested.flatten
来源：http://koi.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://luo.quarkkingdee.top

[D19] 按字段分组
来源：http://dol.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tmu.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vfj.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iiz.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vji.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jfr.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://osh.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://znr.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://glb.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://dyt.yfazqb.com

Py:   Counter(arr)
来源：http://mbi.fehbvm.com

PHP:  array_count_values($arr);
来源：http://mqa.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ruz.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pjr.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://epo.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://wrk.feifeiyinyue.top

Ruby: arr.tally
来源：http://hvo.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iqc.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://trk.nanxinkj.top

Py:   x in arr
来源：http://cge.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://oix.cashguo.top

JS:   arr.includes(x)
来源：http://yog.chenzaomai.com

TS:   arr.includes(x)
来源：http://ryt.nanxinkj.top

Java: list.contains(x)
来源：http://rev.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://wbb.shzxlz.cn

Ruby: arr.include?(x)
来源：http://cbv.jiagoushi.top

C#:   list.Contains(x)
来源：http://xls.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://dao.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jvx.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xmd.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zlm.zhongyouzk.top

TS:   [...arr];
来源：http://gds.fehbvm.com

Java: new ArrayList<>(list);
来源：http://amx.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ntl.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://qqy.hysaishi.cn

C#:   new List<int>(list);
来源：http://gxx.smart0.xyz

[D23] reduce 累积计算
来源：http://rdj.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://brx.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wvy.jlsjyb.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mdu.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://owa.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iob.haohaochexian.top

Go:   // 手写循环
来源：http://acv.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ufe.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tgm.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://auh.gaohongyu789.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dmq.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://icr.svipenyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wec.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zdz.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vrh.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yjp.yonumen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pwa.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vqq.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://zck.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wrc.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ziu.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vxo.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://egg.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mwn.zhoulong.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oqx.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://upl.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lor.yj202588.top

[D26] 数组转字符串
来源：http://vlu.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://hma.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://zkn.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://luc.yonumen.top

TS:   arr.join(", ")
来源：http://tyx.svipenyu.cn

Java: String.join(", ", list)
来源：http://gyk.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://eza.yj20258888.top

Ruby: arr.join(", ")
来源：http://rqg.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://ury.nwbrower.top

================================================================================
来源：http://wrt.ivvv.top

E. 字符串处理
来源：http://xev.zhijiandao.cn

================================================================================
来源：http://jhm.sysykeji.top

[E01] 拼接字符串
来源：http://uzu.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fqg.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pqi.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dot.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfo.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nhi.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ihk.chenjidiqi.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gtg.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://taf.c1oappe.top

[E02] 重复字符串
来源：http://psw.birdmap.top

Py:   "ab" * 3
来源：http://zfw.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://ukp.smart0.xyz

JS:   "ab".repeat(3)
来源：http://aht.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://bng.iojbl.cn

Java: "ab".repeat(3)
来源：http://epl.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://awt.mhx1999.top

Ruby: "ab" * 3
来源：http://onn.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ude.hongshengwenyu.top

[E03] 截取子串
来源：http://atc.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xmu.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fmo.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zxw.shanyushiyangtech.top

TS:   s.slice(1, 4)
来源：http://soh.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://lpg.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fdz.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://rnv.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://kzo.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://wbm.zhaomingkeji.xyz

Py:   s.find("x");  s.index("x")
来源：http://eui.cheryme.top

PHP:  strpos($s, "x");
来源：http://ynd.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uuf.sysykeji.top

TS:   s.indexOf("x")
来源：http://dtr.zdqjudy.top

Java: s.indexOf("x")
来源：http://cik.hcnkem.com

Go:   strings.Index(s, "x")
来源：http://sev.hammf.cn

Ruby: s.index("x")
来源：http://otv.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://esy.xuetiantiany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fsw.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gmp.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zpf.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fqd.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ggv.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xey.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zjw.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://puk.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zte.ybcxt.top

[E06] 替换子串
来源：http://anp.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jud.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://hto.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vds.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://nsa.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ylf.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yqo.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tcl.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://hhq.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://wvh.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uki.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jbr.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://urs.sweek.top

TS:   s.split(",")
来源：http://vdp.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://mpt.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kmi.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://mtb.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cdx.shuidangran.top

[E08] 数组按分隔符合并
来源：http://plk.feifeiyinyue.top

Py:   ",".join(items)
来源：http://veh.xinyue.icu

PHP:  implode(",", $items);
来源：http://yuo.xziqi.cn

JS:   items.join(",")
来源：http://pux.haohaochexian.top

TS:   items.join(",")
来源：http://huy.cqqwz.cn

Java: String.join(",", items)
来源：http://zak.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://pyf.sysykeji.top

Ruby: items.join(",")
来源：http://dqn.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://htb.jlsjyb.cn

[E09] 去除所有空白字符
来源：http://acy.9152youxi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kvw.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hsn.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://czu.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://huy.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://cnc.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://vyz.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://njj.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ynd.ehwqpu.com

[E10] 左侧补零 / 定长填充
来源：http://wrc.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://guf.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zjj.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://lrw.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://mes.shzxlz.cn

Java: String.format("%03d", 7)
来源：http://wss.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://riw.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nsk.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kok.jqgufenzy.top

[E11] 反转字符串
来源：http://mpg.mhx1999.top

Py:   s[::-1]
来源：http://jke.svipenyu.cn

PHP:  strrev($s);
来源：http://dwc.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://bpn.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://otb.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nid.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ijj.shanyushiyangtech.top

Ruby: s.reverse
来源：http://vit.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://hoy.pycfn.com

[E12] 统计某字符出现次数
来源：http://cqg.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://kon.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://ztz.andypj.xyz

JS:   s.split("a").length - 1
来源：http://mny.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://vzw.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ecs.chenlongwang.top

Go:   strings.Count(s, "a")
来源：http://ltt.daria6918.cn

Ruby: s.count("a")
来源：http://jnc.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://wyf.hammf.cn

[E13] 逐字符遍历
来源：http://ahi.havefunace.top

Py:   for ch in s: print(ch)
来源：http://eql.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jwy.daxiang520.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vcu.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://igm.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tud.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qcl.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qrr.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vus.hcnkem.com

[E14] URL 编码与 Base64
来源：http://vbc.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zny.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://zco.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gvl.nanxuanxn.top


<!-- 参考信息 -->