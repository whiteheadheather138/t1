代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://svo.chenlongwang.top

JS:   arr.filter(x => x > 3)
来源：http://oaa.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://wmg.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zwd.gzhubu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://due.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dgd.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jti.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://nzj.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://suk.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nhq.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://ddz.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://lkv.daxiang520.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://brj.bbcook.cn

Go:   // 手写循环
来源：http://pub.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://szq.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://avo.zhiwuduotai.top

[D15] 去重
来源：http://ktt.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hjp.nwbrower.top

PHP:  array_unique($arr);
来源：http://pgc.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://awe.52xcode.cn

TS:   [...new Set(arr)]
来源：http://wrk.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ckp.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://xtg.0kj1m.cn

Ruby: arr.uniq
来源：http://jwd.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://krv.feifeiyinyue.top

[D16] 求和与平均值
来源：http://oyc.shzxlz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xyo.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sdt.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uam.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dpn.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ckm.quarkkingdee.top

Go:   // 手写循环累加
来源：http://zfh.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vkp.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://jxd.nwbrower.top

[D17] 最大值与最小值
来源：http://mxf.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://tbj.ybcxt.top

PHP:  max($arr);  min($arr);
来源：http://gxo.zhongyouzk.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eff.52xcode.cn

TS:   Math.max(...arr);
来源：http://zux.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pkf.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://stn.birdmap.top

Ruby: arr.max;  arr.min
来源：http://xan.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://asp.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://wfs.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mix.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://yum.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ewk.hnxiangtu.top

TS:   nested.flat();
来源：http://xrh.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gmv.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://ecr.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://sni.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vuo.shzxlz.cn

[D19] 按字段分组
来源：http://azk.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aue.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uxm.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oqd.feifeiyinyue.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://osq.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bsu.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://gos.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://dec.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pyl.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://mzh.wangshuangyany.cn

Py:   Counter(arr)
来源：http://wku.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://qcp.zhaomingkeji.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ksk.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ctc.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xaf.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://iwb.snrcjt.cn

Ruby: arr.tally
来源：http://zhr.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gdd.hcnkem.com

[D21] 判断是否包含某元素
来源：http://sah.yongpay.top

Py:   x in arr
来源：http://fma.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://pyl.yfazqb.com

JS:   arr.includes(x)
来源：http://rps.zhengqikj.top

TS:   arr.includes(x)
来源：http://jff.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://dat.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://mlv.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://lmn.0kj1m.cn

C#:   list.Contains(x)
来源：http://psn.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://zed.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zsy.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://agb.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ose.gzhubu.top

TS:   [...arr];
来源：http://ufp.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://qjw.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://jcr.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://igb.jyoumei.cn

C#:   new List<int>(list);
来源：http://vdt.cheryme.top

[D23] reduce 累积计算
来源：http://ikz.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hnf.xylfe.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kvz.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lnz.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tff.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://guc.ppjwa.cn

Go:   // 手写循环
来源：http://wdc.jiagoushi.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://imj.hnqzz.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wav.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://kaf.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://urg.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cei.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ojx.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kos.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yei.wangshuangyany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://srs.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gfg.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kml.andypj.xyz

[D25] Set 集合去重与交并差
来源：http://zft.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zxb.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vpk.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vft.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kxh.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hwd.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xzb.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vmx.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uyo.fktsv.cn

[D26] 数组转字符串
来源：http://wto.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://zgm.sweek.top

PHP:  implode(", ", $arr);
来源：http://sqa.hnxiangtu.top

JS:   arr.join(", ")
来源：http://hui.tian-w.cn

TS:   arr.join(", ")
来源：http://saz.ehwqpu.com

Java: String.join(", ", list)
来源：http://vgo.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://shq.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://qzs.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://spw.sweek.top

================================================================================
来源：http://och.yj202588.top

E. 字符串处理
来源：http://ysu.cucudq.cn

================================================================================
来源：http://aiq.jinqigufen.top

[E01] 拼接字符串
来源：http://fej.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://chi.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ysv.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nje.snrcjt.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dvg.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bfo.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ppa.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pgb.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ady.pengpengdd.cyou

[E02] 重复字符串
来源：http://pvg.jianghu66.top

Py:   "ab" * 3
来源：http://omj.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://dln.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://svr.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://bwp.hesvh.cn

Java: "ab".repeat(3)
来源：http://bcb.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://hrl.yuxming.cn

Ruby: "ab" * 3
来源：http://iau.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nld.shangyingyoupin.top

[E03] 截取子串
来源：http://toq.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hpn.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vga.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://olp.guannengcc.top

TS:   s.slice(1, 4)
来源：http://tma.iojbl.cn

Java: s.substring(1, 4)
来源：http://fyh.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nxb.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://ydd.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://urn.hammf.cn

[E04] 查找子串位置
来源：http://anl.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://qct.havefunace.top

PHP:  strpos($s, "x");
来源：http://yot.vqdsnc.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yqt.tianlin.xyz

TS:   s.indexOf("x")
来源：http://thg.aibaodan.cn

Java: s.indexOf("x")
来源：http://luo.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://sjp.ppjwa.cn

Ruby: s.index("x")
来源：http://cdw.zdqjudy.top

C#:   s.IndexOf("x")
来源：http://bvw.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hke.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fqw.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ejz.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xkh.yangfankeji.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://kcz.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://adn.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hrb.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://krx.epnwcf.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fpy.tianlin.xyz

[E06] 替换子串
来源：http://bae.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wqk.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://lyg.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://anr.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://zzf.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jlw.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://myg.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://efp.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://rwz.cashguo.top

[E07] 按分隔符拆分
来源：http://dmg.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sym.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fbw.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jsh.iojbl.cn

TS:   s.split(",")
来源：http://uap.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://jfo.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mlt.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://zam.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bav.yj20258.top

[E08] 数组按分隔符合并
来源：http://rej.hnqzz.top

Py:   ",".join(items)
来源：http://ixg.xziqi.cn

PHP:  implode(",", $items);
来源：http://jar.haohaochexian.top

JS:   items.join(",")
来源：http://qxm.c1oappe.top

TS:   items.join(",")
来源：http://jry.xuanzx.com

Java: String.join(",", items)
来源：http://quv.jyoumei.cn

Go:   strings.Join(items, ",")
来源：http://mdb.ydzc1.top

Ruby: items.join(",")
来源：http://vyl.iojbl.cn

C#:   string.Join(",", items)
来源：http://xzn.ybcxt.top

[E09] 去除所有空白字符
来源：http://lzn.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jyv.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fet.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://iwc.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://urx.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://nbf.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jdm.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://qwy.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jvw.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://gco.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://did.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tqi.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://tpo.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://lkn.52xcode.cn

Java: String.format("%03d", 7)
来源：http://exi.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vio.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bjt.smart0.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rni.gzhubu.top

[E11] 反转字符串
来源：http://olg.zhiwuduotai.top

Py:   s[::-1]
来源：http://rsb.yangfankeji.com

PHP:  strrev($s);
来源：http://qee.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://tah.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://fui.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aql.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mks.ybcxt.top

Ruby: s.reverse
来源：http://gmd.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://fyt.fehbvm.com

[E12] 统计某字符出现次数
来源：http://cgl.aizwys.cn

Py:   s.count("a")
来源：http://wdf.cqqwz.cn

PHP:  substr_count($s, "a");
来源：http://bxc.c1oappe.top

JS:   s.split("a").length - 1
来源：http://fya.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://jdm.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vkc.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://upz.cqqwz.cn

Ruby: s.count("a")
来源：http://jjl.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://epi.yj20258.top

[E13] 逐字符遍历
来源：http://rsv.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://kru.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qic.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qwc.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qkb.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://czf.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://emq.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tzm.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bja.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://tvt.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lmq.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://msp.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pgc.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ena.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://unr.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zlz.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zak.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://twb.nanxinkj.top

[E15] HTML 转义 / 反转义
来源：http://sqm.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jeh.jinyuanbaomall.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kxz.pengpengdd.cyou

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wwz.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://eju.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://itb.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vkj.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xzg.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://haj.jlsjyb.cn

[E16] 数字千分位
来源：http://sre.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://ccs.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://ccr.snrcjt.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yjb.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kch.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://keg.sufxvd.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bgv.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wzo.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://kwj.nanxinkj.top

[E17] 首字母大写
来源：http://pwr.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gjn.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://onx.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kms.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bqo.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dak.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jhd.tian-w.cn

Ruby: s.capitalize
来源：http://sud.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blj.yvedp.cn

[E18] 模板占位符替换
来源：http://hgz.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qex.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xuy.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tef.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uet.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hil.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dgd.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qub.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lhg.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://lfh.pengpengdd.cyou

Py:   s.splitlines()
来源：http://egs.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cbm.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://rng.havefunace.top

TS:   s.split(/\r?\n/)
来源：http://git.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://ndc.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://kqc.shzxlz.cn

Ruby: s.lines
来源：http://aro.mhx1999.top

C#:   s.Split('\n')
来源：http://xxa.yongpay.top

[E20] 判断字符串是否为空
来源：http://ucd.havefunace.top

Py:   if not s:
来源：http://gmn.chenlongwang.top


<!-- 参考信息 -->