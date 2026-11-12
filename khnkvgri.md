代发 wailian999

C#:   list.Reverse();
来源：http://mhw.birdmap.top

[D12] 查找元素下标
来源：http://wun.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://tnd.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ods.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vbe.hywenlv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ifi.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zfo.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://xdz.wangdashe.top

Ruby: arr.index(x)
来源：http://eyl.yonumen.top

C#:   list.IndexOf(x);
来源：http://yhg.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://ihi.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xpv.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://owv.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://cns.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://nek.hcnkem.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zfb.tarul.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yib.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zud.hysaishi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://usx.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://fvz.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rry.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://irm.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://ktf.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://vnj.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gxd.ydzc1.top

Go:   // 手写循环
来源：http://mlb.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://kdt.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://stx.dianchejie.cn

[D15] 去重
来源：http://fvi.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mnw.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://qqh.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://hvk.zhoulong.xyz

TS:   [...new Set(arr)]
来源：http://rcg.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://buh.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://rmr.xuanzx.com

Ruby: arr.uniq
来源：http://yld.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://uqc.wangdashe.top

[D16] 求和与平均值
来源：http://tkf.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nzn.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hhn.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sca.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pdh.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rjg.cucudq.cn

Go:   // 手写循环累加
来源：http://oeb.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pyi.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://hpb.hcnkem.com

[D17] 最大值与最小值
来源：http://nkh.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://dup.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://osx.yuxming.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gbg.zdbjq.cn

TS:   Math.max(...arr);
来源：http://mtn.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lvj.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qir.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://xtf.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://mrt.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://flp.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pss.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://khp.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jqj.gzhubu.top

TS:   nested.flat();
来源：http://rtg.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sav.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://men.c1oappe.top

Ruby: nested.flatten
来源：http://jzz.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lmy.havefunace.top

[D19] 按字段分组
来源：http://byc.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sjd.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fkb.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gcs.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ugt.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mfk.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://vnd.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iss.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://glh.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://xwy.yfazqb.com

Py:   Counter(arr)
来源：http://oft.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://qeh.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gju.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ksw.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uqo.52xcode.cn

Go:   // 手写 map[T]int
来源：http://zwn.shanyushiyangtech.top

Ruby: arr.tally
来源：http://wyn.daxiang520.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ehs.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://ccn.hammf.cn

Py:   x in arr
来源：http://pzl.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://qps.kuanghao11.cn

JS:   arr.includes(x)
来源：http://jsu.aizwys.cn

TS:   arr.includes(x)
来源：http://edc.redwolf501.top

Java: list.contains(x)
来源：http://gyx.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://kyu.pycfn.com

Ruby: arr.include?(x)
来源：http://ogs.redwolf501.top

C#:   list.Contains(x)
来源：http://nih.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://abo.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zfe.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wvh.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xmg.ctjpmb.com

TS:   [...arr];
来源：http://chc.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://ihu.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://ofy.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://eyq.yangfankeji.com

C#:   new List<int>(list);
来源：http://put.zycfv.cn

[D23] reduce 累积计算
来源：http://ouo.ydjk.org.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lla.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iuu.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xdf.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lnm.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://hhe.yvedp.cn

Go:   // 手写循环
来源：http://cgt.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jie.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cfh.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://dup.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://odf.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fjv.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dbn.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uxt.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xuu.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gpr.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kab.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hkk.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://tdc.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oso.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eoi.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://abi.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://anr.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pap.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://thm.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kwh.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jom.guowangkeji.top

[D26] 数组转字符串
来源：http://fhs.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://hsq.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://pnp.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://cdf.316326.xyz

TS:   arr.join(", ")
来源：http://lzr.epnwcf.com

Java: String.join(", ", list)
来源：http://xgd.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://apt.hcnkem.com

Ruby: arr.join(", ")
来源：http://rbv.yueranfly.top

C#:   string.Join(", ", list)
来源：http://epm.nanxuanxn.top

================================================================================
来源：http://fmt.birdmap.top

E. 字符串处理
来源：http://aut.yuxming.cn

================================================================================
来源：http://tcv.feifeiyinyue.top

[E01] 拼接字符串
来源：http://xyf.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tnu.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uqf.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wkv.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wzq.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://brz.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pfu.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xrx.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zmc.nwbrower.top

[E02] 重复字符串
来源：http://ysh.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://bek.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://kew.xylfe.cn

JS:   "ab".repeat(3)
来源：http://pub.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://wxm.ydzc1.top

Java: "ab".repeat(3)
来源：http://pzi.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://fcs.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://cbb.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lhj.yuanzhike.top

[E03] 截取子串
来源：http://rfk.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wdq.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yar.jinqigufen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://csr.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://ipj.yangfankeji.com

Java: s.substring(1, 4)
来源：http://bjr.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ubk.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://atj.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://vyf.kuanghao11.cn

[E04] 查找子串位置
来源：http://vcw.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://hbd.nwbrower.top

PHP:  strpos($s, "x");
来源：http://rjc.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tac.yuanzhike.top

TS:   s.indexOf("x")
来源：http://kul.guannengcc.top

Java: s.indexOf("x")
来源：http://ege.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://qpq.vehdjk.com

Ruby: s.index("x")
来源：http://bbq.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://bih.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://flq.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nzl.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xsl.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ptc.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://fxw.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qhd.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mas.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eke.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sjc.c1oappe.top

[E06] 替换子串
来源：http://ukd.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dbn.guowangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://mgf.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hdi.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://jrn.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ubg.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sqd.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hje.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://znf.xuanzx.com

[E07] 按分隔符拆分
来源：http://uby.fehbvm.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iyd.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vxx.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jmt.sjlbkw.cn

TS:   s.split(",")
来源：http://oes.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://sge.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pnm.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://zea.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://spj.gzhubu.top

[E08] 数组按分隔符合并
来源：http://grv.zhoulong.xyz

Py:   ",".join(items)
来源：http://guh.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://ree.guannengcc.top

JS:   items.join(",")
来源：http://cbh.gotoacloud.top

TS:   items.join(",")
来源：http://wua.aizwys.cn

Java: String.join(",", items)
来源：http://ryw.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://udu.9152youxi.cn

Ruby: items.join(",")
来源：http://ptx.yongpay.top

C#:   string.Join(",", items)
来源：http://fiq.xylfe.cn

[E09] 去除所有空白字符
来源：http://thi.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nty.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rrv.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://rop.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://imu.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://dxc.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ifo.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://oel.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://avf.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://ouc.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://idx.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ryk.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://rok.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://slw.xuanzx.com

Java: String.format("%03d", 7)
来源：http://unw.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zmb.xingfuxueyuan.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xtg.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cqt.xylfe.cn

[E11] 反转字符串
来源：http://llo.yj20258.top

Py:   s[::-1]
来源：http://rxt.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://emb.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://bok.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://bxu.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ync.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mhh.ybcxt.top

Ruby: s.reverse
来源：http://mhq.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jwz.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://lhy.jqgufenzy.top

Py:   s.count("a")
来源：http://axf.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://fdk.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://vor.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://ksu.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tfj.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://nqz.ehwqpu.com

Ruby: s.count("a")
来源：http://fnp.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://fqg.havefunace.top

[E13] 逐字符遍历
来源：http://oxs.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://mnc.yongpay.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jio.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ksl.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jpe.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eba.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kvo.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ayu.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lya.yj20258.top

[E14] URL 编码与 Base64
来源：http://htu.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qwq.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kll.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iwh.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ojh.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vbz.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://paq.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cvs.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xqs.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://rkt.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://eyv.bjfxy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tyd.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sfc.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uqa.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bik.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ejc.jinqigfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uww.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pwv.jiagoushi.top

[E16] 数字千分位
来源：http://wvq.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://jny.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://dlh.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://lkx.jqgufenzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ius.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jnm.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zvd.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tjj.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://hde.zhengqikj.top

[E17] 首字母大写
来源：http://vch.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://smi.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ndi.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dzm.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rll.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vur.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ybi.zhiwuduotai.top

Ruby: s.capitalize
来源：http://xhx.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gii.yangfankeji.com

[E18] 模板占位符替换
来源：http://rwa.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kki.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nfq.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tul.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yah.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hrb.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gni.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qsb.shangyingyoupin.top


<!-- 参考信息 -->