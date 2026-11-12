代发 wailian999

[D11] 反转数组
来源：http://bdx.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ukc.316326.xyz

PHP:  array_reverse($arr);
来源：http://nff.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qha.jyoumei.cn

TS:   [...arr].reverse();
来源：http://kxq.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://qpb.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://hxg.jqgufenzy.top

Ruby: arr.reverse
来源：http://bvh.jqgufenzy.top

C#:   list.Reverse();
来源：http://xqq.0kj1m.cn

[D12] 查找元素下标
来源：http://ugu.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://gxm.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zzp.xylfe.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nrm.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wam.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://edm.guowangkeji.top

Go:   slices.Index(arr, x)
来源：http://dkg.andypj.xyz

Ruby: arr.index(x)
来源：http://sno.0kj1m.cn

C#:   list.IndexOf(x);
来源：http://iob.vehdjk.com

[D13] 过滤（保留满足条件的）
来源：http://nav.fzhhl.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yfj.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qlj.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://ltg.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://jcc.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vfm.zdqjudy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hsb.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://juw.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://riq.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://xxo.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gkx.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://epe.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://uld.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://lkx.ehwqpu.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://oju.yj202588.top

Go:   // 手写循环
来源：http://wnr.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wih.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yzr.9152youxi.cn

[D15] 去重
来源：http://fkc.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bdt.gogol.net.cn

PHP:  array_unique($arr);
来源：http://lcl.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://hzl.shanyushiyangtech.top

TS:   [...new Set(arr)]
来源：http://thu.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cbe.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://crg.vqdsnc.cn

Ruby: arr.uniq
来源：http://boh.birdmap.top

C#:   list.Distinct().ToList()
来源：http://fze.hnxiangtu.top

[D16] 求和与平均值
来源：http://tzi.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jxu.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://atc.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rud.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kgk.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bgb.dashuyun.cn

Go:   // 手写循环累加
来源：http://mtr.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lrl.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://pnd.haohaochexian.top

[D17] 最大值与最小值
来源：http://mtf.sxryk.cn

Py:   max(arr);  min(arr)
来源：http://mnh.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://zhv.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xal.hywenlv.cn

TS:   Math.max(...arr);
来源：http://ugr.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vkm.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zqc.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://ata.jiagoushi.top

C#:   list.Max();  list.Min()
来源：http://zkp.sxryk.cn

[D18] 扁平化嵌套数组
来源：http://sco.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jxi.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://lsn.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lml.jinghuilouyu.cn

TS:   nested.flat();
来源：http://vjv.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pym.zdqjudy.top

Go:   // 手写双层循环
来源：http://rdb.yongpay.top

Ruby: nested.flatten
来源：http://lne.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pvz.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://vnk.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hiz.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jnp.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ohh.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://aaf.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://skb.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://lfo.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kna.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gzw.c1oappe.top

[D20] 统计每个元素出现次数
来源：http://pco.hfpthk.cn

Py:   Counter(arr)
来源：http://xyg.c1oappe.top

PHP:  array_count_values($arr);
来源：http://yuk.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yab.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yjz.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://skn.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://mlz.jinghuilouyu.cn

Ruby: arr.tally
来源：http://ovv.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qfw.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://boi.zhijiandao.cn

Py:   x in arr
来源：http://cdj.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://aeo.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://tuy.zdqjudy.top

TS:   arr.includes(x)
来源：http://wpx.fzhhl.top

Java: list.contains(x)
来源：http://fpu.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://uwk.dianchejie.cn

Ruby: arr.include?(x)
来源：http://fpt.cashguo.top

C#:   list.Contains(x)
来源：http://opk.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://uwn.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cva.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cat.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aja.ybcxt.top

TS:   [...arr];
来源：http://jcf.uphjek.com

Java: new ArrayList<>(list);
来源：http://swu.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kdd.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://ice.yanxiufei.cn

C#:   new List<int>(list);
来源：http://zbt.hywenlv.cn

[D23] reduce 累积计算
来源：http://rdf.zhongyouzk.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lkv.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wwx.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://peh.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://grq.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://xey.shuidangran.top

Go:   // 手写循环
来源：http://gjk.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aad.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cot.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://apj.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vmb.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://crt.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iim.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ptc.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lvi.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://klr.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jfr.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fyp.316326.xyz

[D25] Set 集合去重与交并差
来源：http://afd.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ogw.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kny.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cva.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zpi.yj20258888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ecs.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wtn.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dnc.zycfv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ass.nanxuanxn.top

[D26] 数组转字符串
来源：http://anr.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://zwo.tarul.cn

PHP:  implode(", ", $arr);
来源：http://iva.hammf.cn

JS:   arr.join(", ")
来源：http://kcv.shuidangran.top

TS:   arr.join(", ")
来源：http://xts.yanxiufei.cn

Java: String.join(", ", list)
来源：http://dbq.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://ggw.havefunace.top

Ruby: arr.join(", ")
来源：http://hdz.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://dee.zhengqikj.top

================================================================================
来源：http://drn.gzhubu.top

E. 字符串处理
来源：http://rvq.fehbvm.com

================================================================================
来源：http://tji.zdqjudy.top

[E01] 拼接字符串
来源：http://hpf.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://okm.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jmu.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bjc.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://unx.hesvh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fpn.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uin.guowangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vaq.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://obj.tanke756.top

[E02] 重复字符串
来源：http://neb.xuanzx.com

Py:   "ab" * 3
来源：http://hci.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://stn.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://dbz.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://hol.zdqjudy.top

Java: "ab".repeat(3)
来源：http://tpx.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://dmo.bbcook.cn

Ruby: "ab" * 3
来源：http://qpd.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://emx.tian-w.cn

[E03] 截取子串
来源：http://twe.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kps.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dlt.shangyingyoupin.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xcv.guannengcc.top

TS:   s.slice(1, 4)
来源：http://rhy.zdbjq.cn

Java: s.substring(1, 4)
来源：http://jvl.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ats.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://rgo.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://zbj.hnxiangtu.top

[E04] 查找子串位置
来源：http://vxu.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://via.tanke756.top

PHP:  strpos($s, "x");
来源：http://xdf.dianchejie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mzh.yuanzhike.top

TS:   s.indexOf("x")
来源：http://aqx.guannengcc.top

Java: s.indexOf("x")
来源：http://giq.yongpay.top

Go:   strings.Index(s, "x")
来源：http://bcn.zhoulong.xyz

Ruby: s.index("x")
来源：http://sza.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://tea.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jhj.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xan.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ueg.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tbv.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://jlv.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uhp.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jdd.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tkr.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sni.sjlbkw.cn

[E06] 替换子串
来源：http://yvi.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jvb.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://asl.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xys.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://bpq.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dou.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cra.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bju.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://nyc.sxryk.cn

[E07] 按分隔符拆分
来源：http://ywd.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ggd.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://awb.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://tcd.sjlbkw.cn

TS:   s.split(",")
来源：http://fqs.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://ltn.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fny.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://vse.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sta.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://ktk.yanxiufei.cn

Py:   ",".join(items)
来源：http://iuo.jqgfzy.top

PHP:  implode(",", $items);
来源：http://cjz.zdqjudy.top

JS:   items.join(",")
来源：http://aul.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://bie.guannengcc.top

Java: String.join(",", items)
来源：http://tzy.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://fbr.redwolf501.top

Ruby: items.join(",")
来源：http://fht.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://wxz.ybcxt.top

[E09] 去除所有空白字符
来源：http://lft.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jzr.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jai.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://jtx.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://kdk.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://qsg.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://uzz.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://bcw.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pvs.vqdsnc.cn

[E10] 左侧补零 / 定长填充
来源：http://lmn.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://saa.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bbv.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://riq.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://kmt.ydzc1.top

Java: String.format("%03d", 7)
来源：http://shj.jinqigfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://quj.zhijiandao.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dqy.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cbj.sufxvd.cn

[E11] 反转字符串
来源：http://uww.daxiang520.top

Py:   s[::-1]
来源：http://tqp.aizwys.cn

PHP:  strrev($s);
来源：http://ohn.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://wqf.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://mic.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fih.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kzr.bbcook.cn

Ruby: s.reverse
来源：http://vde.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rpm.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://wru.haohaochexian.top

Py:   s.count("a")
来源：http://hau.ydjk.org.cn

PHP:  substr_count($s, "a");
来源：http://lpr.jqgfzy.top

JS:   s.split("a").length - 1
来源：http://wox.sweek.top

TS:   s.split("a").length - 1
来源：http://jel.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://whv.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://koy.ppjwa.cn

Ruby: s.count("a")
来源：http://alv.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://mso.dianchejie.cn

[E13] 逐字符遍历
来源：http://cto.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://xzc.hysaishi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xuj.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qix.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://ukx.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ebe.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wul.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://rpv.shanyushiyangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gtz.316326.xyz

[E14] URL 编码与 Base64
来源：http://jnn.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://opc.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://seu.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sdl.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pax.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://djz.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dnk.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oxy.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ilt.gogol.net.cn

[E15] HTML 转义 / 反转义
来源：http://ous.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://box.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bkv.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vqq.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gfa.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://okg.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ogn.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pmr.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ime.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://pqu.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://cvp.52xcode.cn

PHP:  number_format(1234567);
来源：http://gph.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://emv.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oij.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ibb.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ugh.hysaishi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://thn.hfpthk.cn

C#:   1234567.ToString("N0")
来源：http://shu.hysaishi.cn

[E17] 首字母大写
来源：http://zgc.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qqy.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://afm.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eju.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qum.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nzp.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hws.c1oappe.top

Ruby: s.capitalize
来源：http://cwz.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rgt.zdqjudy.top


<!-- 参考信息 -->