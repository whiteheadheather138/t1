代发 wailian999

C#:   list.Reverse();
来源：http://itt.chenlongwang.top

[D12] 查找元素下标
来源：http://ksu.feifeiyinyue.top

Py:   arr.index(x);  x in arr
来源：http://enu.bjfxy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tdn.xuetiantiany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wfi.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://don.zhoulong.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ljx.hammf.cn

Go:   slices.Index(arr, x)
来源：http://chi.vqdsnc.cn

Ruby: arr.index(x)
来源：http://sbm.tanke756.top

C#:   list.IndexOf(x);
来源：http://lob.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://jty.xinyue.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://avb.fanxiaobao.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eoy.smart0.xyz

JS:   arr.filter(x => x > 3)
来源：http://vod.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://ylu.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jeg.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://khy.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hxj.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pky.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://gvd.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pdd.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fbr.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://avu.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://bfm.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://lja.jinghuilouyu.cn

Go:   // 手写循环
来源：http://adi.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://glu.daxiang520.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lor.guowangkeji.top

[D15] 去重
来源：http://xmu.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dit.meibo888.top

PHP:  array_unique($arr);
来源：http://heo.cucudq.cn

JS:   [...new Set(arr)]
来源：http://vxl.fzhhl.top

TS:   [...new Set(arr)]
来源：http://vul.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wdx.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://ijk.bjfxy.top

Ruby: arr.uniq
来源：http://xrb.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://ned.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://bft.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ogv.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://utp.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uym.cqqwz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vii.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yvn.ehwqpu.com

Go:   // 手写循环累加
来源：http://ilm.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iuj.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://fea.fzhhl.top

[D17] 最大值与最小值
来源：http://fyl.shzxlz.cn

Py:   max(arr);  min(arr)
来源：http://qla.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://zuh.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rkp.nwbrower.top

TS:   Math.max(...arr);
来源：http://bri.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://bjd.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rxv.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://baj.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://utn.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://sux.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qny.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://hpe.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://weq.yonumen.top

TS:   nested.flat();
来源：http://qmg.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ucy.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://epo.smart0.xyz

Ruby: nested.flatten
来源：http://uyd.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ccm.gaohongyu789.top

[D19] 按字段分组
来源：http://vcr.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ycv.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mzi.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xtz.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://swr.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rxz.wangdashe.top

Go:   // 手写 map[string][]T
来源：http://gil.ctjpmb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ben.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fpz.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://lgn.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://tis.zdbjq.cn

PHP:  array_count_values($arr);
来源：http://bur.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kwr.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xay.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://luf.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://tmf.hnqzz.top

Ruby: arr.tally
来源：http://zsj.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kjb.redwolf501.top

[D21] 判断是否包含某元素
来源：http://jsq.ivvv.top

Py:   x in arr
来源：http://rqo.chenjidiqi.icu

PHP:  in_array($x, $arr, true);
来源：http://xka.jlsjyb.cn

JS:   arr.includes(x)
来源：http://kaf.zhijiandao.cn

TS:   arr.includes(x)
来源：http://zkb.pycfn.com

Java: list.contains(x)
来源：http://spe.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://tqa.tanke756.top

Ruby: arr.include?(x)
来源：http://kuf.tianlin.xyz

C#:   list.Contains(x)
来源：http://zvq.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://zsv.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://whm.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iiu.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://chz.guowangkeji.top

TS:   [...arr];
来源：http://nnw.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://xqt.cheryme.top

Go:   copied := append([]int(nil), arr...)
来源：http://fbj.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://wyv.cucudq.cn

C#:   new List<int>(list);
来源：http://lim.wangdashe.top

[D23] reduce 累积计算
来源：http://cyb.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blm.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jqf.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uno.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://khb.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ojk.cdnleiting.top

Go:   // 手写循环
来源：http://evx.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tdm.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hqp.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://nfk.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://otq.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vjc.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pyp.yuxming.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bhq.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nou.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://azs.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oqa.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sop.yonumen.top

[D25] Set 集合去重与交并差
来源：http://oon.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jwb.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ims.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://knl.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ivc.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://opu.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eqw.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qsg.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://krz.nwbrower.top

[D26] 数组转字符串
来源：http://omr.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://ktc.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://pvc.0kj1m.cn

JS:   arr.join(", ")
来源：http://ldu.yj20258888.top

TS:   arr.join(", ")
来源：http://nkv.shuidangran.top

Java: String.join(", ", list)
来源：http://ddg.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://ege.daria6918.cn

Ruby: arr.join(", ")
来源：http://bpc.sxryk.cn

C#:   string.Join(", ", list)
来源：http://dgs.zhongyouzk.top

================================================================================
来源：http://qqc.aibaodan.cn

E. 字符串处理
来源：http://fpg.zycfv.cn

================================================================================
来源：http://bdf.zhiwuduotai.top

[E01] 拼接字符串
来源：http://ovn.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zkm.zdbjq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://asl.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ohb.tian-w.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lgi.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eay.sxryk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qvm.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gbf.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mtz.fengsongda.top

[E02] 重复字符串
来源：http://nel.cucudq.cn

Py:   "ab" * 3
来源：http://khw.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://dih.sysykeji.top

JS:   "ab".repeat(3)
来源：http://kjc.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://tkp.jyoumei.cn

Java: "ab".repeat(3)
来源：http://gea.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://arx.hnxiangtu.top

Ruby: "ab" * 3
来源：http://ozl.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yco.fehbvm.com

[E03] 截取子串
来源：http://znr.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sth.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://llk.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vce.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://vty.jyoumei.cn

Java: s.substring(1, 4)
来源：http://yfv.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gkl.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zgr.tanke756.top

C#:   s.Substring(1, 3)
来源：http://zjv.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://nsh.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://cai.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://tyc.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gby.haohaochexian.top

TS:   s.indexOf("x")
来源：http://wpl.nanxinkj.top

Java: s.indexOf("x")
来源：http://ztz.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://vbq.tian-w.cn

Ruby: s.index("x")
来源：http://ilw.tarul.cn

C#:   s.IndexOf("x")
来源：http://xga.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yxm.zycfv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wvh.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jkj.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zta.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xiq.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vas.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pwm.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ykd.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bht.snrcjt.cn

[E06] 替换子串
来源：http://ujx.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xxl.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://xqe.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pmj.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://htt.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ewu.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gdt.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vvm.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://xjs.vehdjk.com

[E07] 按分隔符拆分
来源：http://wsz.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bow.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gqs.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xvf.ydjk.org.cn

TS:   s.split(",")
来源：http://oto.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://jdh.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ecl.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://mti.havefunace.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jnw.cucudq.cn

[E08] 数组按分隔符合并
来源：http://mvd.yvedp.cn

Py:   ",".join(items)
来源：http://ihn.hcnkem.com

PHP:  implode(",", $items);
来源：http://mmh.gaohongyu789.top

JS:   items.join(",")
来源：http://hvf.hcnkem.com

TS:   items.join(",")
来源：http://pzv.ctjpmb.com

Java: String.join(",", items)
来源：http://sqh.meibo888.top

Go:   strings.Join(items, ",")
来源：http://gkj.zhixingplan.top

Ruby: items.join(",")
来源：http://rvx.birdmap.top

C#:   string.Join(",", items)
来源：http://cls.jyoumei.cn

[E09] 去除所有空白字符
来源：http://oag.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zah.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hip.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://fhx.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://uxh.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://dhb.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ymv.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://uky.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qda.jinghuilouyu.cn

[E10] 左侧补零 / 定长填充
来源：http://pus.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oqj.chenzaomai.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jlt.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://fsa.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://heb.sysykeji.top

Java: String.format("%03d", 7)
来源：http://dcv.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xti.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bap.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bxv.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://gln.sjlbkw.cn

Py:   s[::-1]
来源：http://bji.zhixingplan.top

PHP:  strrev($s);
来源：http://fsz.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://knz.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://ilu.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bag.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ygn.fanxiaobao.xyz

Ruby: s.reverse
来源：http://wxg.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://rcs.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://iwx.yuanzhike.top

Py:   s.count("a")
来源：http://jrj.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://wvc.birdmap.top

JS:   s.split("a").length - 1
来源：http://ykl.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://ipd.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vmg.hnqzz.top

Go:   strings.Count(s, "a")
来源：http://qgd.yvedp.cn

Ruby: s.count("a")
来源：http://txo.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://fys.gzhubu.top

[E13] 逐字符遍历
来源：http://pso.yueranfly.top

Py:   for ch in s: print(ch)
来源：http://mwb.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fyj.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sdq.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ejq.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yss.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://njb.ctjpmb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://xuy.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pex.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://lmj.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vzd.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zfh.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://puu.bjfxy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ang.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qmf.yuxming.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tqw.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ngu.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://izu.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://qjo.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://clq.ywan-chungtsiang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ruu.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bej.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ehb.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iim.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zwt.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rbj.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dtg.zhengqikj.top

[E16] 数字千分位
来源：http://tsk.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://fek.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://aod.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rvz.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://irb.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wls.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ngm.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nen.epnwcf.com

C#:   1234567.ToString("N0")
来源：http://rbd.zdqjudy.top

[E17] 首字母大写
来源：http://dsd.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rsp.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://jlw.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iqm.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://anl.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tzs.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cdb.fktsv.cn

Ruby: s.capitalize
来源：http://orh.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kju.yj202588.top

[E18] 模板占位符替换
来源：http://uje.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qfa.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xqq.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yyb.yj202588.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aki.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wyo.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vdc.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sea.vqdsnc.cn


<!-- 参考信息 -->