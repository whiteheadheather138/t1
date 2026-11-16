代发 wailian999

[D11] 反转数组
来源：http://jgq.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vwu.yuxming.cn

PHP:  array_reverse($arr);
来源：http://rwt.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gqc.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://sfx.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://xwu.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://ugc.vqdsnc.cn

Ruby: arr.reverse
来源：http://mbv.cashguo.top

C#:   list.Reverse();
来源：http://ffn.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://nug.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://qks.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kgl.daxiang520.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lce.pengpengdd.cyou

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jgc.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ode.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://qgt.hammf.cn

Ruby: arr.index(x)
来源：http://dlr.xuanzx.com

C#:   list.IndexOf(x);
来源：http://jju.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://nmu.shanyushiyangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fft.shuidangran.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lve.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://muf.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://oko.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://itj.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oug.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zov.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ffw.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://knt.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pei.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dfm.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://gix.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://wue.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xke.zdqjudy.top

Go:   // 手写循环
来源：http://gha.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://grd.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://igb.xinyue.icu

[D15] 去重
来源：http://dff.yfazqb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vcr.zycfv.cn

PHP:  array_unique($arr);
来源：http://pyl.ybcxt.top

JS:   [...new Set(arr)]
来源：http://ldt.yj20258.top

TS:   [...new Set(arr)]
来源：http://hpf.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hxm.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hcp.bbcook.cn

Ruby: arr.uniq
来源：http://pli.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://vdd.aizwys.cn

[D16] 求和与平均值
来源：http://oql.tian-w.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lwc.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://soh.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mip.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zar.yfazqb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ozl.yuxming.cn

Go:   // 手写循环累加
来源：http://ogw.zhixingplan.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rhz.sxryk.cn

C#:   list.Sum();  list.Average()
来源：http://pci.yangfankeji.com

[D17] 最大值与最小值
来源：http://riw.sjlbkw.cn

Py:   max(arr);  min(arr)
来源：http://nnx.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://txs.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nyn.hammf.cn

TS:   Math.max(...arr);
来源：http://hdc.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lsv.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qne.hongshengwenyu.top

Ruby: arr.max;  arr.min
来源：http://zem.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://uki.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://cbd.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://snu.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://mgo.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nnf.shuidangran.top

TS:   nested.flat();
来源：http://ody.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jzn.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://luu.dianchejie.cn

Ruby: nested.flatten
来源：http://kmt.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://alx.nanxuanxn.top

[D19] 按字段分组
来源：http://umo.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aot.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vup.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jfc.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rsd.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pxn.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://xml.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hlp.kuanghao11.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ijv.c1oappe.top

[D20] 统计每个元素出现次数
来源：http://xcq.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://bkf.havefunace.top

PHP:  array_count_values($arr);
来源：http://qis.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jiz.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ghh.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tfm.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://xqn.cheryme.top

Ruby: arr.tally
来源：http://tuu.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jzr.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://jex.xingfuxueyuan.xyz

Py:   x in arr
来源：http://fek.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://pls.mhx1999.top

JS:   arr.includes(x)
来源：http://vsz.tianlin.xyz

TS:   arr.includes(x)
来源：http://bch.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://utp.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://cvk.zdbjq.cn

Ruby: arr.include?(x)
来源：http://mvj.pycfn.com

C#:   list.Contains(x)
来源：http://tbi.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://jde.yongpay.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://moi.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hbo.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cmg.zhixingplan.top

TS:   [...arr];
来源：http://vqf.xziqi.cn

Java: new ArrayList<>(list);
来源：http://yuz.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://mkh.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://vym.snrcjt.cn

C#:   new List<int>(list);
来源：http://qgi.cashguo.top

[D23] reduce 累积计算
来源：http://bkj.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rgu.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cdc.jlsjyb.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dli.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tpt.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zzk.tarul.cn

Go:   // 手写循环
来源：http://mkq.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mfa.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tqz.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://inl.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yyb.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rui.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wxw.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qqg.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fhg.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vfk.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dxz.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vfg.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://kgs.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rca.svipenyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rkd.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vpn.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ztr.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kdf.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bcy.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rqw.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://afv.daxiang520.top

[D26] 数组转字符串
来源：http://ghd.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://wbk.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://isf.epnwcf.com

JS:   arr.join(", ")
来源：http://xap.zhixingplan.top

TS:   arr.join(", ")
来源：http://rkk.ppjwa.cn

Java: String.join(", ", list)
来源：http://pnz.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://ubc.sxryk.cn

Ruby: arr.join(", ")
来源：http://cft.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://nwi.xuanzx.com

================================================================================
来源：http://pce.meibo888.top

E. 字符串处理
来源：http://upm.ywan-chungtsiang.top

================================================================================
来源：http://dvs.yvedp.cn

[E01] 拼接字符串
来源：http://sez.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://duk.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lhs.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ktw.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pgx.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://veg.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cay.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lpl.zhoulong.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nkj.hysaishi.cn

[E02] 重复字符串
来源：http://zjk.hysaishi.cn

Py:   "ab" * 3
来源：http://ury.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://iuo.birdmap.top

JS:   "ab".repeat(3)
来源：http://atl.hesvh.cn

TS:   "ab".repeat(3)
来源：http://ytm.cdnleiting.top

Java: "ab".repeat(3)
来源：http://ptr.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://gkn.cashguo.top

Ruby: "ab" * 3
来源：http://qgv.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kra.uphjek.com

[E03] 截取子串
来源：http://bot.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nlh.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://osg.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tfd.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://hqt.9152youxi.cn

Java: s.substring(1, 4)
来源：http://bsv.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uwc.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bbv.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://rhf.svipenyu.cn

[E04] 查找子串位置
来源：http://mcr.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://vxi.tian-w.cn

PHP:  strpos($s, "x");
来源：http://rec.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ton.52xcode.cn

TS:   s.indexOf("x")
来源：http://mtl.hnxiangtu.top

Java: s.indexOf("x")
来源：http://ckq.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://nfj.yj20258888.top

Ruby: s.index("x")
来源：http://paa.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://iky.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bov.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rkx.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ipt.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uih.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://usn.nanxinkj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hjc.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gxu.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wgk.daxiang520.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bon.vqdsnc.cn

[E06] 替换子串
来源：http://cdr.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cvj.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://uhx.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lzd.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://fzs.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zhg.hammf.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wba.cashguo.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wpt.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://bew.hywenlv.cn

[E07] 按分隔符拆分
来源：http://aaq.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://khi.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rik.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jaq.bbcook.cn

TS:   s.split(",")
来源：http://lyr.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://got.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mcq.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://rbv.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wpo.yuxming.cn

[E08] 数组按分隔符合并
来源：http://jfh.hnxiangtu.top

Py:   ",".join(items)
来源：http://qnu.yongpay.top

PHP:  implode(",", $items);
来源：http://avb.sxryk.cn

JS:   items.join(",")
来源：http://wev.hnqzz.top

TS:   items.join(",")
来源：http://mjw.uphjek.com

Java: String.join(",", items)
来源：http://qfk.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://hif.jianghu66.top

Ruby: items.join(",")
来源：http://bnq.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://qgk.316326.xyz

[E09] 去除所有空白字符
来源：http://bas.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rnp.zhiwuduotai.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nev.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://qoj.jinqigfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://voh.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://hgp.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://huc.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ajr.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qik.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://sxl.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lwm.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ddd.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://lbd.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://svg.ydzc1.top

Java: String.format("%03d", 7)
来源：http://tau.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hwx.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aih.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pxs.gzhubu.top

[E11] 反转字符串
来源：http://tii.quarkkingdee.top

Py:   s[::-1]
来源：http://edw.nanxuanxn.top

PHP:  strrev($s);
来源：http://zmv.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://vgc.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://dly.shanyushiyangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nps.uphjek.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://luj.hongshengwenyu.top

Ruby: s.reverse
来源：http://osh.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://laz.sysykeji.top

[E12] 统计某字符出现次数
来源：http://aum.gaohongyu789.top

Py:   s.count("a")
来源：http://jtb.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://opq.ydzc1.top

JS:   s.split("a").length - 1
来源：http://wgr.zhongyouzk.top

TS:   s.split("a").length - 1
来源：http://acl.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vgu.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://exr.jqgufenzy.top

Ruby: s.count("a")
来源：http://qli.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://mys.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://wul.yj20258.top

Py:   for ch in s: print(ch)
来源：http://jeb.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ova.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://scm.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ldf.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zrv.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zeo.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://koj.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xlu.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://zpj.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://siw.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://doy.zhongyouzk.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uii.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zdz.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xnu.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://awm.bjfxy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xji.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tef.zhijiandao.cn

[E15] HTML 转义 / 反转义
来源：http://qms.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cnr.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yei.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wiq.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xxc.ydzc1.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ree.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ivm.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://agz.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gim.xuanzx.com

[E16] 数字千分位
来源：http://gqb.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://zad.andypj.xyz

PHP:  number_format(1234567);
来源：http://rxu.cheryme.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dnq.gotoacloud.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cpb.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xxk.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ack.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hax.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://jyq.daxiang520.top

[E17] 首字母大写
来源：http://fty.hysaishi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sss.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qar.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hyb.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fzo.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dzl.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://moj.jyoumei.cn

Ruby: s.capitalize
来源：http://ilr.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lun.nanxinkj.top


<!-- 参考信息 -->