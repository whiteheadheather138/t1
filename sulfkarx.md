代发 wailian999

[D11] 反转数组
来源：http://vnk.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iiu.xuanzx.com

PHP:  array_reverse($arr);
来源：http://cyj.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wng.guowangkeji.top

TS:   [...arr].reverse();
来源：http://wuw.havefunace.top

Java: Collections.reverse(list);
来源：http://qda.yanxiufei.cn

Go:   slices.Reverse(arr)
来源：http://mgx.hywenlv.cn

Ruby: arr.reverse
来源：http://dsx.chenzaomai.com

C#:   list.Reverse();
来源：http://jij.xuanzx.com

[D12] 查找元素下标
来源：http://aix.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://spy.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rgw.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mpg.birdmap.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kca.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ioy.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://zpp.xziqi.cn

Ruby: arr.index(x)
来源：http://cnq.hammf.cn

C#:   list.IndexOf(x);
来源：http://qev.dashuyun.cn

[D13] 过滤（保留满足条件的）
来源：http://ayv.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fao.9152youxi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dzg.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://xje.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://mct.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://njh.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eho.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://aix.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gfs.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://qnh.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rvo.shzxlz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fmu.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://lyz.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://izx.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://fcc.hfpthk.cn

Go:   // 手写循环
来源：http://nmg.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://sce.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yxg.jinqigfzy.top

[D15] 去重
来源：http://axb.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://psr.hfpthk.cn

PHP:  array_unique($arr);
来源：http://djn.xziqi.cn

JS:   [...new Set(arr)]
来源：http://bsl.nwbrower.top

TS:   [...new Set(arr)]
来源：http://pws.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qbt.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://scw.jlsjyb.cn

Ruby: arr.uniq
来源：http://biy.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://tyn.jinqigufen.top

[D16] 求和与平均值
来源：http://afb.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nfb.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pru.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gxm.jinqigfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qvv.sweek.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gfc.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://pcy.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vbp.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://vnr.ctjpmb.com

[D17] 最大值与最小值
来源：http://lbo.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://tqi.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://bbd.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qjj.ivvv.top

TS:   Math.max(...arr);
来源：http://fjp.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://jtd.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qex.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://plj.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://dtk.cheryme.top

[D18] 扁平化嵌套数组
来源：http://urs.tanke756.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zwp.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://usi.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hjq.pycfn.com

TS:   nested.flat();
来源：http://fxz.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lyn.jinqigufen.top

Go:   // 手写双层循环
来源：http://awq.epnwcf.com

Ruby: nested.flatten
来源：http://qmf.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://duk.hysaishi.cn

[D19] 按字段分组
来源：http://tyc.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nln.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ujn.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kla.vehdjk.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://wrw.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://coj.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://ibw.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mjs.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lci.tanke756.top

[D20] 统计每个元素出现次数
来源：http://tsz.vqdsnc.cn

Py:   Counter(arr)
来源：http://bek.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://rgc.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ggr.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://guo.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rdb.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://ors.zhijiandao.cn

Ruby: arr.tally
来源：http://dec.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tut.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://hje.vehdjk.com

Py:   x in arr
来源：http://cey.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://wvo.yvedp.cn

JS:   arr.includes(x)
来源：http://gdc.havefunace.top

TS:   arr.includes(x)
来源：http://iak.yuxming.cn

Java: list.contains(x)
来源：http://fus.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://wrx.0kj1m.cn

Ruby: arr.include?(x)
来源：http://kbk.316326.xyz

C#:   list.Contains(x)
来源：http://hdg.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://mec.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dhm.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rtv.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qdf.hywenlv.cn

TS:   [...arr];
来源：http://irl.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://qsg.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://rrs.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://fyn.uphjek.com

C#:   new List<int>(list);
来源：http://ckg.jyoumei.cn

[D23] reduce 累积计算
来源：http://byz.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yrv.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gac.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lgj.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jyq.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qja.guowangkeji.top

Go:   // 手写循环
来源：http://zlj.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://myt.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zuo.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://lzq.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xjz.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xmz.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pmp.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lng.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rbc.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vcv.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kcf.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hix.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://ulz.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xqt.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nzb.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://prw.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dby.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aty.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zmd.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kie.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nss.quarkkingdee.top

[D26] 数组转字符串
来源：http://vde.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://cdx.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://nvx.ydzc1.top

JS:   arr.join(", ")
来源：http://lvm.hnqzz.top

TS:   arr.join(", ")
来源：http://uri.hfpthk.cn

Java: String.join(", ", list)
来源：http://zac.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://ral.sufxvd.cn

Ruby: arr.join(", ")
来源：http://asd.aizwys.cn

C#:   string.Join(", ", list)
来源：http://dwz.snrcjt.cn

================================================================================
来源：http://zga.snrcjt.cn

E. 字符串处理
来源：http://qsr.hywenlv.cn

================================================================================
来源：http://pwe.ehwqpu.com

[E01] 拼接字符串
来源：http://hmn.zhengqikj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zwr.zycfv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dxo.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yvs.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aho.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eby.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qkj.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nkv.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jls.c1oappe.top

[E02] 重复字符串
来源：http://vom.yongpay.top

Py:   "ab" * 3
来源：http://jlf.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://dsm.daria6918.cn

JS:   "ab".repeat(3)
来源：http://tuv.cucudq.cn

TS:   "ab".repeat(3)
来源：http://khb.jinghuilouyu.cn

Java: "ab".repeat(3)
来源：http://erc.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://opp.aibaodan.cn

Ruby: "ab" * 3
来源：http://kyd.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://llj.aizwys.cn

[E03] 截取子串
来源：http://cvg.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yao.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xrt.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xmu.316326.xyz

TS:   s.slice(1, 4)
来源：http://eth.ctjpmb.com

Java: s.substring(1, 4)
来源：http://dtl.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qia.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://gam.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://tvg.shuidangran.top

[E04] 查找子串位置
来源：http://qrq.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://aci.cheryme.top

PHP:  strpos($s, "x");
来源：http://cna.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kgs.jiagoushi.top

TS:   s.indexOf("x")
来源：http://txb.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://nhd.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://mkg.tanke756.top

Ruby: s.index("x")
来源：http://oar.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://tsc.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oop.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://snm.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jaq.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wft.c1oappe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://afb.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qje.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pyk.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://peh.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://prk.feifeiyinyue.top

[E06] 替换子串
来源：http://ubg.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kld.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://say.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ajk.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://bgd.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uda.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bnc.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fwi.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://evt.zhixingplan.top

[E07] 按分隔符拆分
来源：http://dyg.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://olj.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://exb.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ald.fzhhl.top

TS:   s.split(",")
来源：http://doa.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lll.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ccp.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://izr.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://crn.jyoumei.cn

[E08] 数组按分隔符合并
来源：http://fkj.jinghuilouyu.cn

Py:   ",".join(items)
来源：http://lnv.yj202588.top

PHP:  implode(",", $items);
来源：http://dnr.havefunace.top

JS:   items.join(",")
来源：http://djk.feifeiyinyue.top

TS:   items.join(",")
来源：http://iym.wangshuangyany.cn

Java: String.join(",", items)
来源：http://wkt.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://qbj.svipenyu.cn

Ruby: items.join(",")
来源：http://sny.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://qwc.pycfn.com

[E09] 去除所有空白字符
来源：http://blj.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pzt.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cgy.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://mss.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://oxu.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://mrv.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pev.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://mbi.havefunace.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://epr.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://hrf.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ooo.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lwk.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://gjl.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://uqw.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://qxn.bbcook.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kex.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ukk.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yfa.jinghuilouyu.cn

[E11] 反转字符串
来源：http://sly.tanke756.top

Py:   s[::-1]
来源：http://cjr.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://chz.guowangkeji.top

JS:   [...s].reverse().join("")
来源：http://dzp.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://rog.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://olz.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qzh.nwbrower.top

Ruby: s.reverse
来源：http://djk.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sqm.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://wkt.shuidangran.top

Py:   s.count("a")
来源：http://imn.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://hnv.hcnkem.com

JS:   s.split("a").length - 1
来源：http://owa.316326.xyz

TS:   s.split("a").length - 1
来源：http://ypl.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tdd.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://hkp.nanxuanxn.top

Ruby: s.count("a")
来源：http://hcg.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://hcw.zhijiandao.cn

[E13] 逐字符遍历
来源：http://lnd.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://qxx.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hze.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://dcr.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://itk.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://soo.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kmg.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://alw.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hxw.tanke756.top

[E14] URL 编码与 Base64
来源：http://tjx.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xla.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://atb.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fiy.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://idy.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xdr.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dgg.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wgg.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dcw.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://jvi.fzhhl.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uwe.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lhq.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vma.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rfm.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gfl.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ifh.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qlm.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hhy.jinqigufen.top

[E16] 数字千分位
来源：http://dhp.chenlongwang.top

Py:   f"{1234567:,}"
来源：http://erd.iojbl.cn

PHP:  number_format(1234567);
来源：http://zuz.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sqd.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://imh.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://whp.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qxv.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aha.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://wcr.ctjpmb.com

[E17] 首字母大写
来源：http://gai.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zkn.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://jdl.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rhh.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pvd.hnxiangtu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gay.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dix.smart0.xyz

Ruby: s.capitalize
来源：http://yme.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tup.jinqigfzy.top


<!-- 参考信息 -->