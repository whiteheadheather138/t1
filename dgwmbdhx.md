代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://anh.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oqj.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kpy.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://edw.zhaomingkeji.xyz

Ruby: arr.index(x)
来源：http://dmy.vehdjk.com

C#:   list.IndexOf(x);
来源：http://ujo.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://vrm.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jfv.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iwz.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://max.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://php.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ztu.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fmv.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dbz.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cfh.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://vws.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ndn.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vnv.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://odv.yj202588.top

TS:   arr.map(x => x * 2)
来源：http://nja.52xcode.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bzr.quarkkingdee.top

Go:   // 手写循环
来源：http://voq.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://xyy.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pea.0kj1m.cn

[D15] 去重
来源：http://xst.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cpu.hywenlv.cn

PHP:  array_unique($arr);
来源：http://dfg.sysykeji.top

JS:   [...new Set(arr)]
来源：http://enl.yueranfly.top

TS:   [...new Set(arr)]
来源：http://tan.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bvt.feifeiyinyue.top

Go:   // 用 map[T]struct{} 手写
来源：http://iao.sxryk.cn

Ruby: arr.uniq
来源：http://nek.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://vyk.hnqzz.top

[D16] 求和与平均值
来源：http://ice.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zjq.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ljx.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yaq.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrw.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qqi.zhixingplan.top

Go:   // 手写循环累加
来源：http://asn.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fhx.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://cjb.wangdashe.top

[D17] 最大值与最小值
来源：http://qcx.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://hsu.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://inu.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://haa.yonumen.top

TS:   Math.max(...arr);
来源：http://pgf.ydjk.org.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nxx.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lvi.pycfn.com

Ruby: arr.max;  arr.min
来源：http://yvc.9152youxi.cn

C#:   list.Max();  list.Min()
来源：http://elw.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://gri.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wlp.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://iqh.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mxf.jqgfzy.top

TS:   nested.flat();
来源：http://lao.fehbvm.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hno.havefunace.top

Go:   // 手写双层循环
来源：http://whj.iojbl.cn

Ruby: nested.flatten
来源：http://xvb.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://myk.0kj1m.cn

[D19] 按字段分组
来源：http://pzc.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lbo.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vau.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tua.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mtv.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sak.cheryme.top

Go:   // 手写 map[string][]T
来源：http://dvf.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bvn.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://izc.sjlbkw.cn

[D20] 统计每个元素出现次数
来源：http://hcm.zhoulong.xyz

Py:   Counter(arr)
来源：http://gej.zdbjq.cn

PHP:  array_count_values($arr);
来源：http://mpb.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mit.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uur.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xrw.redwolf501.top

Go:   // 手写 map[T]int
来源：http://xvs.xuanzx.com

Ruby: arr.tally
来源：http://lor.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ati.vehdjk.com

[D21] 判断是否包含某元素
来源：http://ngk.jinyuanbaomall.cn

Py:   x in arr
来源：http://qee.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://pmc.cdnleiting.top

JS:   arr.includes(x)
来源：http://qdy.yj20258.top

TS:   arr.includes(x)
来源：http://giq.jiagoushi.top

Java: list.contains(x)
来源：http://vcq.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://xjf.fzhhl.top

Ruby: arr.include?(x)
来源：http://yva.yonumen.top

C#:   list.Contains(x)
来源：http://bvi.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://awo.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zfh.hnxiangtu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vts.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dmk.jiagoushi.top

TS:   [...arr];
来源：http://rmi.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://bow.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://umf.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://zba.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://hha.uphjek.com

[D23] reduce 累积计算
来源：http://gid.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eld.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yeb.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lsk.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://khk.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://axj.yueranfly.top

Go:   // 手写循环
来源：http://oka.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fho.sxryk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ngc.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://pxl.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://epw.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ehf.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gar.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://akr.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ilp.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ksp.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fax.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rnw.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://kgc.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cjo.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oor.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://upx.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xzm.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://msd.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qtp.jinyuanbaomall.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yef.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yqh.9152youxi.cn

[D26] 数组转字符串
来源：http://agz.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://xmy.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://suv.epnwcf.com

JS:   arr.join(", ")
来源：http://onv.cucudq.cn

TS:   arr.join(", ")
来源：http://tui.hesvh.cn

Java: String.join(", ", list)
来源：http://faw.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://pjs.shuidangran.top

Ruby: arr.join(", ")
来源：http://nzp.yj20258.top

C#:   string.Join(", ", list)
来源：http://iam.gogol.net.cn

================================================================================
来源：http://ifz.jinqigfzy.top

E. 字符串处理
来源：http://egl.pycfn.com

================================================================================
来源：http://rup.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://vds.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rnv.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qiu.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wcs.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nul.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jbl.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xbo.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lvp.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qep.svipenyu.cn

[E02] 重复字符串
来源：http://ybo.jqgfzy.top

Py:   "ab" * 3
来源：http://day.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://eli.vehdjk.com

JS:   "ab".repeat(3)
来源：http://ugv.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://wif.daria6918.cn

Java: "ab".repeat(3)
来源：http://ity.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://ouj.gotoacloud.top

Ruby: "ab" * 3
来源：http://jgd.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yin.ivvv.top

[E03] 截取子串
来源：http://cjq.zhoulong.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ihy.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uom.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mak.hesvh.cn

TS:   s.slice(1, 4)
来源：http://pum.0kj1m.cn

Java: s.substring(1, 4)
来源：http://imy.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ffb.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vyz.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://wjm.xinyue.icu

[E04] 查找子串位置
来源：http://osw.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://hyf.yfazqb.com

PHP:  strpos($s, "x");
来源：http://dpv.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cal.xylfe.cn

TS:   s.indexOf("x")
来源：http://qhj.yuanzhike.top

Java: s.indexOf("x")
来源：http://urd.havefunace.top

Go:   strings.Index(s, "x")
来源：http://wmz.fehbvm.com

Ruby: s.index("x")
来源：http://tbm.iojbl.cn

C#:   s.IndexOf("x")
来源：http://cez.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lrw.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zzh.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rei.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igi.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://izu.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://trf.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lyv.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mzo.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hgk.hongshengwenyu.top

[E06] 替换子串
来源：http://apv.meibo888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://flt.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://ocz.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hgn.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://xjc.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hst.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eny.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://son.gaohongyu789.top

C#:   s.Replace("a", "b")
来源：http://mkk.yangfankeji.com

[E07] 按分隔符拆分
来源：http://ila.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://llj.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ikw.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lyz.vqdsnc.cn

TS:   s.split(",")
来源：http://lto.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dut.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vau.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://aqb.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dxq.cucudq.cn

[E08] 数组按分隔符合并
来源：http://mec.havefunace.top

Py:   ",".join(items)
来源：http://npr.hammf.cn

PHP:  implode(",", $items);
来源：http://hvp.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://ttl.hammf.cn

TS:   items.join(",")
来源：http://iqm.xuanzx.com

Java: String.join(",", items)
来源：http://etx.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://zsy.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://exd.wangdashe.top

C#:   string.Join(",", items)
来源：http://klm.316326.xyz

[E09] 去除所有空白字符
来源：http://qcz.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kqv.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lez.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://pce.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://tft.c1oappe.top

Java: s.replaceAll("\\s+", "")
来源：http://soq.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yti.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://svl.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jwk.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://lfx.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hha.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://udj.ywan-chungtsiang.top

JS:   "7".padStart(3, "0")
来源：http://eyp.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://and.yueranfly.top

Java: String.format("%03d", 7)
来源：http://bqy.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wcx.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tia.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://omi.redwolf501.top

[E11] 反转字符串
来源：http://bjg.zhengqikj.top

Py:   s[::-1]
来源：http://ope.sweek.top

PHP:  strrev($s);
来源：http://mkq.cheryme.top

JS:   [...s].reverse().join("")
来源：http://fkb.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://nsn.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pyc.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://uwn.chenlongwang.top

Ruby: s.reverse
来源：http://dln.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://tkp.tanke756.top

[E12] 统计某字符出现次数
来源：http://brf.kuanghao11.cn

Py:   s.count("a")
来源：http://skw.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://wbr.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://kcm.xuanzx.com

TS:   s.split("a").length - 1
来源：http://ilx.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jdg.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://hdu.tianlin.xyz

Ruby: s.count("a")
来源：http://qcb.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://qit.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://ovl.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://prk.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eso.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://war.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rmz.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aak.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://brx.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yjk.jqgufenzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ycp.yongpay.top

[E14] URL 编码与 Base64
来源：http://ipg.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fbs.0kj1m.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://txs.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vho.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://umw.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ymn.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kqb.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hse.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rae.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://qpr.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://irh.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ntv.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dam.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://vrp.sysykeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ubv.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rti.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wgr.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fhz.sjlbkw.cn

[E16] 数字千分位
来源：http://pkt.fzhhl.top

Py:   f"{1234567:,}"
来源：http://ggx.birdmap.top

PHP:  number_format(1234567);
来源：http://kzc.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zyy.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kjb.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://het.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://izk.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ltb.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://mci.chenzaomai.com

[E17] 首字母大写
来源：http://ojt.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vav.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tqi.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://djt.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ave.quarkkingdee.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qxj.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uvz.yonumen.top

Ruby: s.capitalize
来源：http://ftx.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ron.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://hkg.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wjf.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kfr.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tem.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ipz.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gig.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://noz.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://psq.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uyn.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://aeg.ydjk.org.cn

Py:   s.splitlines()
来源：http://fwl.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hzi.zhiwuduotai.top


<!-- 参考信息 -->