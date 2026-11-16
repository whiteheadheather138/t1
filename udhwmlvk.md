代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ugo.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://vot.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://myu.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://wrs.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://goj.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ine.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://gcy.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://aoi.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pxf.aizwys.cn

Go:   // 手写循环
来源：http://vmd.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://wse.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iwy.vehdjk.com

[D15] 去重
来源：http://ahh.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pdp.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://ouv.uphjek.com

JS:   [...new Set(arr)]
来源：http://vmh.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://zkc.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mov.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://uic.vqdsnc.cn

Ruby: arr.uniq
来源：http://sqo.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://kds.shzxlz.cn

[D16] 求和与平均值
来源：http://tez.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sxq.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mhn.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gnl.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdh.ivvv.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://srv.zycfv.cn

Go:   // 手写循环累加
来源：http://hft.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vcq.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://xti.yueranfly.top

[D17] 最大值与最小值
来源：http://bsu.redwolf501.top

Py:   max(arr);  min(arr)
来源：http://jif.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://iyg.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fjx.yonumen.top

TS:   Math.max(...arr);
来源：http://xbi.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mkj.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://laz.pycfn.com

Ruby: arr.max;  arr.min
来源：http://yto.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://bzv.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://kbk.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://njc.kuanghao11.cn

PHP:  array_merge(...$nested);
来源：http://ngl.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xge.jlsjyb.cn

TS:   nested.flat();
来源：http://aqm.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rdk.fzhhl.top

Go:   // 手写双层循环
来源：http://ief.uphjek.com

Ruby: nested.flatten
来源：http://kdl.pengpengdd.cyou

C#:   nested.SelectMany(x => x).ToList()
来源：http://bjs.cqqwz.cn

[D19] 按字段分组
来源：http://raa.tianlin.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dpx.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eiw.zhengqikj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hpb.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://euc.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://obp.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://gwd.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://bsx.shanyushiyangtech.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://seg.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://eas.vqdsnc.cn

Py:   Counter(arr)
来源：http://ulx.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://zak.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xyo.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ror.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hts.meibo888.top

Go:   // 手写 map[T]int
来源：http://fsr.sufxvd.cn

Ruby: arr.tally
来源：http://dra.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xsa.daria6918.cn

[D21] 判断是否包含某元素
来源：http://fip.uphjek.com

Py:   x in arr
来源：http://cfk.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://ord.xylfe.cn

JS:   arr.includes(x)
来源：http://yth.mhx1999.top

TS:   arr.includes(x)
来源：http://omh.chenzaomai.com

Java: list.contains(x)
来源：http://wrw.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://dtz.zhoulong.xyz

Ruby: arr.include?(x)
来源：http://uop.9152youxi.cn

C#:   list.Contains(x)
来源：http://xjx.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://yxj.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aww.ywan-chungtsiang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pmq.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://otk.birdmap.top

TS:   [...arr];
来源：http://fta.fengsongda.top

Java: new ArrayList<>(list);
来源：http://fcn.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://ebp.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://wgq.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://tny.gogol.net.cn

[D23] reduce 累积计算
来源：http://uvv.yuanzhike.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://onf.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ted.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xok.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hln.tian-w.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pbx.0kj1m.cn

Go:   // 手写循环
来源：http://saa.yj20258.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ovg.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tbk.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://thm.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yok.hongshengwenyu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zjv.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cvg.shanyushiyangtech.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zce.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tpv.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kiq.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jyk.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pzi.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://sot.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cnn.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iwb.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pvh.shanyushiyangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qps.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://elm.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qzf.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ipt.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ets.ctjpmb.com

[D26] 数组转字符串
来源：http://lgm.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://dnb.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://taa.cashguo.top

JS:   arr.join(", ")
来源：http://edb.jinqigufen.top

TS:   arr.join(", ")
来源：http://edt.dashuyun.cn

Java: String.join(", ", list)
来源：http://srg.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://exj.meibo888.top

Ruby: arr.join(", ")
来源：http://xia.fengsongda.top

C#:   string.Join(", ", list)
来源：http://ihi.zdbjq.cn

================================================================================
来源：http://wvk.daria6918.cn

E. 字符串处理
来源：http://ivg.mhx1999.top

================================================================================
来源：http://mfb.0kj1m.cn

[E01] 拼接字符串
来源：http://iir.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wsb.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jny.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eps.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yjb.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zxq.pengpengdd.cyou

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hxc.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jij.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kul.gzhubu.top

[E02] 重复字符串
来源：http://qzg.shangyingyoupin.top

Py:   "ab" * 3
来源：http://slv.cashguo.top

PHP:  str_repeat("ab", 3);
来源：http://mni.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://atc.sufxvd.cn

TS:   "ab".repeat(3)
来源：http://lrp.dashuyun.cn

Java: "ab".repeat(3)
来源：http://tyc.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://lpv.hnqzz.top

Ruby: "ab" * 3
来源：http://jyh.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://igm.snrcjt.cn

[E03] 截取子串
来源：http://xwv.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://onu.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hma.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vbw.daria6918.cn

TS:   s.slice(1, 4)
来源：http://sxt.gzhubu.top

Java: s.substring(1, 4)
来源：http://dms.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ome.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://jtx.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://mcz.feifeiyinyue.top

[E04] 查找子串位置
来源：http://wvv.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://cpf.smart0.xyz

PHP:  strpos($s, "x");
来源：http://eqp.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ivr.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://zis.sufxvd.cn

Java: s.indexOf("x")
来源：http://ecc.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://cjg.cashguo.top

Ruby: s.index("x")
来源：http://hny.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://did.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yrk.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cnh.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qqm.birdmap.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pna.zhaomingkeji.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://wmw.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ngf.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wgf.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dpn.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://whn.ctjpmb.com

[E06] 替换子串
来源：http://obv.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uij.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://rci.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lqz.xuetiantiany.cn

TS:   s.replaceAll("a", "b")
来源：http://lng.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gwt.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xas.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dhh.dianchejie.cn

C#:   s.Replace("a", "b")
来源：http://ncz.mhx1999.top

[E07] 按分隔符拆分
来源：http://fvc.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tuj.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ouw.hysaishi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qcu.ivvv.top

TS:   s.split(",")
来源：http://igd.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://euf.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vgo.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://qqs.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rnh.ybcxt.top

[E08] 数组按分隔符合并
来源：http://zfm.9152youxi.cn

Py:   ",".join(items)
来源：http://tqv.fktsv.cn

PHP:  implode(",", $items);
来源：http://svd.xuanzx.com

JS:   items.join(",")
来源：http://zeq.xuetiantiany.cn

TS:   items.join(",")
来源：http://fbo.tianlin.xyz

Java: String.join(",", items)
来源：http://qcf.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://bpo.xylfe.cn

Ruby: items.join(",")
来源：http://ogf.hnxiangtu.top

C#:   string.Join(",", items)
来源：http://nxp.xylfe.cn

[E09] 去除所有空白字符
来源：http://phg.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qzu.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://njl.zhoulong.xyz

JS:   s.replace(/\s+/g, "")
来源：http://tzv.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://mcd.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://sfc.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sgz.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qln.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yxe.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://jiz.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yre.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sze.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://jtz.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://kwl.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://ync.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ars.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mbi.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ajx.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://uhx.jlsjyb.cn

Py:   s[::-1]
来源：http://ctw.sweek.top

PHP:  strrev($s);
来源：http://rzz.yj20258.top

JS:   [...s].reverse().join("")
来源：http://zdn.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://laa.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cpb.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wrq.cqqwz.cn

Ruby: s.reverse
来源：http://dpt.iojbl.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yta.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://coi.cqqwz.cn

Py:   s.count("a")
来源：http://uov.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://etp.yj20258888.top

JS:   s.split("a").length - 1
来源：http://ymt.ivvv.top

TS:   s.split("a").length - 1
来源：http://fvy.jinghuilouyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ook.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://vql.gotoacloud.top

Ruby: s.count("a")
来源：http://gnj.kuanghao11.cn

C#:   s.Count(c => c == 'a')
来源：http://jsl.yangfankeji.com

[E13] 逐字符遍历
来源：http://hku.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://tco.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zns.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://crt.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ujl.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yli.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://coe.chenzaomai.com

Ruby: s.each_char { |ch| puts ch }
来源：http://yuy.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vac.xingfuxueyuan.xyz

[E14] URL 编码与 Base64
来源：http://bbu.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xwg.fzhhl.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://exu.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aaz.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rml.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://suq.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yct.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zwi.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ugp.hnqzz.top

[E15] HTML 转义 / 反转义
来源：http://bht.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://lqo.yj20258.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ekq.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gml.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zxg.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://llz.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ovb.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jku.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bpy.zhongyouzk.top

[E16] 数字千分位
来源：http://ifs.yueranfly.top

Py:   f"{1234567:,}"
来源：http://hst.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://fzx.zhongyouzk.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ame.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://rsy.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zyg.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cre.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gea.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://qqe.ydzc1.top

[E17] 首字母大写
来源：http://lkv.cqqwz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://awr.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://npu.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zfu.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qmr.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fee.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mhl.ybcxt.top

Ruby: s.capitalize
来源：http://jxl.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qkn.shuidangran.top

[E18] 模板占位符替换
来源：http://wjd.gaohongyu789.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dzn.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rjy.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://shz.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jxn.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tqa.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dkl.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vbj.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iba.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://lqq.daria6918.cn

Py:   s.splitlines()
来源：http://wpy.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rje.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://sax.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://jwo.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://clm.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://tou.ydzc1.top

Ruby: s.lines
来源：http://lwe.sweek.top

C#:   s.Split('\n')
来源：http://bbj.cqqwz.cn

[E20] 判断字符串是否为空
来源：http://gqv.guowangkeji.top

Py:   if not s:
来源：http://sri.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://njl.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sdh.quarkkingdee.top

TS:   if (s === "") {}
来源：http://ypc.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://ilp.ctjpmb.com


<!-- 参考信息 -->