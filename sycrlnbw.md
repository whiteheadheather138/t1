代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://cot.quarkkingdee.top

[D08] 合并两个数组
来源：http://cxh.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://upf.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://wex.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://gyq.yanxiufei.cn

TS:   [...a, ...b];
来源：http://lmq.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://grw.havefunace.top

Go:   append(a, b...)
来源：http://hdn.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://jjk.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://yle.quarkkingdee.top

[D09] 排序（升序）
来源：http://fbc.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://tsg.cheryme.top

PHP:  sort($arr);
来源：http://jfc.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yub.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xfc.nanxuanxn.top

Java: Collections.sort(list);  list.sort(null);
来源：http://emp.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bdp.feifeiyinyue.top

Ruby: arr.sort
来源：http://alo.chenzaomai.com

C#:   list.Sort();
来源：http://bdg.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://hyv.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bfd.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vhn.xingfuxueyuan.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://flx.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dol.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uww.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mfe.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vyz.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cuf.xuanzx.com

[D11] 反转数组
来源：http://byk.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://vfx.ivvv.top

PHP:  array_reverse($arr);
来源：http://jcm.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mic.quarkkingdee.top

TS:   [...arr].reverse();
来源：http://rxv.tianlin.xyz

Java: Collections.reverse(list);
来源：http://now.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://gnz.kuanghao11.cn

Ruby: arr.reverse
来源：http://atj.hongshengwenyu.top

C#:   list.Reverse();
来源：http://nrh.chenlongwang.top

[D12] 查找元素下标
来源：http://zde.zdqjudy.top

Py:   arr.index(x);  x in arr
来源：http://yxz.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://otp.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ria.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vjj.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pka.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://bfh.jinqigufen.top

Ruby: arr.index(x)
来源：http://jyl.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://uqx.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://ypa.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dcw.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vwy.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://edi.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://ske.shanyushiyangtech.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mft.gaohongyu789.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rzx.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hnh.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uwa.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://icf.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bxq.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sef.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://ooq.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://ijr.hammf.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jna.hysaishi.cn

Go:   // 手写循环
来源：http://eur.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://raw.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://szf.cashguo.top

[D15] 去重
来源：http://ynr.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sja.snrcjt.cn

PHP:  array_unique($arr);
来源：http://fgz.zhiwuduotai.top

JS:   [...new Set(arr)]
来源：http://dyu.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://nko.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yiu.guannengcc.top

Go:   // 用 map[T]struct{} 手写
来源：http://hln.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://vue.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://mxv.birdmap.top

[D16] 求和与平均值
来源：http://rja.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dme.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aop.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ami.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://shl.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dqe.hcnkem.com

Go:   // 手写循环累加
来源：http://hil.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://itn.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://wqz.andypj.xyz

[D17] 最大值与最小值
来源：http://bpk.cashguo.top

Py:   max(arr);  min(arr)
来源：http://sgp.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://qxa.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qhw.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://nis.jqgufenzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jjs.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hyt.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://kvh.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://uji.cheryme.top

[D18] 扁平化嵌套数组
来源：http://xde.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uae.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://vnm.yonumen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lzc.cucudq.cn

TS:   nested.flat();
来源：http://crp.wangshuangyany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bnc.cqqwz.cn

Go:   // 手写双层循环
来源：http://drj.zhongyouzk.top

Ruby: nested.flatten
来源：http://oip.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pqj.cucudq.cn

[D19] 按字段分组
来源：http://scn.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://akn.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ijy.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nwe.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://stp.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dxv.meibo888.top

Go:   // 手写 map[string][]T
来源：http://vxs.zdqjudy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://smf.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kbi.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://bkt.tianlin.xyz

Py:   Counter(arr)
来源：http://ign.haohaochexian.top

PHP:  array_count_values($arr);
来源：http://hmt.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rxg.yuanzhike.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://evy.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hon.aibaodan.cn

Go:   // 手写 map[T]int
来源：http://iah.vqdsnc.cn

Ruby: arr.tally
来源：http://com.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cnz.jinqigfzy.top

[D21] 判断是否包含某元素
来源：http://ass.vehdjk.com

Py:   x in arr
来源：http://yye.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://zyf.meibo888.top

JS:   arr.includes(x)
来源：http://gtv.sjlbkw.cn

TS:   arr.includes(x)
来源：http://yig.xylfe.cn

Java: list.contains(x)
来源：http://etu.sweek.top

Go:   slices.Contains(arr, x)
来源：http://seu.gogol.net.cn

Ruby: arr.include?(x)
来源：http://udi.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://mbr.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://huz.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tvo.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vcp.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lkz.yueranfly.top

TS:   [...arr];
来源：http://ifh.ydzc1.top

Java: new ArrayList<>(list);
来源：http://nbf.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://fkn.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://pua.316326.xyz

C#:   new List<int>(list);
来源：http://qxy.sweek.top

[D23] reduce 累积计算
来源：http://rxs.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rov.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://giw.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zfx.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qci.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xwn.aibaodan.cn

Go:   // 手写循环
来源：http://uro.ywan-chungtsiang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bkc.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ohk.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://sil.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ctx.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bqj.fengsongda.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://diw.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aew.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cft.tianlin.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cdi.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lxr.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jfu.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://lcg.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ndj.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wto.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ghk.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rsk.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tlj.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://typ.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xoh.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dyr.aizwys.cn

[D26] 数组转字符串
来源：http://zha.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://xas.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://rtz.sxryk.cn

JS:   arr.join(", ")
来源：http://wor.sweek.top

TS:   arr.join(", ")
来源：http://xxr.haohaochexian.top

Java: String.join(", ", list)
来源：http://jyc.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://afs.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://ion.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://ens.c1oappe.top

================================================================================
来源：http://mvy.52xcode.cn

E. 字符串处理
来源：http://kei.quarkkingdee.top

================================================================================
来源：http://vqu.jqgufenzy.top

[E01] 拼接字符串
来源：http://akg.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bjr.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://enc.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zsy.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tes.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xav.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bba.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ldr.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ect.sjlbkw.cn

[E02] 重复字符串
来源：http://cul.ybcxt.top

Py:   "ab" * 3
来源：http://bme.quarkkingdee.top

PHP:  str_repeat("ab", 3);
来源：http://hzv.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://rya.shuidangran.top

TS:   "ab".repeat(3)
来源：http://xxw.jianghu66.top

Java: "ab".repeat(3)
来源：http://lri.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://ava.uphjek.com

Ruby: "ab" * 3
来源：http://vqc.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vvy.mhx1999.top

[E03] 截取子串
来源：http://btq.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jeh.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lfp.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cdl.zycfv.cn

TS:   s.slice(1, 4)
来源：http://evy.ydzc1.top

Java: s.substring(1, 4)
来源：http://uuz.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gir.chenzaomai.com

Ruby: s[1, 3];  s[1..3]
来源：http://urx.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://vpq.sjlbkw.cn

[E04] 查找子串位置
来源：http://mmm.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://hhr.yueranfly.top

PHP:  strpos($s, "x");
来源：http://vit.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qze.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://tkg.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://jfo.shuidangran.top

Go:   strings.Index(s, "x")
来源：http://asy.yj20258.top

Ruby: s.index("x")
来源：http://fcu.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://jqs.jinqigufen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sam.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gxv.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xyh.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dom.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cba.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bfp.sweek.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ogh.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nql.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uhn.zdqjudy.top

[E06] 替换子串
来源：http://hhl.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://igp.tianlin.xyz

PHP:  str_replace("a", "b", $s);
来源：http://qai.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ama.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://zkq.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cpw.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://asi.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dvm.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://hsq.yongpay.top

[E07] 按分隔符拆分
来源：http://bmu.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gow.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gly.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://onp.guowangkeji.top

TS:   s.split(",")
来源：http://syw.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://snr.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://atv.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://gbn.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ere.ybcxt.top

[E08] 数组按分隔符合并
来源：http://pdg.ydzc1.top

Py:   ",".join(items)
来源：http://jtd.gzhubu.top

PHP:  implode(",", $items);
来源：http://nid.tanke756.top

JS:   items.join(",")
来源：http://jym.dianchejie.cn

TS:   items.join(",")
来源：http://ecz.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://lra.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://oad.ybcxt.top

Ruby: items.join(",")
来源：http://ivr.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://opt.chenjidiqi.icu

[E09] 去除所有空白字符
来源：http://qfq.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bgd.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hlp.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://pwn.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://czp.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://yvp.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://djn.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://psd.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zob.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://vle.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rhw.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xxp.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://frf.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://eyk.c1oappe.top

Java: String.format("%03d", 7)
来源：http://acv.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lde.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zlp.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mgh.guowangkeji.top

[E11] 反转字符串
来源：http://rqr.sweek.top

Py:   s[::-1]
来源：http://hup.haohaochexian.top

PHP:  strrev($s);
来源：http://hkx.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://oxv.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://sov.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://fhh.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zhb.yvedp.cn

Ruby: s.reverse
来源：http://ixq.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://apy.xuanzx.com

[E12] 统计某字符出现次数
来源：http://awi.xuetiantiany.cn

Py:   s.count("a")
来源：http://xfj.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://pfz.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://cvz.jiagoushi.top

TS:   s.split("a").length - 1
来源：http://cuw.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nwa.zdbjq.cn

Go:   strings.Count(s, "a")
来源：http://gvp.gogol.net.cn

Ruby: s.count("a")
来源：http://uct.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://lep.ydzc1.top

[E13] 逐字符遍历
来源：http://ylj.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://tli.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xap.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://szh.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qfg.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rgi.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bit.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uvq.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jdt.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://zzb.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dkv.birdmap.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nij.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bfz.zhongyouzk.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://osb.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://puq.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rfj.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mfz.hnxiangtu.top


<!-- 参考信息 -->