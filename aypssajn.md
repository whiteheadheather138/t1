代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://osv.cqqwz.cn

Ruby: arr.sort
来源：http://lwo.dianchejie.cn

C#:   list.Sort();
来源：http://ulu.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wng.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bny.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uzv.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cfr.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kix.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hnr.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xbb.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://scm.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wlf.andypj.xyz

[D11] 反转数组
来源：http://sub.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://oys.xylfe.cn

PHP:  array_reverse($arr);
来源：http://iag.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dkc.chenlongwang.top

TS:   [...arr].reverse();
来源：http://bbz.hfpthk.cn

Java: Collections.reverse(list);
来源：http://vgx.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://klp.aibaodan.cn

Ruby: arr.reverse
来源：http://lhm.hnqzz.top

C#:   list.Reverse();
来源：http://glb.mhx1999.top

[D12] 查找元素下标
来源：http://siv.sxryk.cn

Py:   arr.index(x);  x in arr
来源：http://dam.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://klx.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gra.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwa.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wgw.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://geh.tianlin.xyz

Ruby: arr.index(x)
来源：http://gng.tanke756.top

C#:   list.IndexOf(x);
来源：http://mpl.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://sdc.tanke756.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bec.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://brp.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://awy.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://drn.hesvh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hes.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pgv.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://pii.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oig.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://knq.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lro.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jur.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://pra.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://rwo.fktsv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zse.yuanzhike.top

Go:   // 手写循环
来源：http://iqu.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fta.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://swf.uphjek.com

[D15] 去重
来源：http://vrj.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ghr.meibo888.top

PHP:  array_unique($arr);
来源：http://iwb.xinyue.icu

JS:   [...new Set(arr)]
来源：http://tuv.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://atg.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fhf.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://fhk.tianlin.xyz

Ruby: arr.uniq
来源：http://sha.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://maq.chenlongwang.top

[D16] 求和与平均值
来源：http://tip.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qki.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ucr.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fth.daxiang520.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://isf.fanxiaobao.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://huv.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://aph.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hal.sufxvd.cn

C#:   list.Sum();  list.Average()
来源：http://fod.quarkkingdee.top

[D17] 最大值与最小值
来源：http://vku.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://ate.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://vct.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fir.cdnleiting.top

TS:   Math.max(...arr);
来源：http://afh.yvedp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ino.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://okb.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://xzl.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://hli.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://qgq.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wiq.sweek.top

PHP:  array_merge(...$nested);
来源：http://qkz.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nmd.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://mnd.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://juh.pycfn.com

Go:   // 手写双层循环
来源：http://nce.daria6918.cn

Ruby: nested.flatten
来源：http://fil.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wtw.9152youxi.cn

[D19] 按字段分组
来源：http://ewc.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iwm.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vfa.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ppa.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eqr.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sif.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://yvv.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dnc.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xny.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://khe.cashguo.top

Py:   Counter(arr)
来源：http://sjo.epnwcf.com

PHP:  array_count_values($arr);
来源：http://mlq.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gmp.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://owh.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dht.fzhhl.top

Go:   // 手写 map[T]int
来源：http://dti.hysaishi.cn

Ruby: arr.tally
来源：http://jrq.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lcz.cucudq.cn

[D21] 判断是否包含某元素
来源：http://bte.iojbl.cn

Py:   x in arr
来源：http://sgt.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://iya.xinyue.icu

JS:   arr.includes(x)
来源：http://unm.sysykeji.top

TS:   arr.includes(x)
来源：http://ftj.cqqwz.cn

Java: list.contains(x)
来源：http://scs.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://ggg.tarul.cn

Ruby: arr.include?(x)
来源：http://tpu.zhongyouzk.top

C#:   list.Contains(x)
来源：http://lob.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://haa.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qnf.mhx1999.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hki.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uxj.vqdsnc.cn

TS:   [...arr];
来源：http://ckq.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://mma.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bgh.tian-w.cn

Ruby: arr.dup;  arr.clone
来源：http://sph.pycfn.com

C#:   new List<int>(list);
来源：http://njc.yj20258888.top

[D23] reduce 累积计算
来源：http://hqw.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://roa.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lac.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qnc.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pbx.jinghuilouyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vdx.smart0.xyz

Go:   // 手写循环
来源：http://adh.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ppj.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://omm.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://rxf.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ivz.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hra.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://voa.cheryme.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jht.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nko.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qaa.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hzk.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://suj.hnqzz.top

[D25] Set 集合去重与交并差
来源：http://lom.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://roa.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jlz.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hvi.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://phm.zdqjudy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mxm.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aor.ybcxt.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ume.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yhg.mhx1999.top

[D26] 数组转字符串
来源：http://yiq.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://njc.pycfn.com

PHP:  implode(", ", $arr);
来源：http://dxk.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://tkt.yvedp.cn

TS:   arr.join(", ")
来源：http://lyb.daxiang520.top

Java: String.join(", ", list)
来源：http://fge.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://bbn.yuxming.cn

Ruby: arr.join(", ")
来源：http://vxg.jlsjyb.cn

C#:   string.Join(", ", list)
来源：http://mjo.redwolf501.top

================================================================================
来源：http://daa.mhx1999.top

E. 字符串处理
来源：http://lzw.316326.xyz

================================================================================
来源：http://sfy.zhongyouzk.top

[E01] 拼接字符串
来源：http://jxv.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tzs.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pfj.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xcl.yfazqb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qdh.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://auy.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qnd.zhengqikj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://btt.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zta.yj20258.top

[E02] 重复字符串
来源：http://xfv.sxryk.cn

Py:   "ab" * 3
来源：http://zic.9152youxi.cn

PHP:  str_repeat("ab", 3);
来源：http://jof.sysykeji.top

JS:   "ab".repeat(3)
来源：http://efr.yuxming.cn

TS:   "ab".repeat(3)
来源：http://ois.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://sci.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://oxo.yj202588.top

Ruby: "ab" * 3
来源：http://zgt.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qkg.shzxlz.cn

[E03] 截取子串
来源：http://ywu.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mdc.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rbt.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qwn.kuanghao11.cn

TS:   s.slice(1, 4)
来源：http://zfv.bbcook.cn

Java: s.substring(1, 4)
来源：http://beb.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://erf.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://aaf.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://guq.zhiwuduotai.top

[E04] 查找子串位置
来源：http://xnd.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://bzy.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://zdc.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cln.jianghu66.top

TS:   s.indexOf("x")
来源：http://ukl.hfpthk.cn

Java: s.indexOf("x")
来源：http://ttq.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://yfw.9152youxi.cn

Ruby: s.index("x")
来源：http://jwb.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://drq.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bvh.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wur.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hse.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qow.daxiang520.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lae.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nob.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mar.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mpy.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pen.redwolf501.top

[E06] 替换子串
来源：http://ein.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ple.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://mnr.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovz.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://rtq.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hpu.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cuh.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xyr.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://qyg.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://otd.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://akg.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jcj.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tzx.jinqigfzy.top

TS:   s.split(",")
来源：http://flv.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qkx.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fuk.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://jym.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cfw.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://plx.dashuyun.cn

Py:   ",".join(items)
来源：http://ifz.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://wkh.hysaishi.cn

JS:   items.join(",")
来源：http://rjc.fanxiaobao.xyz

TS:   items.join(",")
来源：http://cus.sjlbkw.cn

Java: String.join(",", items)
来源：http://xmj.cashguo.top

Go:   strings.Join(items, ",")
来源：http://fft.xylfe.cn

Ruby: items.join(",")
来源：http://qgk.meibo888.top

C#:   string.Join(",", items)
来源：http://qny.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://jwh.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gjt.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jak.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://loc.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://fwh.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://rer.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qng.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://sow.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://phi.vqdsnc.cn

[E10] 左侧补零 / 定长填充
来源：http://zwm.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cvi.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://drn.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://fbc.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://zkb.jqgfzy.top

Java: String.format("%03d", 7)
来源：http://xpi.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://iqo.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://llh.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xfl.tian-w.cn

[E11] 反转字符串
来源：http://geq.yuxming.cn

Py:   s[::-1]
来源：http://usy.ydzc1.top

PHP:  strrev($s);
来源：http://bjy.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://lke.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://xfi.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://syk.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qjd.gotoacloud.top

Ruby: s.reverse
来源：http://bch.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://pjc.yj20258888.top

[E12] 统计某字符出现次数
来源：http://hlt.ydzc1.top

Py:   s.count("a")
来源：http://vbq.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://vzu.andypj.xyz

JS:   s.split("a").length - 1
来源：http://dni.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://qec.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://twr.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://zjn.snrcjt.cn

Ruby: s.count("a")
来源：http://ifr.ppjwa.cn

C#:   s.Count(c => c == 'a')
来源：http://dxx.pycfn.com

[E13] 逐字符遍历
来源：http://zoi.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://wqz.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mda.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fqi.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yue.shuidangran.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oyn.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vah.fzhhl.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bea.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rrd.guowangkeji.top

[E14] URL 编码与 Base64
来源：http://ele.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://btk.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fhm.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vwx.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jjg.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vuh.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cwc.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fdm.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dck.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://yaj.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eew.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://atc.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bdc.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wxw.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ohv.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ntr.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rdd.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pzd.cdnleiting.top

[E16] 数字千分位
来源：http://hds.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://ohm.epnwcf.com

PHP:  number_format(1234567);
来源：http://mqd.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://uvu.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kai.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bal.zycfv.cn


<!-- 参考信息 -->