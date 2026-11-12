代发 wailian999

PHP:  sort($arr);
来源：http://hci.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eot.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mec.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ajy.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mui.0kj1m.cn

Ruby: arr.sort
来源：http://quz.hnqzz.top

C#:   list.Sort();
来源：http://vjb.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uyp.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wru.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cxr.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qgq.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vtd.bjfxy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://afs.yuxming.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://grw.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wgl.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eix.yj202588.top

[D11] 反转数组
来源：http://wef.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://ieu.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://wrj.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ykv.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://oei.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://ple.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://wnt.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://kne.andypj.xyz

C#:   list.Reverse();
来源：http://lhl.sjlbkw.cn

[D12] 查找元素下标
来源：http://ydn.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://xsm.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hma.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://szj.epnwcf.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iab.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uug.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://epa.cucudq.cn

Ruby: arr.index(x)
来源：http://nuv.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://wmt.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://sfa.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mfv.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://erp.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://uwi.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://edj.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pip.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fgd.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://osk.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tiq.hywenlv.cn

[D14] 映射转换（每个元素变形）
来源：http://ryp.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bxj.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zsq.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://vdo.jiagoushi.top

TS:   arr.map(x => x * 2)
来源：http://won.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pxt.hongshengwenyu.top

Go:   // 手写循环
来源：http://xge.hcnkem.com

Ruby: arr.map { |x| x * 2 }
来源：http://rbb.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://xik.jiagoushi.top

[D15] 去重
来源：http://qil.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qex.ybcxt.top

PHP:  array_unique($arr);
来源：http://vwk.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://pof.wangdashe.top

TS:   [...new Set(arr)]
来源：http://mdn.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hcf.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://cyc.birdmap.top

Ruby: arr.uniq
来源：http://ird.snrcjt.cn

C#:   list.Distinct().ToList()
来源：http://ilm.shuidangran.top

[D16] 求和与平均值
来源：http://ldr.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rfv.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zbm.c1oappe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sar.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tji.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ttz.yuanzhike.top

Go:   // 手写循环累加
来源：http://rbr.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jxy.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://nre.zhixingplan.top

[D17] 最大值与最小值
来源：http://rii.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://xlj.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://dbv.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dqt.daxiang520.top

TS:   Math.max(...arr);
来源：http://kil.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://idl.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ywe.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://jlj.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://xpo.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://por.yuanzhike.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dve.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://xvv.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xrv.yuxming.cn

TS:   nested.flat();
来源：http://acq.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tqw.zdqjudy.top

Go:   // 手写双层循环
来源：http://mbo.haohaochexian.top

Ruby: nested.flatten
来源：http://tdk.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://uuc.gaohongyu789.top

[D19] 按字段分组
来源：http://paq.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ccc.0kj1m.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yrz.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wya.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qvx.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kwy.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://hsj.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hxk.ybcxt.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qat.yj20258.top

[D20] 统计每个元素出现次数
来源：http://qhf.bbcook.cn

Py:   Counter(arr)
来源：http://tkk.hammf.cn

PHP:  array_count_values($arr);
来源：http://pta.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wqi.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cua.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pnz.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://ojl.ybcxt.top

Ruby: arr.tally
来源：http://cja.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qrs.bbcook.cn

[D21] 判断是否包含某元素
来源：http://cgl.nwbrower.top

Py:   x in arr
来源：http://qyt.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://hhf.jinqigfzy.top

JS:   arr.includes(x)
来源：http://ros.nanxuanxn.top

TS:   arr.includes(x)
来源：http://dxw.yuanzhike.top

Java: list.contains(x)
来源：http://psr.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://mvj.yvedp.cn

Ruby: arr.include?(x)
来源：http://yux.meibo888.top

C#:   list.Contains(x)
来源：http://kak.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://qhg.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xur.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hyx.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://esj.cqqwz.cn

TS:   [...arr];
来源：http://yjc.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://rzw.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rga.hnqzz.top

Ruby: arr.dup;  arr.clone
来源：http://ucg.iojbl.cn

C#:   new List<int>(list);
来源：http://auf.52xcode.cn

[D23] reduce 累积计算
来源：http://awo.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fqe.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xxb.bbcook.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://idh.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vzq.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jsu.vqdsnc.cn

Go:   // 手写循环
来源：http://iwh.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kyl.zhijiandao.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zja.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://nto.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mdj.meibo888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uty.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dlt.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tvn.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lep.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://apf.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cxn.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gkg.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://wfe.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ctv.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zdi.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jik.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://izd.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://apz.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://owe.hesvh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gbq.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fzg.yfazqb.com

[D26] 数组转字符串
来源：http://huh.ivvv.top

Py:   ", ".join(map(str, arr))
来源：http://iwf.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://xyp.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://yln.vehdjk.com

TS:   arr.join(", ")
来源：http://dyj.hfpthk.cn

Java: String.join(", ", list)
来源：http://wtl.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://pdi.iojbl.cn

Ruby: arr.join(", ")
来源：http://ovm.daxiang520.top

C#:   string.Join(", ", list)
来源：http://uwg.yj202588.top

================================================================================
来源：http://swl.xuetiantiany.cn

E. 字符串处理
来源：http://ipu.hnqzz.top

================================================================================
来源：http://nhr.wangshuangyany.cn

[E01] 拼接字符串
来源：http://xux.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cup.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wms.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cre.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aul.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mka.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://msx.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://euu.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nut.jlsjyb.cn

[E02] 重复字符串
来源：http://wwr.cashguo.top

Py:   "ab" * 3
来源：http://kru.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://srn.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://czz.birdmap.top

TS:   "ab".repeat(3)
来源：http://kit.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://art.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://ibm.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://din.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xfv.hammf.cn

[E03] 截取子串
来源：http://qzq.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wwl.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mpg.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qrt.sysykeji.top

TS:   s.slice(1, 4)
来源：http://lge.hfpthk.cn

Java: s.substring(1, 4)
来源：http://ucq.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iwc.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://xuu.jlsjyb.cn

C#:   s.Substring(1, 3)
来源：http://sxe.yj202588.top

[E04] 查找子串位置
来源：http://aff.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://mgp.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://sax.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bxn.c1oappe.top

TS:   s.indexOf("x")
来源：http://mem.xuanzx.com

Java: s.indexOf("x")
来源：http://hmx.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://ovj.yj20258.top

Ruby: s.index("x")
来源：http://qxk.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://ygc.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://whm.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ayl.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://npw.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fdg.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://oun.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bcy.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rdn.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mof.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vjj.chenjidiqi.icu

[E06] 替换子串
来源：http://ptw.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pdo.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://baq.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qzr.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://tce.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fgy.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yby.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ajb.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://zul.cucudq.cn

[E07] 按分隔符拆分
来源：http://tdz.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oqv.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rcf.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qfw.chenjidiqi.icu

TS:   s.split(",")
来源：http://ryu.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://rty.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hre.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://wwj.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oeh.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://ten.bbcook.cn

Py:   ",".join(items)
来源：http://ajm.mhx1999.top

PHP:  implode(",", $items);
来源：http://svp.meibo888.top

JS:   items.join(",")
来源：http://tol.ehwqpu.com

TS:   items.join(",")
来源：http://wdl.xylfe.cn

Java: String.join(",", items)
来源：http://tis.birdmap.top

Go:   strings.Join(items, ",")
来源：http://orv.hammf.cn

Ruby: items.join(",")
来源：http://hva.uphjek.com

C#:   string.Join(",", items)
来源：http://sse.smart0.xyz

[E09] 去除所有空白字符
来源：http://kqw.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://egf.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://egi.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://pqx.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://gle.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://hgs.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://yhc.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://fym.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://med.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://icb.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gnc.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tbx.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://njo.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://xrw.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://dai.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nao.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pug.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ome.shzxlz.cn

[E11] 反转字符串
来源：http://edy.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://vqo.fanxiaobao.xyz

PHP:  strrev($s);
来源：http://ptt.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://was.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://qun.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://taw.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zgy.hongshengwenyu.top

Ruby: s.reverse
来源：http://nac.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://phj.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://mem.xinyue.icu

Py:   s.count("a")
来源：http://mfl.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://qln.zhengqikj.top

JS:   s.split("a").length - 1
来源：http://huq.52xcode.cn

TS:   s.split("a").length - 1
来源：http://ecd.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hdh.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://suj.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://sxy.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://geq.gaohongyu789.top

[E13] 逐字符遍历
来源：http://roh.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://zyp.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rmf.hysaishi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://usy.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wrz.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pjk.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bkq.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iao.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://feq.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://njd.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dfo.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qhg.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wjx.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mmi.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bss.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vhz.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zrq.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xww.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://ghf.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ksn.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://slm.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gmp.cqqwz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aiy.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ycq.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ano.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dtm.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rbf.tianlin.xyz

[E16] 数字千分位
来源：http://shh.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://aci.havefunace.top


<!-- 参考信息 -->