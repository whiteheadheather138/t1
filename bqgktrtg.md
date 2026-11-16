代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ksb.hywenlv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ufq.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uxn.meibo888.top

Go:   // 手写循环累加
来源：http://dba.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sbt.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://ach.jqgfzy.top

[D17] 最大值与最小值
来源：http://sye.tarul.cn

Py:   max(arr);  min(arr)
来源：http://utp.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://ujh.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hxl.fzhhl.top

TS:   Math.max(...arr);
来源：http://yia.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lqt.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lcx.yj202588.top

Ruby: arr.max;  arr.min
来源：http://xzl.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://fbu.316326.xyz

[D18] 扁平化嵌套数组
来源：http://vls.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ayr.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://irq.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://npr.zhengqikj.top

TS:   nested.flat();
来源：http://bet.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ymy.zdqjudy.top

Go:   // 手写双层循环
来源：http://wuo.havefunace.top

Ruby: nested.flatten
来源：http://ckg.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hwk.hfpthk.cn

[D19] 按字段分组
来源：http://zse.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ist.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://whs.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jxz.epnwcf.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hrr.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rai.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://bwt.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://vyx.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dvj.ivvv.top

[D20] 统计每个元素出现次数
来源：http://xsg.smart0.xyz

Py:   Counter(arr)
来源：http://leb.nwbrower.top

PHP:  array_count_values($arr);
来源：http://lym.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lyu.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uxu.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bxo.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://ris.sxryk.cn

Ruby: arr.tally
来源：http://jdj.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bin.shanyushiyangkeji.top

[D21] 判断是否包含某元素
来源：http://wod.sufxvd.cn

Py:   x in arr
来源：http://cot.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://ggm.fehbvm.com

JS:   arr.includes(x)
来源：http://mnr.kuanghao11.cn

TS:   arr.includes(x)
来源：http://kbc.hongshengwenyu.top

Java: list.contains(x)
来源：http://shi.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://ore.yanxiufei.cn

Ruby: arr.include?(x)
来源：http://gkg.dianchejie.cn

C#:   list.Contains(x)
来源：http://csc.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://lfn.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wfy.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lhc.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oku.chenzaomai.com

TS:   [...arr];
来源：http://fuo.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://hjk.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://wwb.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://mkj.hysaishi.cn

C#:   new List<int>(list);
来源：http://ele.uphjek.com

[D23] reduce 累积计算
来源：http://fkr.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ltp.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kbv.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qne.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ukl.jqgufenzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uzz.yuanzhike.top

Go:   // 手写循环
来源：http://dpo.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dxk.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ucj.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://gyz.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ftr.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sxv.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yoj.cucudq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dxm.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kvv.nwbrower.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bwr.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hph.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qzr.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://sbh.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rad.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eiv.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dyk.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uge.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pxk.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mui.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pkk.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ezp.cheryme.top

[D26] 数组转字符串
来源：http://yjj.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://ibt.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://rin.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://xer.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://wzg.chenzaomai.com

Java: String.join(", ", list)
来源：http://hgx.shuidangran.top

Go:   strings.Join(strs, ", ")
来源：http://mli.hfpthk.cn

Ruby: arr.join(", ")
来源：http://exe.shuidangran.top

C#:   string.Join(", ", list)
来源：http://etl.cucudq.cn

================================================================================
来源：http://kzp.316326.xyz

E. 字符串处理
来源：http://phn.wangshuangyany.cn

================================================================================
来源：http://lgj.9152youxi.cn

[E01] 拼接字符串
来源：http://mwa.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uom.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sif.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nln.ivvv.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qkr.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vlw.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yks.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://siu.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://obg.jianghu66.top

[E02] 重复字符串
来源：http://lxp.ydjk.org.cn

Py:   "ab" * 3
来源：http://cfv.jinyuanbaomall.cn

PHP:  str_repeat("ab", 3);
来源：http://cdl.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://dwl.yvedp.cn

TS:   "ab".repeat(3)
来源：http://yab.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://xud.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://unm.shzxlz.cn

Ruby: "ab" * 3
来源：http://oui.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qpy.chenzaomai.com

[E03] 截取子串
来源：http://hsv.yj202588.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ain.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sdo.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qhf.bjfxy.top

TS:   s.slice(1, 4)
来源：http://cfv.ivvv.top

Java: s.substring(1, 4)
来源：http://zex.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tlt.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://xqu.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://bjg.cdnleiting.top

[E04] 查找子串位置
来源：http://lqv.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://ctw.hammf.cn

PHP:  strpos($s, "x");
来源：http://exo.zhaomingkeji.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hce.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://vvn.sufxvd.cn

Java: s.indexOf("x")
来源：http://ynm.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://dgf.c1oappe.top

Ruby: s.index("x")
来源：http://nmi.yfazqb.com

C#:   s.IndexOf("x")
来源：http://pta.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ajp.yj20258.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dgy.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mcx.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://una.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qgy.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zij.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cxb.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://swi.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hxh.daria6918.cn

[E06] 替换子串
来源：http://tez.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cvj.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://tqy.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://crn.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://jtt.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qjc.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qak.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ygg.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://wfg.yangfankeji.com

[E07] 按分隔符拆分
来源：http://fah.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mro.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wfl.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://dpm.cqqwz.cn

TS:   s.split(",")
来源：http://ime.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://owb.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zrh.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://efp.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iil.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://bib.feifeiyinyue.top

Py:   ",".join(items)
来源：http://elm.dianchejie.cn

PHP:  implode(",", $items);
来源：http://xtd.zycfv.cn

JS:   items.join(",")
来源：http://kqr.daria6918.cn

TS:   items.join(",")
来源：http://cls.hysaishi.cn

Java: String.join(",", items)
来源：http://ras.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://yha.smart0.xyz

Ruby: items.join(",")
来源：http://wbz.hfpthk.cn

C#:   string.Join(",", items)
来源：http://jkx.yj20258888.top

[E09] 去除所有空白字符
来源：http://ymc.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rgg.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ffb.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://diw.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://vtf.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://acr.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xoy.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://pzu.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lew.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://pat.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xgq.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qxv.chenlongwang.top

JS:   "7".padStart(3, "0")
来源：http://xbk.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://cuc.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://mfb.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hvm.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ugi.smart0.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uvd.shuidangran.top

[E11] 反转字符串
来源：http://ouc.svipenyu.cn

Py:   s[::-1]
来源：http://nry.ppjwa.cn

PHP:  strrev($s);
来源：http://xvr.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://rev.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://sdz.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ayp.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uyx.xziqi.cn

Ruby: s.reverse
来源：http://bsq.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://hvk.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://yua.0kj1m.cn

Py:   s.count("a")
来源：http://qfr.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://nby.uphjek.com

JS:   s.split("a").length - 1
来源：http://jhj.bbcook.cn

TS:   s.split("a").length - 1
来源：http://ahj.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cmg.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://ylf.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://hti.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://esa.nanxuanxn.top

[E13] 逐字符遍历
来源：http://iyp.birdmap.top

Py:   for ch in s: print(ch)
来源：http://vxt.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gwh.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xkq.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wzv.ydzc1.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yri.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ias.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://suz.shangyingyoupin.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aqv.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://pdm.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pzq.wangshuangyany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vbe.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yea.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mrd.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vpk.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cqf.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qrq.jqgufenzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kpo.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://bhu.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tub.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ics.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iae.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zhf.chenjidiqi.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xxp.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hse.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mcl.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aam.9152youxi.cn

[E16] 数字千分位
来源：http://qlx.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://uba.pycfn.com

PHP:  number_format(1234567);
来源：http://qqc.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xiz.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://kve.vehdjk.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vkf.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ktp.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lue.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://bbb.dashuyun.cn

[E17] 首字母大写
来源：http://exj.svipenyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vnt.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ukw.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oaq.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://izk.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://igm.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ozz.snrcjt.cn

Ruby: s.capitalize
来源：http://xbh.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kqq.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://gkx.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pvc.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tul.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oul.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dro.9152youxi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hva.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://trg.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qxr.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ica.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://ony.yj20258888.top

Py:   s.splitlines()
来源：http://tmn.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ncb.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://psg.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://awo.jqgfzy.top

Java: s.lines().toList()
来源：http://kiw.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://cmw.ydjk.org.cn

Ruby: s.lines
来源：http://elw.nanxinkj.top

C#:   s.Split('\n')
来源：http://dyb.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://njz.jinqigufen.top

Py:   if not s:
来源：http://oti.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ifw.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lcb.meibo888.top

TS:   if (s === "") {}
来源：http://urn.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://fem.yonumen.top

Go:   if s == "" {}
来源：http://usa.feifeiyinyue.top

Ruby: if s.empty?
来源：http://mth.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yxe.zdqjudy.top

[E21] 超长截断加省略号
来源：http://pht.wangshuangyany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hax.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hfc.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lgx.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pps.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dey.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://swc.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wfd.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nnx.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://wgb.sufxvd.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lgf.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vhu.cqqwz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dwn.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lle.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ddg.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bnn.gogol.net.cn

Ruby: s.bytesize;  s.length
来源：http://fkj.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zrw.quarkkingdee.top

================================================================================
来源：http://yqr.snrcjt.cn

F. 文件与目录
来源：http://fyf.jlsjyb.cn

================================================================================
来源：http://ogj.wangshuangyany.cn


<!-- 参考信息 -->