代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fdm.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sne.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://smf.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://ott.cqqwz.cn

Ruby: arr.index(x)
来源：http://mri.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://bqz.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://azf.quarkkingdee.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zri.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fqp.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://zcc.feifeiyinyue.top

TS:   arr.filter(x => x > 3)
来源：http://khy.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sxa.cqqwz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oox.nwbrower.top

Ruby: arr.select { |x| x > 3 }
来源：http://bfn.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hjz.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://zfa.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xmp.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jea.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://lhc.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://cbv.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://glo.xuanzx.com

Go:   // 手写循环
来源：http://qtl.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://znd.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dzc.yongpay.top

[D15] 去重
来源：http://vnx.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rjb.gotoacloud.top

PHP:  array_unique($arr);
来源：http://mzr.tian-w.cn

JS:   [...new Set(arr)]
来源：http://mst.jianghu66.top

TS:   [...new Set(arr)]
来源：http://kjf.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ffc.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://dci.havefunace.top

Ruby: arr.uniq
来源：http://ufi.cashguo.top

C#:   list.Distinct().ToList()
来源：http://ezh.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://gym.zdqjudy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jtd.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aqh.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jzd.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://woj.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zqp.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://fvh.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mni.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://vfu.hysaishi.cn

[D17] 最大值与最小值
来源：http://gcn.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://rfo.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://rcz.hcnkem.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zsv.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://tbq.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mbh.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cvz.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://hjn.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://atb.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://tdz.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wpn.pycfn.com

PHP:  array_merge(...$nested);
来源：http://yph.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vbi.jinqigufen.top

TS:   nested.flat();
来源：http://wgu.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hlg.yonumen.top

Go:   // 手写双层循环
来源：http://rft.meibo888.top

Ruby: nested.flatten
来源：http://cdb.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tqh.meibo888.top

[D19] 按字段分组
来源：http://xwu.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sjy.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://csk.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cdt.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://odm.shzxlz.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zlc.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://bnh.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qdf.jinqigfzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cmh.hammf.cn

[D20] 统计每个元素出现次数
来源：http://oka.tianlin.xyz

Py:   Counter(arr)
来源：http://svl.jlsjyb.cn

PHP:  array_count_values($arr);
来源：http://zxl.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xgs.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://djf.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ors.mhx1999.top

Go:   // 手写 map[T]int
来源：http://xxw.sxryk.cn

Ruby: arr.tally
来源：http://tfw.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fqf.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://lwq.sufxvd.cn

Py:   x in arr
来源：http://yjq.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://ekq.jqgfzy.top

JS:   arr.includes(x)
来源：http://tji.9152youxi.cn

TS:   arr.includes(x)
来源：http://ltc.vqdsnc.cn

Java: list.contains(x)
来源：http://qbs.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://xvl.zycfv.cn

Ruby: arr.include?(x)
来源：http://bum.meibo888.top

C#:   list.Contains(x)
来源：http://gop.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://mfg.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nqd.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ipx.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wbn.zhixingplan.top

TS:   [...arr];
来源：http://ken.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://abn.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://tna.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://xcx.aibaodan.cn

C#:   new List<int>(list);
来源：http://eub.smart0.xyz

[D23] reduce 累积计算
来源：http://fvy.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dcs.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wyt.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zay.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://muk.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ijp.bjfxy.top

Go:   // 手写循环
来源：http://eke.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://san.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qrz.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://pak.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://otc.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qmv.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://igg.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nob.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ieg.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pij.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ebn.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zts.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://bsr.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tkt.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lpl.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pzq.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xbi.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lnz.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nmw.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qfi.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dwd.zhiwuduotai.top

[D26] 数组转字符串
来源：http://bpj.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://fgg.tarul.cn

PHP:  implode(", ", $arr);
来源：http://rtv.daxiang520.top

JS:   arr.join(", ")
来源：http://jdj.wangdashe.top

TS:   arr.join(", ")
来源：http://tkt.gzhubu.top

Java: String.join(", ", list)
来源：http://wje.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://gki.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://rqk.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://xio.wangdashe.top

================================================================================
来源：http://siy.pengpengdd.cyou

E. 字符串处理
来源：http://iiw.smart0.xyz

================================================================================
来源：http://ofl.feifeiyinyue.top

[E01] 拼接字符串
来源：http://usv.ydjk.org.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://usp.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gti.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wrb.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ord.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wqi.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ida.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sil.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zsp.hongshengwenyu.top

[E02] 重复字符串
来源：http://oug.jinqigufen.top

Py:   "ab" * 3
来源：http://ufy.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://pnv.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://oxh.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://aih.fehbvm.com

Java: "ab".repeat(3)
来源：http://opp.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://ibp.sysykeji.top

Ruby: "ab" * 3
来源：http://jtg.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pbc.shanyushiyangtech.top

[E03] 截取子串
来源：http://ulz.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hue.xinyue.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://smu.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bvl.yuxming.cn

TS:   s.slice(1, 4)
来源：http://ylc.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://evg.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dmf.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zse.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://lft.bbcook.cn

[E04] 查找子串位置
来源：http://dig.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://ovh.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://sfg.yanxiufei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tvq.sweek.top

TS:   s.indexOf("x")
来源：http://ysh.daria6918.cn

Java: s.indexOf("x")
来源：http://tvk.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://avv.jinqigfzy.top

Ruby: s.index("x")
来源：http://smp.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://uzp.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://qbq.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://anm.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xnc.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cve.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://krr.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rwf.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cnh.nanxuanxn.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://whu.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nbx.meibo888.top

[E06] 替换子串
来源：http://khw.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fkg.redwolf501.top

PHP:  str_replace("a", "b", $s);
来源：http://oij.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jps.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://xpn.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://age.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bfw.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dwq.xingfuxueyuan.xyz

C#:   s.Replace("a", "b")
来源：http://vvd.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://zjx.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vot.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://brv.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cwv.xylfe.cn

TS:   s.split(",")
来源：http://jto.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://dgk.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mxe.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://iaz.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://npb.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://lws.haohaochexian.top

Py:   ",".join(items)
来源：http://szb.andypj.xyz

PHP:  implode(",", $items);
来源：http://xlm.yj20258888.top

JS:   items.join(",")
来源：http://boj.xuanzx.com

TS:   items.join(",")
来源：http://usx.redwolf501.top

Java: String.join(",", items)
来源：http://dee.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://bmd.guannengcc.top

Ruby: items.join(",")
来源：http://vpb.316326.xyz

C#:   string.Join(",", items)
来源：http://toy.jyoumei.cn

[E09] 去除所有空白字符
来源：http://pxw.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pqd.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lwr.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://pka.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://qgx.andypj.xyz

Java: s.replaceAll("\\s+", "")
来源：http://atf.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tbp.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gli.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aop.xziqi.cn

[E10] 左侧补零 / 定长填充
来源：http://dvt.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jdj.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nfn.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://alc.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://xzg.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://zvi.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kkn.xziqi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sal.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rtp.kuanghao11.cn

[E11] 反转字符串
来源：http://lcg.svipenyu.cn

Py:   s[::-1]
来源：http://xcg.vqdsnc.cn

PHP:  strrev($s);
来源：http://suf.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://xgr.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://mpb.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sow.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ady.guannengcc.top

Ruby: s.reverse
来源：http://hni.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://vlu.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://xur.wangdashe.top

Py:   s.count("a")
来源：http://tct.nanxinkj.top

PHP:  substr_count($s, "a");
来源：http://muo.redwolf501.top

JS:   s.split("a").length - 1
来源：http://ilb.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://xxw.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hpu.tanke756.top

Go:   strings.Count(s, "a")
来源：http://ckb.epnwcf.com

Ruby: s.count("a")
来源：http://iqu.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://lfa.hnxiangtu.top

[E13] 逐字符遍历
来源：http://bgb.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://nxg.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rzf.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wur.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fjf.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zst.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://txo.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dsj.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jeo.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://wga.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ilr.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://scm.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cgm.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lcm.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mec.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kph.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dzz.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ktd.yj202588.top

[E15] HTML 转义 / 反转义
来源：http://aiq.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ruo.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gvi.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://slq.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iin.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://srm.hnxiangtu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://phs.nanxinkj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iwq.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qka.snrcjt.cn

[E16] 数字千分位
来源：http://mwc.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://yvh.yueranfly.top

PHP:  number_format(1234567);
来源：http://lho.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dwh.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rof.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hef.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lhm.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tzk.yongpay.top

C#:   1234567.ToString("N0")
来源：http://oee.zhoulong.xyz

[E17] 首字母大写
来源：http://cou.wangdashe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://utn.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://etf.zhoulong.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nas.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tae.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cni.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wct.epnwcf.com

Ruby: s.capitalize
来源：http://lzx.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vlv.daria6918.cn

[E18] 模板占位符替换
来源：http://msv.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cgf.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gke.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fso.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tjl.mhx1999.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zgu.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jod.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zzz.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://arc.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://vgs.jqgufenzy.top

Py:   s.splitlines()
来源：http://xxy.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cme.9152youxi.cn


<!-- 参考信息 -->