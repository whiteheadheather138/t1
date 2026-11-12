代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://edt.guowangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jzu.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pyo.gaohongyu789.top

Go:   // 手写循环累加
来源：http://ivx.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jfl.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://gsh.ctjpmb.com

[D17] 最大值与最小值
来源：http://wxu.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://mkt.yvedp.cn

PHP:  max($arr);  min($arr);
来源：http://tzb.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://smw.smart0.xyz

TS:   Math.max(...arr);
来源：http://vax.ydjk.org.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ozk.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uct.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://tqw.hammf.cn

C#:   list.Max();  list.Min()
来源：http://yul.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://krp.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://som.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://nuy.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bnq.jianghu66.top

TS:   nested.flat();
来源：http://cxf.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ouh.sxryk.cn

Go:   // 手写双层循环
来源：http://vot.havefunace.top

Ruby: nested.flatten
来源：http://pjc.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yay.hongshengwenyu.top

[D19] 按字段分组
来源：http://guc.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vhi.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fwn.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qxs.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vkv.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ubq.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://qap.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ltl.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://brk.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://rlc.fzhhl.top

Py:   Counter(arr)
来源：http://nkj.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://awb.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hbp.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hzy.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hbi.daxiang520.top

Go:   // 手写 map[T]int
来源：http://tbu.xuetiantiany.cn

Ruby: arr.tally
来源：http://bik.jqgfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vzz.guannengcc.top

[D21] 判断是否包含某元素
来源：http://zvz.cdnleiting.top

Py:   x in arr
来源：http://peg.wangdashe.top

PHP:  in_array($x, $arr, true);
来源：http://pwk.chenzaomai.com

JS:   arr.includes(x)
来源：http://itr.pycfn.com

TS:   arr.includes(x)
来源：http://gct.sweek.top

Java: list.contains(x)
来源：http://ckv.aibaodan.cn

Go:   slices.Contains(arr, x)
来源：http://qei.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://ftr.snrcjt.cn

C#:   list.Contains(x)
来源：http://jle.gogol.net.cn

[D22] 复制数组（避免共享引用）
来源：http://jtl.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vpf.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yws.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bma.hysaishi.cn

TS:   [...arr];
来源：http://bgk.epnwcf.com

Java: new ArrayList<>(list);
来源：http://fjm.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://xeb.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://odx.52xcode.cn

C#:   new List<int>(list);
来源：http://nkw.fehbvm.com

[D23] reduce 累积计算
来源：http://fhq.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sgo.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://auo.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gmq.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dyp.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://oww.ydjk.org.cn

Go:   // 手写循环
来源：http://vxh.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ptu.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://say.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://hxr.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wmi.yuanzhike.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jbq.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://khl.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wdr.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pkz.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vno.xinyue.icu

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ney.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dna.yvedp.cn

[D25] Set 集合去重与交并差
来源：http://jqy.zhongyouzk.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nlt.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://skm.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fta.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bzt.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qtf.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hzw.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://izj.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qry.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://otj.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://ubc.tarul.cn

PHP:  implode(", ", $arr);
来源：http://nau.yanxiufei.cn

JS:   arr.join(", ")
来源：http://oqk.shangyingyoupin.top

TS:   arr.join(", ")
来源：http://igp.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://cxy.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://kdq.bbcook.cn

Ruby: arr.join(", ")
来源：http://kpo.c1oappe.top

C#:   string.Join(", ", list)
来源：http://eif.yfazqb.com

================================================================================
来源：http://osz.xinyue.icu

E. 字符串处理
来源：http://rse.jianghu66.top

================================================================================
来源：http://lpw.pengpengdd.cyou

[E01] 拼接字符串
来源：http://zxl.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cnb.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://npp.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ogj.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hxg.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jbw.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ncc.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rtp.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://aql.zhoulong.xyz

[E02] 重复字符串
来源：http://gyu.daxiang520.top

Py:   "ab" * 3
来源：http://nod.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://tza.yfazqb.com

JS:   "ab".repeat(3)
来源：http://meo.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://ftd.cashguo.top

Java: "ab".repeat(3)
来源：http://amp.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://lqt.9152youxi.cn

Ruby: "ab" * 3
来源：http://yfn.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ptx.zhiwuduotai.top

[E03] 截取子串
来源：http://ssz.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ymh.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://igy.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mam.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://ydv.hcnkem.com

Java: s.substring(1, 4)
来源：http://fts.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ydt.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://oyv.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://nih.xuetiantiany.cn

[E04] 查找子串位置
来源：http://zeu.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://eyf.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://ftm.guannengcc.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rqd.fktsv.cn

TS:   s.indexOf("x")
来源：http://nun.yj20258.top

Java: s.indexOf("x")
来源：http://ogs.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://vls.c1oappe.top

Ruby: s.index("x")
来源：http://vko.ybcxt.top

C#:   s.IndexOf("x")
来源：http://poa.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cff.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jkq.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kel.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://skc.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gxa.ydjk.org.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://utq.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://efc.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xtq.sjlbkw.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kbl.jinyuanbaomall.cn

[E06] 替换子串
来源：http://end.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xdb.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://xbq.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gtq.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://syk.fehbvm.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xqq.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fzi.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ibn.zdqjudy.top

C#:   s.Replace("a", "b")
来源：http://img.yonumen.top

[E07] 按分隔符拆分
来源：http://xkw.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zvn.ivvv.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://njh.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ctv.chenlongwang.top

TS:   s.split(",")
来源：http://qut.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://ppo.daria6918.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://diw.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://cmj.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fyk.cashguo.top

[E08] 数组按分隔符合并
来源：http://yxf.yj20258888.top

Py:   ",".join(items)
来源：http://ujn.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://ste.ivvv.top

JS:   items.join(",")
来源：http://rlu.hfpthk.cn

TS:   items.join(",")
来源：http://hkp.fehbvm.com

Java: String.join(",", items)
来源：http://fxr.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://epd.chenzaomai.com

Ruby: items.join(",")
来源：http://ops.fengsongda.top

C#:   string.Join(",", items)
来源：http://lri.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://jzq.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cvp.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aey.52xcode.cn

JS:   s.replace(/\s+/g, "")
来源：http://aby.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://tkf.zhiwuduotai.top

Java: s.replaceAll("\\s+", "")
来源：http://gzz.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://npu.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://cjh.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qjc.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://qil.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mys.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zdb.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://uro.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://bhl.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://btl.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://rkx.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mue.guannengcc.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ohz.nwbrower.top

[E11] 反转字符串
来源：http://enn.chenjidiqi.icu

Py:   s[::-1]
来源：http://jlc.cqqwz.cn

PHP:  strrev($s);
来源：http://wwi.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://pee.hammf.cn

TS:   [...s].reverse().join("")
来源：http://obe.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vtq.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://owe.hammf.cn

Ruby: s.reverse
来源：http://rpa.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://riz.cashguo.top

[E12] 统计某字符出现次数
来源：http://ytc.snrcjt.cn

Py:   s.count("a")
来源：http://wdd.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://uub.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://beb.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://yap.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ecy.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://ioi.redwolf501.top

Ruby: s.count("a")
来源：http://dsn.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://llq.vehdjk.com

[E13] 逐字符遍历
来源：http://xzi.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://xlx.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hbm.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nwv.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://qnx.yj202588.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lab.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://izq.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ric.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vtt.xylfe.cn

[E14] URL 编码与 Base64
来源：http://oie.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vyg.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ohr.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rxg.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mia.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dcr.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fur.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://smc.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fbv.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://htd.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://klo.hesvh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ydg.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zzq.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://hts.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vut.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://umb.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jhr.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ilr.wangshuangyany.cn

[E16] 数字千分位
来源：http://ccd.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://wmc.xinyue.icu

PHP:  number_format(1234567);
来源：http://bjd.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rax.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wcl.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dtj.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://agt.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yer.zhengqikj.top

C#:   1234567.ToString("N0")
来源：http://qfj.feifeiyinyue.top

[E17] 首字母大写
来源：http://fki.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uhc.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jzm.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dkj.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xfm.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lta.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pii.chenlongwang.top

Ruby: s.capitalize
来源：http://oyk.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ium.hfpthk.cn

[E18] 模板占位符替换
来源：http://stp.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uho.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qgs.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nul.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yzq.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://but.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pye.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://szj.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ujb.shuidangran.top

[E19] 多行文本按行拆分
来源：http://nvn.shzxlz.cn

Py:   s.splitlines()
来源：http://beu.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cbf.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://myt.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://ypi.nanxinkj.top

Java: s.lines().toList()
来源：http://ytl.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://vsa.jqgfzy.top

Ruby: s.lines
来源：http://wju.sufxvd.cn

C#:   s.Split('\n')
来源：http://quu.yuxming.cn

[E20] 判断字符串是否为空
来源：http://fzx.jlsjyb.cn

Py:   if not s:
来源：http://pgt.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://smz.zhongyouzk.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tjh.cdnleiting.top

TS:   if (s === "") {}
来源：http://tgd.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://oby.tarul.cn

Go:   if s == "" {}
来源：http://ehj.nanxuanxn.top

Ruby: if s.empty?
来源：http://mdi.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bwq.yvedp.cn

[E21] 超长截断加省略号
来源：http://pol.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gvs.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xzq.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nvw.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ent.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ysj.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://phs.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hcv.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://erp.hnxiangtu.top

[E22] 字节长度与字符长度
来源：http://pug.gogol.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aim.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kcr.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qto.jiagoushi.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kia.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://imm.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xgm.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://dhl.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vva.quarkkingdee.top

================================================================================
来源：http://one.xinyue.icu

F. 文件与目录
来源：http://swj.shanyushiyangtech.top

================================================================================
来源：http://dku.iojbl.cn


<!-- 参考信息 -->