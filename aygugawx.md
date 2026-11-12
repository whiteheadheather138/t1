代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://sks.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uaz.hcnkem.com

TS:   Math.max(...arr);
来源：http://stj.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ufy.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://njr.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://yjs.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://dmy.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://bjx.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xki.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://myy.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://irl.ybcxt.top

TS:   nested.flat();
来源：http://giv.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mwg.snrcjt.cn

Go:   // 手写双层循环
来源：http://kni.fktsv.cn

Ruby: nested.flatten
来源：http://hgw.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://yze.xinyue.icu

[D19] 按字段分组
来源：http://gwh.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://giq.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uaw.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://thc.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://thx.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pdp.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://xsg.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xoz.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vyt.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://oeo.ydjk.org.cn

Py:   Counter(arr)
来源：http://wde.xinyue.icu

PHP:  array_count_values($arr);
来源：http://ali.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://alb.jqgfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cxn.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ucw.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://uqr.redwolf501.top

Ruby: arr.tally
来源：http://dvo.xinyue.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zhm.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://elf.shanyushiyangkeji.top

Py:   x in arr
来源：http://upn.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://gii.guannengcc.top

JS:   arr.includes(x)
来源：http://tnt.ivvv.top

TS:   arr.includes(x)
来源：http://dwi.xylfe.cn

Java: list.contains(x)
来源：http://xoe.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://frr.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://cdx.cdnleiting.top

C#:   list.Contains(x)
来源：http://dgc.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://qlv.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://djl.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://udt.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gti.ivvv.top

TS:   [...arr];
来源：http://xdv.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://qhk.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ajs.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://kic.daria6918.cn

C#:   new List<int>(list);
来源：http://hli.fengsongda.top

[D23] reduce 累积计算
来源：http://dfb.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://grg.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ekg.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpw.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vet.zhongyouzk.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dko.gotoacloud.top

Go:   // 手写循环
来源：http://vvg.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lul.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nxe.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://jhy.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bby.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iud.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://myf.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wbp.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ykk.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nmw.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vpe.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ddm.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://kbd.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hke.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qrr.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xgb.yueranfly.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dra.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jec.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://whk.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qtt.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hwo.cucudq.cn

[D26] 数组转字符串
来源：http://rau.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://uwy.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://ori.yvedp.cn

JS:   arr.join(", ")
来源：http://cia.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://anq.gzhubu.top

Java: String.join(", ", list)
来源：http://wdw.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://okn.ybcxt.top

Ruby: arr.join(", ")
来源：http://dts.vehdjk.com

C#:   string.Join(", ", list)
来源：http://fbd.yuxming.cn

================================================================================
来源：http://jlw.cheryme.top

E. 字符串处理
来源：http://gum.fengsongda.top

================================================================================
来源：http://znk.hongshengwenyu.top

[E01] 拼接字符串
来源：http://hlp.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://loc.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pqh.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gfq.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zcq.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qgq.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rdt.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wyc.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nnf.jiagoushi.top

[E02] 重复字符串
来源：http://izs.pycfn.com

Py:   "ab" * 3
来源：http://ctg.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://ske.shuidangran.top

JS:   "ab".repeat(3)
来源：http://eyu.cucudq.cn

TS:   "ab".repeat(3)
来源：http://fpa.dashuyun.cn

Java: "ab".repeat(3)
来源：http://zlu.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://dzy.andypj.xyz

Ruby: "ab" * 3
来源：http://aod.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://erh.jinqigufen.top

[E03] 截取子串
来源：http://wfk.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zom.pengpengdd.cyou

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zqq.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pua.daxiang520.top

TS:   s.slice(1, 4)
来源：http://rby.birdmap.top

Java: s.substring(1, 4)
来源：http://keq.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://trj.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://etj.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://jjq.tian-w.cn

[E04] 查找子串位置
来源：http://dim.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://jxa.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://ewc.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ikl.hesvh.cn

TS:   s.indexOf("x")
来源：http://qth.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://clj.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://ogn.bbcook.cn

Ruby: s.index("x")
来源：http://fzs.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://wuc.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://msa.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://syd.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aie.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://swm.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pji.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wng.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ipm.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eju.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hfx.fzhhl.top

[E06] 替换子串
来源：http://bpm.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jbg.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://qqi.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://umo.iojbl.cn

TS:   s.replaceAll("a", "b")
来源：http://fay.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ydx.ydzc1.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://voq.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://plz.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://ouy.bjfxy.top

[E07] 按分隔符拆分
来源：http://guh.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://voa.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zbp.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://liv.fanxiaobao.xyz

TS:   s.split(",")
来源：http://egp.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://fnh.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ahj.316326.xyz

Ruby: s.split(",");  s.split
来源：http://drj.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zzl.fengsongda.top

[E08] 数组按分隔符合并
来源：http://xdk.zdbjq.cn

Py:   ",".join(items)
来源：http://mob.ctjpmb.com

PHP:  implode(",", $items);
来源：http://xby.jqgfzy.top

JS:   items.join(",")
来源：http://dbw.tianlin.xyz

TS:   items.join(",")
来源：http://hpv.zhengqikj.top

Java: String.join(",", items)
来源：http://kqd.havefunace.top

Go:   strings.Join(items, ",")
来源：http://eru.yonumen.top

Ruby: items.join(",")
来源：http://bam.smart0.xyz

C#:   string.Join(",", items)
来源：http://xyj.zhixingplan.top

[E09] 去除所有空白字符
来源：http://ciw.zhixingplan.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jfh.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xnu.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://gyb.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://phi.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://ize.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://jle.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://rfr.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eju.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://riz.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ykm.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mtb.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://oqv.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://gap.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://mlb.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://paw.jinqigfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ear.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zzh.hammf.cn

[E11] 反转字符串
来源：http://iub.cucudq.cn

Py:   s[::-1]
来源：http://lli.chenzaomai.com

PHP:  strrev($s);
来源：http://wcl.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://gec.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://qts.shanyushiyangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vcw.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ilm.zdqjudy.top

Ruby: s.reverse
来源：http://hpk.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://hom.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://vgo.xuanzx.com

Py:   s.count("a")
来源：http://oym.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://yyt.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://dqy.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://ong.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jsx.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://ymn.jqgufenzy.top

Ruby: s.count("a")
来源：http://boi.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://kmr.cqqwz.cn

[E13] 逐字符遍历
来源：http://vdf.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://hlf.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pos.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dnj.cheryme.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://evr.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kqs.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fbj.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ihs.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pqe.smart0.xyz

[E14] URL 编码与 Base64
来源：http://ibg.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ckw.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dbm.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xvs.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vpq.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qoh.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://isu.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kty.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wsg.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://oap.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cpi.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xks.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cca.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://phm.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hhi.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jzq.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dnt.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vwc.ctjpmb.com

[E16] 数字千分位
来源：http://zgm.redwolf501.top

Py:   f"{1234567:,}"
来源：http://mcj.sxryk.cn

PHP:  number_format(1234567);
来源：http://twa.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://get.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oxs.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mrm.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xsn.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nkl.iojbl.cn

C#:   1234567.ToString("N0")
来源：http://owc.cashguo.top

[E17] 首字母大写
来源：http://pxb.daria6918.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xrk.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://ihx.pycfn.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vob.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hnj.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eaz.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gmx.shanyushiyangkeji.top

Ruby: s.capitalize
来源：http://cjm.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yyd.smart0.xyz

[E18] 模板占位符替换
来源：http://jbj.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kpt.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hwy.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://ums.zhongyouzk.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tkc.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bpk.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://siu.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bhk.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://azz.sxryk.cn

[E19] 多行文本按行拆分
来源：http://dwi.nwbrower.top

Py:   s.splitlines()
来源：http://zng.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nzb.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://pea.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://bqv.wangshuangyany.cn

Java: s.lines().toList()
来源：http://hhr.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://ykl.cucudq.cn

Ruby: s.lines
来源：http://cwp.smart0.xyz

C#:   s.Split('\n')
来源：http://kdv.yj202588.top

[E20] 判断字符串是否为空
来源：http://dxw.birdmap.top

Py:   if not s:
来源：http://zpx.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zju.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xix.sysykeji.top

TS:   if (s === "") {}
来源：http://dxi.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://rae.jlsjyb.cn

Go:   if s == "" {}
来源：http://nju.hfpthk.cn

Ruby: if s.empty?
来源：http://dfe.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vhf.tianlin.xyz

[E21] 超长截断加省略号
来源：http://rmc.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sok.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wlh.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pbg.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dzp.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qzb.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://uoe.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dqq.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dis.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://ekp.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://roi.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dsd.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lpa.nanxinkj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://akg.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kef.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lbe.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://hpn.hnqzz.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tfg.vqdsnc.cn

================================================================================
来源：http://zrg.yangfankeji.com

F. 文件与目录
来源：http://swd.ydjk.org.cn

================================================================================
来源：http://uvu.jqgufenzy.top

[F01] 读取整个文件
来源：http://fqf.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kre.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://lms.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jfs.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ahf.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qdq.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ejl.cucudq.cn

Ruby: File.read("a.txt")
来源：http://qbl.shangyingyoupin.top


<!-- 参考信息 -->