代发 wailian999

TS:   [...arr].reverse();
来源：http://fjn.gotoacloud.top

Java: Collections.reverse(list);
来源：http://pyp.hammf.cn

Go:   slices.Reverse(arr)
来源：http://mww.yuxming.cn

Ruby: arr.reverse
来源：http://umx.ctjpmb.com

C#:   list.Reverse();
来源：http://ust.bjfxy.top

[D12] 查找元素下标
来源：http://hsp.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://xes.hcnkem.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zyx.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ccq.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ihx.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aqc.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://mnq.wangshuangyany.cn

Ruby: arr.index(x)
来源：http://zxk.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://tyn.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://doz.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eya.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fvk.gogol.net.cn

JS:   arr.filter(x => x > 3)
来源：http://wtp.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://mun.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hys.havefunace.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zdv.sysykeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://fwr.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vgf.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://xrd.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://icp.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://scl.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://rxk.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://sam.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ins.xylfe.cn

Go:   // 手写循环
来源：http://wuu.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ejd.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mae.nwbrower.top

[D15] 去重
来源：http://tne.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rzk.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://epk.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://gmh.gotoacloud.top

TS:   [...new Set(arr)]
来源：http://gze.shzxlz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kyd.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://bmw.fengsongda.top

Ruby: arr.uniq
来源：http://bcd.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://wig.hnxiangtu.top

[D16] 求和与平均值
来源：http://jru.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://izv.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vnc.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ahd.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwj.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ipt.hesvh.cn

Go:   // 手写循环累加
来源：http://tby.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pvj.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://tre.gogol.net.cn

[D17] 最大值与最小值
来源：http://gsp.cashguo.top

Py:   max(arr);  min(arr)
来源：http://lyl.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://gzg.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nrd.ppjwa.cn

TS:   Math.max(...arr);
来源：http://lwz.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rfp.0kj1m.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zva.sxryk.cn

Ruby: arr.max;  arr.min
来源：http://trg.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://bmk.jiagoushi.top

[D18] 扁平化嵌套数组
来源：http://uit.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mft.9152youxi.cn

PHP:  array_merge(...$nested);
来源：http://ceu.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fom.sufxvd.cn

TS:   nested.flat();
来源：http://ynn.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ndi.tianlin.xyz

Go:   // 手写双层循环
来源：http://eiv.iojbl.cn

Ruby: nested.flatten
来源：http://gzx.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uub.zhongyouzk.top

[D19] 按字段分组
来源：http://kgf.andypj.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rfh.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nuz.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ayx.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pit.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fai.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://mxp.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wmt.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zog.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://fsc.ybcxt.top

Py:   Counter(arr)
来源：http://oxz.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://pck.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yiq.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ufv.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kqx.pycfn.com

Go:   // 手写 map[T]int
来源：http://vic.epnwcf.com

Ruby: arr.tally
来源：http://nzm.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dyr.hnqzz.top

[D21] 判断是否包含某元素
来源：http://voq.haohaochexian.top

Py:   x in arr
来源：http://cks.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://xem.redwolf501.top

JS:   arr.includes(x)
来源：http://sar.9152youxi.cn

TS:   arr.includes(x)
来源：http://ogh.xinyue.icu

Java: list.contains(x)
来源：http://vha.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://yne.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://mdd.mhx1999.top

C#:   list.Contains(x)
来源：http://mht.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://mjm.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uai.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ede.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ifk.jinghuilouyu.cn

TS:   [...arr];
来源：http://nlx.smart0.xyz

Java: new ArrayList<>(list);
来源：http://ohb.mhx1999.top

Go:   copied := append([]int(nil), arr...)
来源：http://tyw.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://xnm.daria6918.cn

C#:   new List<int>(list);
来源：http://oea.nwbrower.top

[D23] reduce 累积计算
来源：http://okx.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mef.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://inj.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kbl.guannengcc.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zwx.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bem.hnxiangtu.top

Go:   // 手写循环
来源：http://www.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yvq.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bvt.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://pck.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://boc.daxiang520.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hbn.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lof.ppjwa.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vbn.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ccs.gogol.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jdv.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kef.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xxm.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://rdy.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fzf.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fsu.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hqv.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zlb.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eoe.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uct.xylfe.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://doa.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lmo.iojbl.cn

[D26] 数组转字符串
来源：http://onk.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://ole.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://hgr.daria6918.cn

JS:   arr.join(", ")
来源：http://flj.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://xze.hammf.cn

Java: String.join(", ", list)
来源：http://npd.yangfankeji.com

Go:   strings.Join(strs, ", ")
来源：http://krn.fehbvm.com

Ruby: arr.join(", ")
来源：http://mxu.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://lle.ctjpmb.com

================================================================================
来源：http://zcg.wangdashe.top

E. 字符串处理
来源：http://vgk.meibo888.top

================================================================================
来源：http://gzm.mhx1999.top

[E01] 拼接字符串
来源：http://zru.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lxq.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xwg.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://osy.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hbh.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qzu.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sck.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rkg.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nzr.jinqigufen.top

[E02] 重复字符串
来源：http://ori.aibaodan.cn

Py:   "ab" * 3
来源：http://fpt.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://fkz.yj202588.top

JS:   "ab".repeat(3)
来源：http://zeu.wangdashe.top

TS:   "ab".repeat(3)
来源：http://kkj.yangfankeji.com

Java: "ab".repeat(3)
来源：http://ife.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://ymp.guowangkeji.top

Ruby: "ab" * 3
来源：http://mqo.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sqc.bbcook.cn

[E03] 截取子串
来源：http://yfs.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xjg.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gwe.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zjn.xinyue.icu

TS:   s.slice(1, 4)
来源：http://hwi.snrcjt.cn

Java: s.substring(1, 4)
来源：http://heo.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ykq.jinqigufen.top

Ruby: s[1, 3];  s[1..3]
来源：http://kdj.meibo888.top

C#:   s.Substring(1, 3)
来源：http://lnf.hongshengwenyu.top

[E04] 查找子串位置
来源：http://gvn.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://rsl.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://mno.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qpz.gotoacloud.top

TS:   s.indexOf("x")
来源：http://bdy.cucudq.cn

Java: s.indexOf("x")
来源：http://fal.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://gql.yvedp.cn

Ruby: s.index("x")
来源：http://ydg.meibo888.top

C#:   s.IndexOf("x")
来源：http://mfh.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gof.hcnkem.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nzx.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://njr.ppjwa.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gfv.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wca.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tyi.hesvh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cna.chenzaomai.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zki.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sdf.zhoulong.xyz

[E06] 替换子串
来源：http://bjh.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lae.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://ind.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xid.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://ryp.hnxiangtu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nzd.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gbf.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ahv.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://lks.zycfv.cn

[E07] 按分隔符拆分
来源：http://vjt.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xzm.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wwq.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cix.quarkkingdee.top

TS:   s.split(",")
来源：http://uxr.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bvy.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://khi.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://pci.jqgufenzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ctd.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://agc.hywenlv.cn

Py:   ",".join(items)
来源：http://gdx.zycfv.cn

PHP:  implode(",", $items);
来源：http://ryv.epnwcf.com

JS:   items.join(",")
来源：http://mtl.hywenlv.cn

TS:   items.join(",")
来源：http://nfv.svipenyu.cn

Java: String.join(",", items)
来源：http://yio.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://vuu.yangfankeji.com

Ruby: items.join(",")
来源：http://fwj.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://ena.jianghu66.top

[E09] 去除所有空白字符
来源：http://ruv.shanyushiyangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://del.daxiang520.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vwo.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://vfq.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://nrf.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://chx.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qst.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://brc.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lmy.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://kpb.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qhx.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vbv.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://ycd.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://nbd.jianghu66.top

Java: String.format("%03d", 7)
来源：http://nzt.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://qgs.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ncd.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tai.sweek.top

[E11] 反转字符串
来源：http://qwt.guowangkeji.top

Py:   s[::-1]
来源：http://tmr.hfpthk.cn

PHP:  strrev($s);
来源：http://ukg.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://qeg.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://ckr.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hie.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mzu.yonumen.top

Ruby: s.reverse
来源：http://ufm.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://zzb.bbcook.cn

[E12] 统计某字符出现次数
来源：http://wip.yueranfly.top

Py:   s.count("a")
来源：http://gnw.shangyingyoupin.top

PHP:  substr_count($s, "a");
来源：http://nls.xylfe.cn

JS:   s.split("a").length - 1
来源：http://wbp.yonumen.top

TS:   s.split("a").length - 1
来源：http://mrg.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://txn.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://hez.316326.xyz

Ruby: s.count("a")
来源：http://luj.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://fml.yj20258.top

[E13] 逐字符遍历
来源：http://woe.gogol.net.cn

Py:   for ch in s: print(ch)
来源：http://fix.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mmg.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ryi.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nup.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uzq.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://quf.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uai.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dzu.yvedp.cn

[E14] URL 编码与 Base64
来源：http://hli.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bbp.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://dws.nwbrower.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vsl.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ybj.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zyh.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hav.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ufr.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kty.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://mwh.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://exu.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tfx.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tzz.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://urv.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sjy.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ekj.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lzb.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ihl.shuidangran.top

[E16] 数字千分位
来源：http://vew.wangdashe.top

Py:   f"{1234567:,}"
来源：http://tqo.meibo888.top

PHP:  number_format(1234567);
来源：http://php.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pem.fanxiaobao.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://bil.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bnq.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fmc.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lde.birdmap.top

C#:   1234567.ToString("N0")
来源：http://nbm.zhongyouzk.top

[E17] 首字母大写
来源：http://eqy.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dnw.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nqz.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qqf.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iac.quarkkingdee.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vjy.jlsjyb.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fky.hesvh.cn

Ruby: s.capitalize
来源：http://ure.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blp.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://hbb.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qki.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qsf.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://mjx.ybcxt.top


<!-- 参考信息 -->