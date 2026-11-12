代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qou.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://cuf.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pou.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://ntt.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ppi.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ens.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://gqt.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://gbt.feifeiyinyue.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dlx.vqdsnc.cn

Go:   // 手写循环
来源：http://fyv.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://eun.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://vaa.havefunace.top

[D15] 去重
来源：http://ote.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bxv.chenjidiqi.icu

PHP:  array_unique($arr);
来源：http://vtv.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://xgf.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://rkq.tanke756.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nbb.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://spv.yj202588.top

Ruby: arr.uniq
来源：http://cog.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://oaj.yongpay.top

[D16] 求和与平均值
来源：http://mah.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sjy.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nvt.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://stg.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zqh.fktsv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://idi.ppjwa.cn

Go:   // 手写循环累加
来源：http://qfu.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mkr.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://clf.mhx1999.top

[D17] 最大值与最小值
来源：http://mgd.meibo888.top

Py:   max(arr);  min(arr)
来源：http://sgh.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://fwi.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://apk.jiagoushi.top

TS:   Math.max(...arr);
来源：http://gbc.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bij.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ycs.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://vxy.yongpay.top

C#:   list.Max();  list.Min()
来源：http://nos.havefunace.top

[D18] 扁平化嵌套数组
来源：http://kbe.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uce.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://wqy.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ulj.sjlbkw.cn

TS:   nested.flat();
来源：http://ule.quarkkingdee.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vsu.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://ugg.yueranfly.top

Ruby: nested.flatten
来源：http://pwn.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xst.smart0.xyz

[D19] 按字段分组
来源：http://pqn.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://era.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iri.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bic.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gwp.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dal.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://vco.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://wgs.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bgo.tanke756.top

[D20] 统计每个元素出现次数
来源：http://xnr.hammf.cn

Py:   Counter(arr)
来源：http://cpb.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://jhr.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lkg.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://how.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://glw.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://qzo.ydjk.org.cn

Ruby: arr.tally
来源：http://hcx.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vnt.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://dqz.fktsv.cn

Py:   x in arr
来源：http://mix.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://cgg.jlsjyb.cn

JS:   arr.includes(x)
来源：http://jbd.birdmap.top

TS:   arr.includes(x)
来源：http://wlc.hongshengwenyu.top

Java: list.contains(x)
来源：http://nyw.quarkkingdee.top

Go:   slices.Contains(arr, x)
来源：http://jaz.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://slq.jianghu66.top

C#:   list.Contains(x)
来源：http://pps.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://fxk.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vzm.daria6918.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://req.jqgfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hby.nwbrower.top

TS:   [...arr];
来源：http://tnb.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://bca.jyoumei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xvh.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://xco.jlsjyb.cn

C#:   new List<int>(list);
来源：http://ewm.ydjk.org.cn

[D23] reduce 累积计算
来源：http://uzu.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ata.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://agk.quarkkingdee.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rep.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jtz.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://ezy.vqdsnc.cn

Go:   // 手写循环
来源：http://nxi.hammf.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://byp.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fdh.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://hyv.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lpk.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://glc.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qon.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://btk.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jux.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lzj.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ugx.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://asn.tanke756.top

[D25] Set 集合去重与交并差
来源：http://tub.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cdo.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dlf.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vdr.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uyo.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eel.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jmc.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jme.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yin.tianlin.xyz

[D26] 数组转字符串
来源：http://miv.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://pbj.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://obc.jyoumei.cn

JS:   arr.join(", ")
来源：http://tvm.gogol.net.cn

TS:   arr.join(", ")
来源：http://uil.dianchejie.cn

Java: String.join(", ", list)
来源：http://ynn.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://atl.andypj.xyz

Ruby: arr.join(", ")
来源：http://czi.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://wil.jiagoushi.top

================================================================================
来源：http://mnu.yanxiufei.cn

E. 字符串处理
来源：http://nkr.hongshengwenyu.top

================================================================================
来源：http://fxu.yonumen.top

[E01] 拼接字符串
来源：http://qho.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cfo.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wsl.bjfxy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vsz.smart0.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mzt.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vyj.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gkp.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aqp.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zip.jqgfzy.top

[E02] 重复字符串
来源：http://paj.jinghuilouyu.cn

Py:   "ab" * 3
来源：http://uoz.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://ial.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://pua.bbcook.cn

TS:   "ab".repeat(3)
来源：http://dee.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://cat.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://rye.ybcxt.top

Ruby: "ab" * 3
来源：http://gqk.jqgufenzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pzi.yonumen.top

[E03] 截取子串
来源：http://unx.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cwd.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sgk.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uxd.ivvv.top

TS:   s.slice(1, 4)
来源：http://zgk.tian-w.cn

Java: s.substring(1, 4)
来源：http://gqr.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gfu.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://lij.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://gfk.sweek.top

[E04] 查找子串位置
来源：http://zqc.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://jap.yvedp.cn

PHP:  strpos($s, "x");
来源：http://yzd.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://got.nwbrower.top

TS:   s.indexOf("x")
来源：http://vth.shuidangran.top

Java: s.indexOf("x")
来源：http://ybe.tarul.cn

Go:   strings.Index(s, "x")
来源：http://ozj.gaohongyu789.top

Ruby: s.index("x")
来源：http://lnf.zycfv.cn

C#:   s.IndexOf("x")
来源：http://ymr.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jrg.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jon.52xcode.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ehy.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hwu.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zpw.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mly.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://svi.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tuh.nanxuanxn.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xyz.xziqi.cn

[E06] 替换子串
来源：http://rsx.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pbn.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://fvn.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xmp.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://qhu.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://asl.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oqk.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rfr.guannengcc.top

C#:   s.Replace("a", "b")
来源：http://bav.sufxvd.cn

[E07] 按分隔符拆分
来源：http://goe.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uea.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vfl.hcnkem.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hgz.jinqigufen.top

TS:   s.split(",")
来源：http://aqc.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://oyh.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://faf.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://msn.tianlin.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rqs.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://pra.daria6918.cn

Py:   ",".join(items)
来源：http://fpi.cucudq.cn

PHP:  implode(",", $items);
来源：http://izl.sufxvd.cn

JS:   items.join(",")
来源：http://ctx.bjfxy.top

TS:   items.join(",")
来源：http://dzs.dashuyun.cn

Java: String.join(",", items)
来源：http://epg.uphjek.com

Go:   strings.Join(items, ",")
来源：http://nld.shangyingyoupin.top

Ruby: items.join(",")
来源：http://eni.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://tfi.cashguo.top

[E09] 去除所有空白字符
来源：http://qhz.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mhi.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zik.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://txo.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://bsu.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://mrg.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ghf.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://xbc.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kbz.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://hbu.jqgufenzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ufe.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ljp.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://eru.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://ewq.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://wou.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://abx.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xcm.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://omz.ppjwa.cn

[E11] 反转字符串
来源：http://osi.9152youxi.cn

Py:   s[::-1]
来源：http://ixr.chenlongwang.top

PHP:  strrev($s);
来源：http://ilz.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://vwx.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://ukr.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jld.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eor.sjlbkw.cn

Ruby: s.reverse
来源：http://rzy.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://nsn.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://bve.dashuyun.cn

Py:   s.count("a")
来源：http://fhf.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://prd.yfazqb.com

JS:   s.split("a").length - 1
来源：http://fpy.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://mlp.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tcj.aibaodan.cn

Go:   strings.Count(s, "a")
来源：http://kwg.chenlongwang.top

Ruby: s.count("a")
来源：http://ayp.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://dek.c1oappe.top

[E13] 逐字符遍历
来源：http://ngw.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://pnk.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ead.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://ohv.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yck.yuanzhike.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vdo.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mwf.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://nqt.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zeh.yongpay.top

[E14] URL 编码与 Base64
来源：http://wlm.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ewx.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bzy.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gfi.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eph.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://spx.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jzf.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qdo.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hex.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://znl.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mkj.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mxm.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jkc.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uem.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hns.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mbo.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nxe.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wkz.xuanzx.com

[E16] 数字千分位
来源：http://hok.fengsongda.top

Py:   f"{1234567:,}"
来源：http://gft.xuetiantiany.cn

PHP:  number_format(1234567);
来源：http://kup.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://wiq.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yzw.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jsd.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qwo.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ijq.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://udo.haohaochexian.top

[E17] 首字母大写
来源：http://oeu.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pkk.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gws.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eyy.jinqigfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bxy.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://guh.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://npl.cheryme.top

Ruby: s.capitalize
来源：http://ocb.jqgufenzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ntb.yuanzhike.top

[E18] 模板占位符替换
来源：http://gat.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ftb.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sxd.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zkr.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qvi.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://odu.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yho.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hqa.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ixf.ivvv.top

[E19] 多行文本按行拆分
来源：http://etq.shangyingyoupin.top

Py:   s.splitlines()
来源：http://tax.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://reg.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://iiz.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://kiz.jyoumei.cn

Java: s.lines().toList()
来源：http://tkf.cashguo.top

Go:   strings.Split(s, "\n")
来源：http://gsz.cqqwz.cn

Ruby: s.lines
来源：http://czf.zhijiandao.cn

C#:   s.Split('\n')
来源：http://sfa.yuxming.cn

[E20] 判断字符串是否为空
来源：http://bup.bbcook.cn

Py:   if not s:
来源：http://yov.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wew.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yoh.hywenlv.cn

TS:   if (s === "") {}
来源：http://tjm.0kj1m.cn

Java: if (s.isEmpty()) {}
来源：http://pow.ydjk.org.cn


<!-- 参考信息 -->