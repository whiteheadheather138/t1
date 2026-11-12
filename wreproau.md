代发 wailian999

TS:   [...arr].reverse();
来源：http://vob.nwbrower.top

Java: Collections.reverse(list);
来源：http://ieu.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://vke.9152youxi.cn

Ruby: arr.reverse
来源：http://scd.xuetiantiany.cn

C#:   list.Reverse();
来源：http://gqw.hysaishi.cn

[D12] 查找元素下标
来源：http://fmh.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://ynt.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ano.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fxo.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://btv.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pil.fktsv.cn

Go:   slices.Index(arr, x)
来源：http://rrn.yanxiufei.cn

Ruby: arr.index(x)
来源：http://eyw.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://xbm.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://prf.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vad.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://puq.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://hfb.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://tph.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tqd.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yyr.jiagoushi.top

Ruby: arr.select { |x| x > 3 }
来源：http://dga.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://aee.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://nwm.zdqjudy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://exv.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fmh.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://gnt.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://hfa.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://whp.uphjek.com

Go:   // 手写循环
来源：http://opi.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://grv.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mhq.nanxuanxn.top

[D15] 去重
来源：http://bgk.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qkb.cheryme.top

PHP:  array_unique($arr);
来源：http://gba.xuanzx.com

JS:   [...new Set(arr)]
来源：http://slr.epnwcf.com

TS:   [...new Set(arr)]
来源：http://gtk.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gqj.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://rei.hammf.cn

Ruby: arr.uniq
来源：http://rkv.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://zht.yj20258888.top

[D16] 求和与平均值
来源：http://tfh.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cki.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rsg.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uac.gzhubu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pwx.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qtl.haohaochexian.top

Go:   // 手写循环累加
来源：http://okj.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dyi.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://xul.yj202588.top

[D17] 最大值与最小值
来源：http://gkz.kuanghao11.cn

Py:   max(arr);  min(arr)
来源：http://kzk.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://mjj.kuanghao11.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://owg.yvedp.cn

TS:   Math.max(...arr);
来源：http://wwu.jinqigfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://smu.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://snt.feifeiyinyue.top

Ruby: arr.max;  arr.min
来源：http://lsu.yonumen.top

C#:   list.Max();  list.Min()
来源：http://jlf.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://gth.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://orz.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://nwm.jinqigufen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ikr.ydzc1.top

TS:   nested.flat();
来源：http://gah.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tmr.xinyue.icu

Go:   // 手写双层循环
来源：http://lsd.shangyingyoupin.top

Ruby: nested.flatten
来源：http://vak.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ajv.gzhubu.top

[D19] 按字段分组
来源：http://tix.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://voo.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ooo.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fyq.haohaochexian.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wwi.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ioj.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://dlp.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ikw.jqgufenzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pwl.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://cpi.dashuyun.cn

Py:   Counter(arr)
来源：http://ovv.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://bfo.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ulf.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hxv.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qhj.chenjidiqi.icu

Go:   // 手写 map[T]int
来源：http://emx.zdbjq.cn

Ruby: arr.tally
来源：http://dzg.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uwe.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://ypi.jianghu66.top

Py:   x in arr
来源：http://qsd.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://pzm.ybcxt.top

JS:   arr.includes(x)
来源：http://dhu.dianchejie.cn

TS:   arr.includes(x)
来源：http://lry.jqgfzy.top

Java: list.contains(x)
来源：http://qjo.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://tnx.shuidangran.top

Ruby: arr.include?(x)
来源：http://yxr.vqdsnc.cn

C#:   list.Contains(x)
来源：http://dwr.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://hbh.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sov.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nci.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vcw.ctjpmb.com

TS:   [...arr];
来源：http://vix.smart0.xyz

Java: new ArrayList<>(list);
来源：http://kca.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ljw.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://geu.cdnleiting.top

C#:   new List<int>(list);
来源：http://ilt.sysykeji.top

[D23] reduce 累积计算
来源：http://yfi.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yqm.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rvd.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rrv.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yxc.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ahm.ybcxt.top

Go:   // 手写循环
来源：http://nnf.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zrr.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://txz.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://xxz.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://doy.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rld.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qwy.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://knn.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rav.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mla.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fni.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mtc.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://wjv.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://imn.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dbp.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mam.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fgr.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rez.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qem.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xnt.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nlt.zhengqikj.top

[D26] 数组转字符串
来源：http://gwm.fktsv.cn

Py:   ", ".join(map(str, arr))
来源：http://ufa.jiagoushi.top

PHP:  implode(", ", $arr);
来源：http://hnp.svipenyu.cn

JS:   arr.join(", ")
来源：http://qbl.pycfn.com

TS:   arr.join(", ")
来源：http://lwq.jlsjyb.cn

Java: String.join(", ", list)
来源：http://wci.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://hmq.hywenlv.cn

Ruby: arr.join(", ")
来源：http://yps.c1oappe.top

C#:   string.Join(", ", list)
来源：http://tjj.andypj.xyz

================================================================================
来源：http://hqs.chenlongwang.top

E. 字符串处理
来源：http://xbz.jyoumei.cn

================================================================================
来源：http://lud.c1oappe.top

[E01] 拼接字符串
来源：http://ryp.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dpa.hnxiangtu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ngs.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fdt.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jex.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rwq.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://onc.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bjy.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://abq.cashguo.top

[E02] 重复字符串
来源：http://swl.ctjpmb.com

Py:   "ab" * 3
来源：http://eae.nanxuanxn.top

PHP:  str_repeat("ab", 3);
来源：http://cla.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://ham.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://wbu.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://igu.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://hya.vehdjk.com

Ruby: "ab" * 3
来源：http://vtl.hfpthk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tdn.jinqigufen.top

[E03] 截取子串
来源：http://rbu.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wvk.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cau.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oxb.fengsongda.top

TS:   s.slice(1, 4)
来源：http://cht.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://nwi.wangdashe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hyw.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bzx.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://mji.316326.xyz

[E04] 查找子串位置
来源：http://zwp.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://pak.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://obn.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vsf.hysaishi.cn

TS:   s.indexOf("x")
来源：http://fxv.gogol.net.cn

Java: s.indexOf("x")
来源：http://nyz.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://znw.hfpthk.cn

Ruby: s.index("x")
来源：http://vqu.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://rdr.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://skf.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yjj.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wde.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jhc.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mav.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nct.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qrz.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xju.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://owc.hongshengwenyu.top

[E06] 替换子串
来源：http://rty.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ukf.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://ucu.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovw.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://lxs.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gsq.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gbd.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gee.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://adc.fzhhl.top

[E07] 按分隔符拆分
来源：http://wna.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gvu.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vhl.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://inn.sweek.top

TS:   s.split(",")
来源：http://gpk.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://qui.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jcq.yj20258888.top

Ruby: s.split(",");  s.split
来源：http://fgy.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wnl.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://kow.zhongyouzk.top

Py:   ",".join(items)
来源：http://lsw.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://grz.birdmap.top

JS:   items.join(",")
来源：http://xmd.cqqwz.cn

TS:   items.join(",")
来源：http://rrz.shzxlz.cn

Java: String.join(",", items)
来源：http://ize.cheryme.top

Go:   strings.Join(items, ",")
来源：http://nfa.cucudq.cn

Ruby: items.join(",")
来源：http://woi.guowangkeji.top

C#:   string.Join(",", items)
来源：http://uis.yj20258.top

[E09] 去除所有空白字符
来源：http://dlp.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zia.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mnv.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://yug.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://emj.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://agw.nanxinkj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sgc.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fgg.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xbs.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://pyv.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qte.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tzm.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://svx.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://asa.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://wdw.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wux.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sgy.hnxiangtu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rdd.shzxlz.cn

[E11] 反转字符串
来源：http://jso.jqgfzy.top

Py:   s[::-1]
来源：http://lwq.fktsv.cn

PHP:  strrev($s);
来源：http://zdt.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://kid.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://liu.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ggm.nwbrower.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ykt.havefunace.top

Ruby: s.reverse
来源：http://ozo.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ote.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://uhv.haohaochexian.top

Py:   s.count("a")
来源：http://iiv.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://efx.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://wom.yj20258888.top

TS:   s.split("a").length - 1
来源：http://cck.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://prk.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://apv.ydjk.org.cn

Ruby: s.count("a")
来源：http://ram.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://xbx.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://puy.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://dka.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://snl.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pmh.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wxz.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qvq.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jow.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mou.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ieh.zdqjudy.top

[E14] URL 编码与 Base64
来源：http://rmm.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eye.xziqi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hoy.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mcy.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tbv.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gpa.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lsz.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ujd.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eod.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://uyp.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cda.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wfb.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zbc.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uba.pengpengdd.cyou

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nau.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ect.hammf.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uem.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pzv.hnxiangtu.top

[E16] 数字千分位
来源：http://kdz.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://dun.zdbjq.cn

PHP:  number_format(1234567);
来源：http://yas.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zog.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://nbi.pycfn.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hwc.ivvv.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lbr.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jtg.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://ybu.svipenyu.cn

[E17] 首字母大写
来源：http://dwf.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ynq.jqgufenzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xsp.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jzm.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wwj.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gfp.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pdn.hongshengwenyu.top

Ruby: s.capitalize
来源：http://dbs.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sbt.quarkkingdee.top

[E18] 模板占位符替换
来源：http://cvy.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://glr.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xne.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vrp.xuetiantiany.cn


<!-- 参考信息 -->