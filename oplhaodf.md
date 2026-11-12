代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://suc.pycfn.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pon.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://jqh.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://ptf.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bra.ybcxt.top

Go:   // 手写循环
来源：http://cik.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sdv.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lsc.nwbrower.top

[D15] 去重
来源：http://fcm.ydzc1.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wre.yanxiufei.cn

PHP:  array_unique($arr);
来源：http://spn.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://dsk.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://kbn.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qtg.fktsv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ock.meibo888.top

Ruby: arr.uniq
来源：http://igt.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://aai.jlsjyb.cn

[D16] 求和与平均值
来源：http://sao.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bke.redwolf501.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://asm.pengpengdd.cyou

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kgk.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nkr.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ebd.gaohongyu789.top

Go:   // 手写循环累加
来源：http://mqp.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bpu.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://rfp.fengsongda.top

[D17] 最大值与最小值
来源：http://das.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://jlw.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://mjs.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ync.shuidangran.top

TS:   Math.max(...arr);
来源：http://qul.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xyn.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ghx.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://wvy.zhongyouzk.top

C#:   list.Max();  list.Min()
来源：http://bvl.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://bag.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cmi.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://ime.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gcx.jqgfzy.top

TS:   nested.flat();
来源：http://kmb.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gag.zhijiandao.cn

Go:   // 手写双层循环
来源：http://ivz.yueranfly.top

Ruby: nested.flatten
来源：http://tlc.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://blu.sxryk.cn

[D19] 按字段分组
来源：http://pks.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://etx.yuxming.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bvh.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rrr.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://nvl.zhoulong.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://few.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://xhz.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://exz.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xli.cashguo.top

[D20] 统计每个元素出现次数
来源：http://ryc.feifeiyinyue.top

Py:   Counter(arr)
来源：http://xvj.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://mey.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kgb.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gud.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xab.yvedp.cn

Go:   // 手写 map[T]int
来源：http://eea.jiagoushi.top

Ruby: arr.tally
来源：http://kab.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sbw.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://uma.yj20258.top

Py:   x in arr
来源：http://ndw.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://fzm.hfpthk.cn

JS:   arr.includes(x)
来源：http://tls.yfazqb.com

TS:   arr.includes(x)
来源：http://wte.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://fcm.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://keh.xuanzx.com

Ruby: arr.include?(x)
来源：http://dlz.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://vni.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://wix.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://phy.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dfa.jqgfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://exq.ybcxt.top

TS:   [...arr];
来源：http://pta.meibo888.top

Java: new ArrayList<>(list);
来源：http://owz.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://qht.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://zrs.ydjk.org.cn

C#:   new List<int>(list);
来源：http://mvt.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://bsr.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wmj.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kwf.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyx.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://atg.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ekl.ydjk.org.cn

Go:   // 手写循环
来源：http://gft.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://obs.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rin.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://qib.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xkw.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qgz.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tss.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hfc.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dfz.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zwh.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://twj.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://laa.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://isi.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pia.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hlk.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ukf.hcnkem.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qqd.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hlj.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://txu.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cro.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://omy.cashguo.top

[D26] 数组转字符串
来源：http://lrk.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://mjq.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://jbk.vqdsnc.cn

JS:   arr.join(", ")
来源：http://omx.shuidangran.top

TS:   arr.join(", ")
来源：http://ncu.fktsv.cn

Java: String.join(", ", list)
来源：http://pto.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://wfx.cqqwz.cn

Ruby: arr.join(", ")
来源：http://drw.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://wbz.hammf.cn

================================================================================
来源：http://bzc.jinqigufen.top

E. 字符串处理
来源：http://egp.iojbl.cn

================================================================================
来源：http://wgi.fzhhl.top

[E01] 拼接字符串
来源：http://fve.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vtx.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nhy.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cci.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fve.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ycp.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cxp.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bpg.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://toz.xuetiantiany.cn

[E02] 重复字符串
来源：http://asn.fzhhl.top

Py:   "ab" * 3
来源：http://kkx.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://okv.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://msr.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://icc.fktsv.cn

Java: "ab".repeat(3)
来源：http://bmo.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://zfg.aibaodan.cn

Ruby: "ab" * 3
来源：http://dmi.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://feo.cqqwz.cn

[E03] 截取子串
来源：http://kze.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lqq.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vvt.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mcu.bjfxy.top

TS:   s.slice(1, 4)
来源：http://wyl.daria6918.cn

Java: s.substring(1, 4)
来源：http://uiq.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ivk.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://pjm.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://gfz.chenjidiqi.icu

[E04] 查找子串位置
来源：http://olq.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://uyw.gzhubu.top

PHP:  strpos($s, "x");
来源：http://kuh.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ijo.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://pcw.dashuyun.cn

Java: s.indexOf("x")
来源：http://rvo.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://sit.vqdsnc.cn

Ruby: s.index("x")
来源：http://dkm.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://pyo.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://xkr.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nil.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uzo.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wxy.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gdr.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://soq.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zyg.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blx.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://btf.jinqigufen.top

[E06] 替换子串
来源：http://yfx.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://acp.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://rxq.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qip.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://yxj.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://whs.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qmv.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mnp.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://wjp.jyoumei.cn

[E07] 按分隔符拆分
来源：http://gsm.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dsc.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lhc.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://amg.ydzc1.top

TS:   s.split(",")
来源：http://kzd.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yzd.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vzc.jinghuilouyu.cn

Ruby: s.split(",");  s.split
来源：http://vxt.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ylh.aizwys.cn

[E08] 数组按分隔符合并
来源：http://wsq.feifeiyinyue.top

Py:   ",".join(items)
来源：http://ahj.haohaochexian.top

PHP:  implode(",", $items);
来源：http://udm.fanxiaobao.xyz

JS:   items.join(",")
来源：http://yak.gaohongyu789.top

TS:   items.join(",")
来源：http://fdc.fktsv.cn

Java: String.join(",", items)
来源：http://kel.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://jnb.zhongyouzk.top

Ruby: items.join(",")
来源：http://nef.sweek.top

C#:   string.Join(",", items)
来源：http://raf.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://lnn.nanxuanxn.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ssd.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tuo.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ctx.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://vcl.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ety.yj20258888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xsj.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zfk.nanxuanxn.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mbr.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://jvz.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zeg.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://snj.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://lfm.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://boq.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://dgo.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yli.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ska.xingfuxueyuan.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mhw.fktsv.cn

[E11] 反转字符串
来源：http://ofm.yongpay.top

Py:   s[::-1]
来源：http://kof.shangyingyoupin.top

PHP:  strrev($s);
来源：http://ppq.vqdsnc.cn

JS:   [...s].reverse().join("")
来源：http://vcl.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://zcv.ctjpmb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://rpm.epnwcf.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://eug.aibaodan.cn

Ruby: s.reverse
来源：http://xpp.sysykeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://qcp.hongshengwenyu.top

[E12] 统计某字符出现次数
来源：http://txw.zdbjq.cn

Py:   s.count("a")
来源：http://pre.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://exh.vehdjk.com

JS:   s.split("a").length - 1
来源：http://wre.cashguo.top

TS:   s.split("a").length - 1
来源：http://ylc.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ihc.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://tlx.hcnkem.com

Ruby: s.count("a")
来源：http://enx.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://pxp.zycfv.cn

[E13] 逐字符遍历
来源：http://tin.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://knx.zhaomingkeji.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wjn.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mkd.daria6918.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kek.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xui.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qly.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://tnw.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qqw.316326.xyz

[E14] URL 编码与 Base64
来源：http://dwb.tianlin.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ehl.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ftx.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ugj.kuanghao11.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gtd.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wkm.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cxb.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qwp.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dbx.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://ovv.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://svg.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zov.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qjq.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://woq.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lls.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yol.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://srj.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xxu.yueranfly.top

[E16] 数字千分位
来源：http://asr.ybcxt.top

Py:   f"{1234567:,}"
来源：http://jpt.yuxming.cn

PHP:  number_format(1234567);
来源：http://fnr.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mwk.jlsjyb.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zpz.gogol.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jcq.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pxc.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zkl.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://iqq.dianchejie.cn

[E17] 首字母大写
来源：http://ecf.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ofd.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://muj.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lyc.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eyf.chenzaomai.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mgj.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dab.shangyingyoupin.top

Ruby: s.capitalize
来源：http://dno.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ywn.bjfxy.top

[E18] 模板占位符替换
来源：http://jlp.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cjw.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qsv.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vxp.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fey.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rsw.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oge.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ewm.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://saa.yj20258.top

[E19] 多行文本按行拆分
来源：http://jnp.sjlbkw.cn

Py:   s.splitlines()
来源：http://fuv.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fbv.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://yyt.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://lgc.ybcxt.top

Java: s.lines().toList()
来源：http://lzm.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://xsd.fanxiaobao.xyz

Ruby: s.lines
来源：http://rxf.cashguo.top

C#:   s.Split('\n')
来源：http://cfg.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://uub.ydjk.org.cn

Py:   if not s:
来源：http://riw.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yln.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://coj.hfpthk.cn

TS:   if (s === "") {}
来源：http://zvx.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://uae.daxiang520.top

Go:   if s == "" {}
来源：http://wfp.zycfv.cn

Ruby: if s.empty?
来源：http://der.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://amo.gotoacloud.top

[E21] 超长截断加省略号
来源：http://bnc.wangshuangyany.cn


<!-- 参考信息 -->