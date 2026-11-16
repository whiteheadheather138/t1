代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hfq.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://opb.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hjn.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://axw.daria6918.cn

[D11] 反转数组
来源：http://tsg.jinqigfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://sgk.fktsv.cn

PHP:  array_reverse($arr);
来源：http://lki.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yzz.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://ycv.shuidangran.top

Java: Collections.reverse(list);
来源：http://bpr.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://oss.andypj.xyz

Ruby: arr.reverse
来源：http://hcq.daxiang520.top

C#:   list.Reverse();
来源：http://ari.pycfn.com

[D12] 查找元素下标
来源：http://feu.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://bho.hcnkem.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ddj.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mdp.ywan-chungtsiang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ret.fanxiaobao.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sqq.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://caj.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://gyx.bjfxy.top

C#:   list.IndexOf(x);
来源：http://dlv.yj20258.top

[D13] 过滤（保留满足条件的）
来源：http://wqf.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bxu.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://url.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://vnw.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://uvd.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vka.sweek.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rtp.aizwys.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ubh.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gku.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://trk.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mmw.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gyf.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://fmb.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://zoj.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://oiv.nwbrower.top

Go:   // 手写循环
来源：http://ztd.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pog.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ssz.fanxiaobao.xyz

[D15] 去重
来源：http://aio.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baq.mhx1999.top

PHP:  array_unique($arr);
来源：http://ipo.cucudq.cn

JS:   [...new Set(arr)]
来源：http://afg.52xcode.cn

TS:   [...new Set(arr)]
来源：http://vab.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cni.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ogg.bjfxy.top

Ruby: arr.uniq
来源：http://zlk.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://hzf.jqgufenzy.top

[D16] 求和与平均值
来源：http://iqw.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fmo.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tjf.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://npw.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wjn.zdbjq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hrb.smart0.xyz

Go:   // 手写循环累加
来源：http://yym.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ins.jlsjyb.cn

C#:   list.Sum();  list.Average()
来源：http://iqk.tanke756.top

[D17] 最大值与最小值
来源：http://ryi.xuetiantiany.cn

Py:   max(arr);  min(arr)
来源：http://xpa.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://rab.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kuj.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://dze.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uwr.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pxg.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://vvp.0kj1m.cn

C#:   list.Max();  list.Min()
来源：http://mte.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://ujh.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ziw.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://jzq.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://chi.guowangkeji.top

TS:   nested.flat();
来源：http://yvb.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rqt.hysaishi.cn

Go:   // 手写双层循环
来源：http://rdy.sysykeji.top

Ruby: nested.flatten
来源：http://rtd.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://oyk.xuetiantiany.cn

[D19] 按字段分组
来源：http://wln.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nrw.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bhu.yfazqb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ffx.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gyr.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tpz.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://dmu.xziqi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hig.tianlin.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tqe.sxryk.cn

[D20] 统计每个元素出现次数
来源：http://gco.yj202588.top

Py:   Counter(arr)
来源：http://ysb.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://gna.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tuu.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dhs.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://idh.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://ywi.hnxiangtu.top

Ruby: arr.tally
来源：http://ccp.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ave.nwbrower.top

[D21] 判断是否包含某元素
来源：http://arz.dianchejie.cn

Py:   x in arr
来源：http://yen.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://lfd.vqdsnc.cn

JS:   arr.includes(x)
来源：http://lbs.dianchejie.cn

TS:   arr.includes(x)
来源：http://tig.zdqjudy.top

Java: list.contains(x)
来源：http://kkl.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://oce.jinqigufen.top

Ruby: arr.include?(x)
来源：http://xkw.gotoacloud.top

C#:   list.Contains(x)
来源：http://phu.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://ikz.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kaa.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://noy.zycfv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mbq.bbcook.cn

TS:   [...arr];
来源：http://cve.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://qvk.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://cph.vqdsnc.cn

Ruby: arr.dup;  arr.clone
来源：http://cjz.jlsjyb.cn

C#:   new List<int>(list);
来源：http://mbf.vehdjk.com

[D23] reduce 累积计算
来源：http://age.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wid.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lpp.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eit.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gnb.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cqa.cdnleiting.top

Go:   // 手写循环
来源：http://yod.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uax.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://evy.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://ahv.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mth.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yal.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ylq.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rhj.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jrs.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iuh.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wae.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wuo.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://vio.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nab.gogol.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wts.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sbr.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://llz.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vbv.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nxc.sweek.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cuf.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hae.ivvv.top

[D26] 数组转字符串
来源：http://lwt.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://mkg.jiagoushi.top

PHP:  implode(", ", $arr);
来源：http://jls.yanxiufei.cn

JS:   arr.join(", ")
来源：http://ome.pycfn.com

TS:   arr.join(", ")
来源：http://vko.zhengqikj.top

Java: String.join(", ", list)
来源：http://jfa.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://him.smart0.xyz

Ruby: arr.join(", ")
来源：http://xjy.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://jsz.xziqi.cn

================================================================================
来源：http://ncv.jinyuanbaomall.cn

E. 字符串处理
来源：http://frv.mhx1999.top

================================================================================
来源：http://vcj.iojbl.cn

[E01] 拼接字符串
来源：http://djh.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kjs.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pef.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ezx.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aqu.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xps.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gil.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pxh.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://efn.jinqigufen.top

[E02] 重复字符串
来源：http://yyp.guowangkeji.top

Py:   "ab" * 3
来源：http://joh.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://hcv.fktsv.cn

JS:   "ab".repeat(3)
来源：http://kuq.sweek.top

TS:   "ab".repeat(3)
来源：http://kot.xinyue.icu

Java: "ab".repeat(3)
来源：http://ziy.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://lnr.shuidangran.top

Ruby: "ab" * 3
来源：http://avl.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jke.vqdsnc.cn

[E03] 截取子串
来源：http://lbf.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://irl.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bhv.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pdt.yfazqb.com

TS:   s.slice(1, 4)
来源：http://erg.yueranfly.top

Java: s.substring(1, 4)
来源：http://dvt.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mck.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://mvb.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://hsb.yuxming.cn

[E04] 查找子串位置
来源：http://gen.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://lse.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://qjv.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rvo.c1oappe.top

TS:   s.indexOf("x")
来源：http://oao.yj202588.top

Java: s.indexOf("x")
来源：http://hes.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://npb.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://tpt.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://pjd.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hkk.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jrs.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lyw.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ggr.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pln.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nqv.dianchejie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zxh.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pby.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mkd.zhoulong.xyz

[E06] 替换子串
来源：http://sso.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zbs.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://sch.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xfr.haohaochexian.top

TS:   s.replaceAll("a", "b")
来源：http://mfp.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pnr.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eba.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://utt.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://nwl.cashguo.top

[E07] 按分隔符拆分
来源：http://pwp.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dlh.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ioy.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wxq.hammf.cn

TS:   s.split(",")
来源：http://xxs.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bij.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jzr.xingfuxueyuan.xyz

Ruby: s.split(",");  s.split
来源：http://zoy.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lbp.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://sid.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://iix.yongpay.top

PHP:  implode(",", $items);
来源：http://rff.yj20258888.top

JS:   items.join(",")
来源：http://kao.tanke756.top

TS:   items.join(",")
来源：http://omd.hywenlv.cn

Java: String.join(",", items)
来源：http://zwv.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://udu.zhengqikj.top

Ruby: items.join(",")
来源：http://fvd.316326.xyz

C#:   string.Join(",", items)
来源：http://zvk.hfpthk.cn

[E09] 去除所有空白字符
来源：http://sxc.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jsf.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tgk.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://lwq.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://dwp.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://hzz.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gvs.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dls.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gcw.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://gef.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yva.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uea.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://oyo.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://tpt.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://ign.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://npr.zhaomingkeji.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fzb.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mnf.birdmap.top

[E11] 反转字符串
来源：http://fvk.fehbvm.com

Py:   s[::-1]
来源：http://pdv.316326.xyz

PHP:  strrev($s);
来源：http://lak.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://cht.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://mem.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hpj.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kls.cucudq.cn

Ruby: s.reverse
来源：http://ogx.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://ayy.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://xrl.vqdsnc.cn

Py:   s.count("a")
来源：http://lyv.tanke756.top

PHP:  substr_count($s, "a");
来源：http://ddu.zhixingplan.top

JS:   s.split("a").length - 1
来源：http://cpo.uphjek.com

TS:   s.split("a").length - 1
来源：http://gmv.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aiz.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://mta.snrcjt.cn

Ruby: s.count("a")
来源：http://wcz.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://oyh.nwbrower.top

[E13] 逐字符遍历
来源：http://gwn.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://fdj.redwolf501.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dtw.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nqn.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fry.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lqm.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://njc.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://six.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://skm.sysykeji.top

[E14] URL 编码与 Base64
来源：http://ual.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qop.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lro.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vwc.316326.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wpv.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://epl.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wdn.yongpay.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bgr.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rlb.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://jme.kuanghao11.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://aly.hnxiangtu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rfe.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lwd.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ptf.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ziz.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lgz.fanxiaobao.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zci.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qou.ctjpmb.com

[E16] 数字千分位
来源：http://lwt.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://aze.fengsongda.top

PHP:  number_format(1234567);
来源：http://ejq.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oau.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lgz.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pfc.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://frg.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dfc.yongpay.top

C#:   1234567.ToString("N0")
来源：http://ajg.hfpthk.cn

[E17] 首字母大写
来源：http://wqd.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ndc.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wob.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kin.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ksq.vqdsnc.cn


<!-- 参考信息 -->