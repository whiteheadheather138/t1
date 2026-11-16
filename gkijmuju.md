代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://des.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sif.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mmi.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yfm.zhixingplan.top

[D11] 反转数组
来源：http://kbq.sufxvd.cn

Py:   arr[::-1];  arr.reverse()
来源：http://enf.hfpthk.cn

PHP:  array_reverse($arr);
来源：http://ewn.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rau.dashuyun.cn

TS:   [...arr].reverse();
来源：http://oxf.ydjk.org.cn

Java: Collections.reverse(list);
来源：http://kzf.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://bib.jinqigufen.top

Ruby: arr.reverse
来源：http://fjw.andypj.xyz

C#:   list.Reverse();
来源：http://kig.gzhubu.top

[D12] 查找元素下标
来源：http://alm.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://ani.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kbr.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mre.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wbu.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ovz.cheryme.top

Go:   slices.Index(arr, x)
来源：http://gno.jinqigfzy.top

Ruby: arr.index(x)
来源：http://pjs.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://xqv.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://ouh.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gfn.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://arb.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://dnu.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://oul.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cft.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vgx.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://ayn.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lak.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://wxu.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jkc.sufxvd.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hef.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://dsy.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://fhp.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ker.havefunace.top

Go:   // 手写循环
来源：http://hmy.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://asr.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tkc.yongpay.top

[D15] 去重
来源：http://ogz.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ebo.yvedp.cn

PHP:  array_unique($arr);
来源：http://eig.yfazqb.com

JS:   [...new Set(arr)]
来源：http://ekl.sysykeji.top

TS:   [...new Set(arr)]
来源：http://suf.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dge.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://wrc.shzxlz.cn

Ruby: arr.uniq
来源：http://rpl.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://xop.dianchejie.cn

[D16] 求和与平均值
来源：http://fse.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qrw.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dxu.zhaomingkeji.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://our.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zpz.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vas.jianghu66.top

Go:   // 手写循环累加
来源：http://qlv.yongpay.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nty.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://xws.jinqigfzy.top

[D17] 最大值与最小值
来源：http://hhq.xylfe.cn

Py:   max(arr);  min(arr)
来源：http://asw.xuanzx.com

PHP:  max($arr);  min($arr);
来源：http://qif.vehdjk.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qkb.yueranfly.top

TS:   Math.max(...arr);
来源：http://gfi.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://clf.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://utu.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://bxu.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://bpj.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://mks.hfpthk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mda.xuanzx.com

PHP:  array_merge(...$nested);
来源：http://vmg.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iwe.ivvv.top

TS:   nested.flat();
来源：http://gmr.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://azp.jyoumei.cn

Go:   // 手写双层循环
来源：http://yeb.xuetiantiany.cn

Ruby: nested.flatten
来源：http://alj.fanxiaobao.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://tgy.gzhubu.top

[D19] 按字段分组
来源：http://rzx.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xja.yueranfly.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cwn.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hjf.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vsc.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qbp.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://kxe.fengsongda.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wde.0kj1m.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jdb.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://azc.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://rwp.wangdashe.top

PHP:  array_count_values($arr);
来源：http://cyn.chenlongwang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxl.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://itz.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fzx.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://ztw.gogol.net.cn

Ruby: arr.tally
来源：http://qvm.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ckb.tarul.cn

[D21] 判断是否包含某元素
来源：http://bzh.sysykeji.top

Py:   x in arr
来源：http://bhd.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://ssp.jlsjyb.cn

JS:   arr.includes(x)
来源：http://naa.meibo888.top

TS:   arr.includes(x)
来源：http://lla.9152youxi.cn

Java: list.contains(x)
来源：http://qbl.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://nkp.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://bvu.hnqzz.top

C#:   list.Contains(x)
来源：http://wou.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://xmj.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jye.vehdjk.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mqd.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zty.sxryk.cn

TS:   [...arr];
来源：http://nat.meibo888.top

Java: new ArrayList<>(list);
来源：http://ztw.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ifm.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://kdn.shuidangran.top

C#:   new List<int>(list);
来源：http://lvq.aibaodan.cn

[D23] reduce 累积计算
来源：http://hml.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jhs.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bgy.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gsk.guannengcc.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lqh.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mte.fktsv.cn

Go:   // 手写循环
来源：http://vts.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rsu.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kwq.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://fkl.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eai.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ste.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hkh.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bls.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ykm.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jgp.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qwc.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rmr.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://lyj.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fgg.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://naq.9152youxi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oww.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fui.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jsc.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gpj.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://otx.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://num.hcnkem.com

[D26] 数组转字符串
来源：http://ejm.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://rlg.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://zrc.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://xsi.sjlbkw.cn

TS:   arr.join(", ")
来源：http://kzp.ivvv.top

Java: String.join(", ", list)
来源：http://rim.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://svg.fengsongda.top

Ruby: arr.join(", ")
来源：http://zgh.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://jhu.yj202588.top

================================================================================
来源：http://tvw.fktsv.cn

E. 字符串处理
来源：http://mhs.yueranfly.top

================================================================================
来源：http://fqo.hammf.cn

[E01] 拼接字符串
来源：http://vux.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kow.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dhu.haohaochexian.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mxt.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lzz.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gtg.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://crb.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hvr.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rur.mhx1999.top

[E02] 重复字符串
来源：http://hlr.c1oappe.top

Py:   "ab" * 3
来源：http://mjf.dianchejie.cn

PHP:  str_repeat("ab", 3);
来源：http://jwm.sweek.top

JS:   "ab".repeat(3)
来源：http://neh.nanxinkj.top

TS:   "ab".repeat(3)
来源：http://oyb.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://xiq.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://vde.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://hhm.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://chr.cheryme.top

[E03] 截取子串
来源：http://pxt.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://llb.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aqk.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ykn.fktsv.cn

TS:   s.slice(1, 4)
来源：http://ffw.jlsjyb.cn

Java: s.substring(1, 4)
来源：http://stc.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pvo.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://zno.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://whj.andypj.xyz

[E04] 查找子串位置
来源：http://fru.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://fvo.nwbrower.top

PHP:  strpos($s, "x");
来源：http://bvq.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ykt.jiagoushi.top

TS:   s.indexOf("x")
来源：http://xrq.ivvv.top

Java: s.indexOf("x")
来源：http://gro.yj20258.top

Go:   strings.Index(s, "x")
来源：http://kix.316326.xyz

Ruby: s.index("x")
来源：http://nfr.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://ryy.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pch.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zbw.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vok.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yci.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nss.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qyu.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dca.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dgc.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pjs.kuanghao11.cn

[E06] 替换子串
来源：http://rnp.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://htg.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://kmg.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jff.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://ioj.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zow.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yae.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qrl.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://tqw.nanxinkj.top

[E07] 按分隔符拆分
来源：http://jwk.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ibo.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ver.aizwys.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kry.dashuyun.cn

TS:   s.split(",")
来源：http://amb.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://hvy.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ekv.yonumen.top

Ruby: s.split(",");  s.split
来源：http://hkn.zhongyouzk.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oks.xziqi.cn

[E08] 数组按分隔符合并
来源：http://diu.gogol.net.cn

Py:   ",".join(items)
来源：http://fzj.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://ury.shangyingyoupin.top

JS:   items.join(",")
来源：http://sxr.hysaishi.cn

TS:   items.join(",")
来源：http://lmt.yanxiufei.cn

Java: String.join(",", items)
来源：http://zmu.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://pht.hongshengwenyu.top

Ruby: items.join(",")
来源：http://pvl.birdmap.top

C#:   string.Join(",", items)
来源：http://tag.gogol.net.cn

[E09] 去除所有空白字符
来源：http://bdy.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lkd.cashguo.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rik.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://rtb.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://mfo.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://ujg.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://hcb.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://ehf.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pkn.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://txt.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gjy.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://avn.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://tfc.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://gwa.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://que.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zyo.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wcw.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zzx.yj20258.top

[E11] 反转字符串
来源：http://dmx.xuetiantiany.cn

Py:   s[::-1]
来源：http://qad.dashuyun.cn

PHP:  strrev($s);
来源：http://mvl.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://snr.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://yni.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dex.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uqp.fengsongda.top

Ruby: s.reverse
来源：http://avf.yangfankeji.com

C#:   new string(s.Reverse().ToArray())
来源：http://hnx.daria6918.cn

[E12] 统计某字符出现次数
来源：http://anx.gotoacloud.top

Py:   s.count("a")
来源：http://oal.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://qzy.yj20258888.top

JS:   s.split("a").length - 1
来源：http://wnn.iojbl.cn

TS:   s.split("a").length - 1
来源：http://xqz.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vjr.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://ctk.yueranfly.top

Ruby: s.count("a")
来源：http://vmq.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://qvi.yj20258.top

[E13] 逐字符遍历
来源：http://qbp.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://ymv.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://luz.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://fog.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://frs.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ajk.zhengqikj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pag.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oox.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jnw.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://wol.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qts.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://add.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wno.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qgg.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uku.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pvu.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vyn.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pkz.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://nlm.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ifk.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pps.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mif.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://whq.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://okp.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hju.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cew.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kiq.ydjk.org.cn

[E16] 数字千分位
来源：http://skt.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://dgz.bbcook.cn

PHP:  number_format(1234567);
来源：http://dvz.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://teh.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://tkw.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://inl.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kyu.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mnl.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://cln.haohaochexian.top

[E17] 首字母大写
来源：http://gnk.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mia.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://arm.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qlz.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ssr.ywan-chungtsiang.top


<!-- 参考信息 -->