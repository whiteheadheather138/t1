代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nrs.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://bwp.ybcxt.top

[D17] 最大值与最小值
来源：http://mdy.hammf.cn

Py:   max(arr);  min(arr)
来源：http://bqm.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://kba.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hgo.cdnleiting.top

TS:   Math.max(...arr);
来源：http://lod.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://fuw.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ovq.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://pdm.cdnleiting.top

C#:   list.Max();  list.Min()
来源：http://rhe.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://anh.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nrk.havefunace.top

PHP:  array_merge(...$nested);
来源：http://qbn.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ezo.jqgfzy.top

TS:   nested.flat();
来源：http://blp.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qvu.yuanzhike.top

Go:   // 手写双层循环
来源：http://fxd.yanxiufei.cn

Ruby: nested.flatten
来源：http://tin.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hhk.chenlongwang.top

[D19] 按字段分组
来源：http://nbh.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oso.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dqi.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fdy.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jdi.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ezk.yfazqb.com

Go:   // 手写 map[string][]T
来源：http://oxf.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pnd.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tos.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://oaa.nanxuanxn.top

Py:   Counter(arr)
来源：http://lgd.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://jfe.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wbe.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fkj.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bkv.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://agg.jyoumei.cn

Ruby: arr.tally
来源：http://rey.meibo888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yfs.fzhhl.top

[D21] 判断是否包含某元素
来源：http://eke.yj20258888.top

Py:   x in arr
来源：http://alb.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://gbk.epnwcf.com

JS:   arr.includes(x)
来源：http://lvm.andypj.xyz

TS:   arr.includes(x)
来源：http://ijz.birdmap.top

Java: list.contains(x)
来源：http://dbo.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://ffg.bbcook.cn

Ruby: arr.include?(x)
来源：http://skr.ydzc1.top

C#:   list.Contains(x)
来源：http://lsw.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://nav.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://enn.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rol.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kbf.yonumen.top

TS:   [...arr];
来源：http://ytf.yj20258.top

Java: new ArrayList<>(list);
来源：http://yqc.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://hgz.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://wxa.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://oze.fzhhl.top

[D23] reduce 累积计算
来源：http://ypy.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tnq.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ecc.zycfv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iad.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oei.yvedp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rtl.nanxinkj.top

Go:   // 手写循环
来源：http://kco.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zlh.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pff.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://qfy.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bnq.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ilq.c1oappe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vgk.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rsw.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qtn.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wdz.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://thp.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tyl.meibo888.top

[D25] Set 集合去重与交并差
来源：http://yvc.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://auo.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sth.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yub.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blv.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cnc.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zqq.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ntg.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lmf.zhoulong.xyz

[D26] 数组转字符串
来源：http://uph.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://hxn.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://hen.andypj.xyz

JS:   arr.join(", ")
来源：http://usc.yfazqb.com

TS:   arr.join(", ")
来源：http://cih.dianchejie.cn

Java: String.join(", ", list)
来源：http://axp.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://tuk.xingfuxueyuan.xyz

Ruby: arr.join(", ")
来源：http://rkb.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://gvc.cdnleiting.top

================================================================================
来源：http://aiq.smart0.xyz

E. 字符串处理
来源：http://vnr.sysykeji.top

================================================================================
来源：http://pxj.hcnkem.com

[E01] 拼接字符串
来源：http://stx.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qwy.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xcj.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ypv.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nrg.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qgz.snrcjt.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hdo.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://orf.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ixb.hnxiangtu.top

[E02] 重复字符串
来源：http://hzt.hesvh.cn

Py:   "ab" * 3
来源：http://sya.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://tiv.havefunace.top

JS:   "ab".repeat(3)
来源：http://xhj.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://lke.fengsongda.top

Java: "ab".repeat(3)
来源：http://ozb.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://isx.yfazqb.com

Ruby: "ab" * 3
来源：http://mkk.shangyingyoupin.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fym.jinqigufen.top

[E03] 截取子串
来源：http://kap.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jva.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pgs.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://foh.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://yuv.redwolf501.top

Java: s.substring(1, 4)
来源：http://qee.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iad.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://web.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://gbi.jqgufenzy.top

[E04] 查找子串位置
来源：http://fkv.sufxvd.cn

Py:   s.find("x");  s.index("x")
来源：http://byh.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://tkw.vqdsnc.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bme.jianghu66.top

TS:   s.indexOf("x")
来源：http://heh.hnxiangtu.top

Java: s.indexOf("x")
来源：http://dem.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://lol.redwolf501.top

Ruby: s.index("x")
来源：http://mtp.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://svn.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wyn.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vzp.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nyt.xinyue.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pzj.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qgv.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://elh.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eaa.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oji.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nme.yuxming.cn

[E06] 替换子串
来源：http://emi.hywenlv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://keh.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://yds.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://weh.uphjek.com

TS:   s.replaceAll("a", "b")
来源：http://vbl.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zqe.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ryz.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://htk.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://dxh.zycfv.cn

[E07] 按分隔符拆分
来源：http://fkv.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zwz.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fic.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wai.chenlongwang.top

TS:   s.split(",")
来源：http://vuy.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://wvg.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wmq.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://mfj.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yhz.hesvh.cn

[E08] 数组按分隔符合并
来源：http://voy.meibo888.top

Py:   ",".join(items)
来源：http://kzz.guannengcc.top

PHP:  implode(",", $items);
来源：http://nod.guowangkeji.top

JS:   items.join(",")
来源：http://idg.ctjpmb.com

TS:   items.join(",")
来源：http://dkk.9152youxi.cn

Java: String.join(",", items)
来源：http://ebr.havefunace.top

Go:   strings.Join(items, ",")
来源：http://dyg.jinyuanbaomall.cn

Ruby: items.join(",")
来源：http://jsf.ybcxt.top

C#:   string.Join(",", items)
来源：http://tfo.tian-w.cn

[E09] 去除所有空白字符
来源：http://hpx.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gfv.cashguo.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wqg.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://obj.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://nzs.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://pdt.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tff.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://uea.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bxn.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://yzs.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yth.chenjidiqi.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://osg.gzhubu.top

JS:   "7".padStart(3, "0")
来源：http://edz.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://yig.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://jrf.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ufa.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://esf.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mol.birdmap.top

[E11] 反转字符串
来源：http://lwu.wangshuangyany.cn

Py:   s[::-1]
来源：http://sjp.snrcjt.cn

PHP:  strrev($s);
来源：http://rso.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://iqu.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://pmx.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tcw.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kqt.nanxinkj.top

Ruby: s.reverse
来源：http://zwk.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://lid.guannengcc.top

[E12] 统计某字符出现次数
来源：http://kvh.iojbl.cn

Py:   s.count("a")
来源：http://nov.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://blb.cheryme.top

JS:   s.split("a").length - 1
来源：http://djv.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://wjq.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hgt.wangshuangyany.cn

Go:   strings.Count(s, "a")
来源：http://khx.tarul.cn

Ruby: s.count("a")
来源：http://ozn.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://svz.yueranfly.top

[E13] 逐字符遍历
来源：http://xwa.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://dha.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zjm.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://xmr.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wui.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bak.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zqi.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://haq.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dak.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://pko.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yky.smart0.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ykk.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bxs.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rxp.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mnv.cheryme.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://esb.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zdr.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://shx.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://bat.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ads.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://usw.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wty.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qrd.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pgi.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uih.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ana.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://csv.birdmap.top

[E16] 数字千分位
来源：http://ufu.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://nwe.nanxinkj.top

PHP:  number_format(1234567);
来源：http://nfy.hnxiangtu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://myn.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qsy.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hza.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bvh.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ffp.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://hng.daxiang520.top

[E17] 首字母大写
来源：http://hac.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mnc.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://usp.jqgfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cvt.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kzl.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xxt.dashuyun.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ftx.nanxinkj.top

Ruby: s.capitalize
来源：http://pxi.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://caa.wangdashe.top

[E18] 模板占位符替换
来源：http://hsp.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://awn.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jot.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uvj.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tsu.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eiy.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bey.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ggy.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hhq.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://cby.dashuyun.cn

Py:   s.splitlines()
来源：http://pau.zhoulong.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wcf.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://xgc.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://vli.vehdjk.com

Java: s.lines().toList()
来源：http://lmc.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://vmd.hongshengwenyu.top

Ruby: s.lines
来源：http://mmd.0kj1m.cn

C#:   s.Split('\n')
来源：http://pee.pycfn.com

[E20] 判断字符串是否为空
来源：http://dsh.jlsjyb.cn

Py:   if not s:
来源：http://ccv.daria6918.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fms.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rxo.9152youxi.cn

TS:   if (s === "") {}
来源：http://qvq.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://szz.zdqjudy.top

Go:   if s == "" {}
来源：http://dlb.daxiang520.top

Ruby: if s.empty?
来源：http://fgl.zdqjudy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lhn.fehbvm.com

[E21] 超长截断加省略号
来源：http://sgs.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pfz.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://urj.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fhf.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://luf.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pte.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://fcw.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cub.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yad.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://ije.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jin.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jpp.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eib.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://grv.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kjt.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rrx.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://mkx.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cie.hongshengwenyu.top

================================================================================
来源：http://lhw.zhoulong.xyz

F. 文件与目录
来源：http://djs.zhijiandao.cn

================================================================================
来源：http://div.52xcode.cn

[F01] 读取整个文件
来源：http://atx.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://thq.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://tvz.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://riq.yfazqb.com


<!-- 参考信息 -->