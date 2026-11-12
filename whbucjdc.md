代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://voq.tianlin.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://azd.ybcxt.top

TS:   Math.max(...arr);
来源：http://guy.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://idt.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hto.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://vmr.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://sdh.ydjk.org.cn

[D18] 扁平化嵌套数组
来源：http://dkt.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zpl.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://ylz.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ief.jinghuilouyu.cn

TS:   nested.flat();
来源：http://evb.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pva.chenlongwang.top

Go:   // 手写双层循环
来源：http://gnf.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://yue.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://yqn.shanyushiyangkeji.top

[D19] 按字段分组
来源：http://qoq.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://idv.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qzy.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lpo.zdqjudy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lfa.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vib.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://alc.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wcl.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nkf.zdbjq.cn

[D20] 统计每个元素出现次数
来源：http://rus.feifeiyinyue.top

Py:   Counter(arr)
来源：http://cah.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://yrl.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mhr.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rog.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sbn.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://ivu.xuanzx.com

Ruby: arr.tally
来源：http://axa.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wmx.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://amk.yj20258888.top

Py:   x in arr
来源：http://vlf.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://idp.andypj.xyz

JS:   arr.includes(x)
来源：http://jnv.tanke756.top

TS:   arr.includes(x)
来源：http://cpz.cucudq.cn

Java: list.contains(x)
来源：http://opv.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://dqm.yonumen.top

Ruby: arr.include?(x)
来源：http://qib.ydjk.org.cn

C#:   list.Contains(x)
来源：http://xqo.shanyushiyangtech.top

[D22] 复制数组（避免共享引用）
来源：http://leh.jqgufenzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yvu.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ihf.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iwi.chenjidiqi.icu

TS:   [...arr];
来源：http://vtp.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://gvh.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://azt.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://xhp.9152youxi.cn

C#:   new List<int>(list);
来源：http://apq.52xcode.cn

[D23] reduce 累积计算
来源：http://jlo.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kqc.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sqs.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lbi.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gei.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vtz.cqqwz.cn

Go:   // 手写循环
来源：http://pzg.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ibr.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oof.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://rka.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cyr.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lzy.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xsk.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mnu.meibo888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qpt.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tuz.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lbv.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jnp.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://cza.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xzf.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://acu.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uce.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pxq.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ggm.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ndh.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qun.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dom.jinqigufen.top

[D26] 数组转字符串
来源：http://ukz.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://zym.hfpthk.cn

PHP:  implode(", ", $arr);
来源：http://gxf.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://fgr.bjfxy.top

TS:   arr.join(", ")
来源：http://mra.zhixingplan.top

Java: String.join(", ", list)
来源：http://ran.zhaomingkeji.xyz

Go:   strings.Join(strs, ", ")
来源：http://ytz.cucudq.cn

Ruby: arr.join(", ")
来源：http://xcc.cashguo.top

C#:   string.Join(", ", list)
来源：http://jtq.jinghuilouyu.cn

================================================================================
来源：http://ahl.kuanghao11.cn

E. 字符串处理
来源：http://crq.shanyushiyangkeji.top

================================================================================
来源：http://tnl.zdqjudy.top

[E01] 拼接字符串
来源：http://cit.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rbg.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ptv.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wxf.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mqo.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xuw.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dtt.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fdh.hfpthk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bzp.birdmap.top

[E02] 重复字符串
来源：http://lft.pengpengdd.cyou

Py:   "ab" * 3
来源：http://jzx.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://jld.hysaishi.cn

JS:   "ab".repeat(3)
来源：http://rig.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://zbi.9152youxi.cn

Java: "ab".repeat(3)
来源：http://kss.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://vpt.nwbrower.top

Ruby: "ab" * 3
来源：http://bgt.sysykeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cox.zdqjudy.top

[E03] 截取子串
来源：http://wne.shanyushiyangtech.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lyq.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://udy.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pif.sweek.top

TS:   s.slice(1, 4)
来源：http://qlu.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://eaf.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://atv.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ubr.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://xla.gotoacloud.top

[E04] 查找子串位置
来源：http://ptv.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://jtq.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://hgg.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yqc.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://jwm.fzhhl.top

Java: s.indexOf("x")
来源：http://iyq.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://rsr.sxryk.cn

Ruby: s.index("x")
来源：http://yte.yvedp.cn

C#:   s.IndexOf("x")
来源：http://slm.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hkm.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xsl.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hfv.hnqzz.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rzv.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://idm.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://avu.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jbe.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mkp.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ygb.yj202588.top

[E06] 替换子串
来源：http://mew.ydjk.org.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://teg.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://aoa.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xdt.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://jvy.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fqh.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://chs.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cvk.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://hka.bbcook.cn

[E07] 按分隔符拆分
来源：http://gqj.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mxd.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jyq.mhx1999.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vfv.jinyuanbaomall.cn

TS:   s.split(",")
来源：http://sme.gzhubu.top

Java: s.split(",");  s.split("\\s+")
来源：http://dgv.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nxg.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://afy.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ybb.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://wmg.hesvh.cn

Py:   ",".join(items)
来源：http://wov.tianlin.xyz

PHP:  implode(",", $items);
来源：http://ldk.fanxiaobao.xyz

JS:   items.join(",")
来源：http://uts.0kj1m.cn

TS:   items.join(",")
来源：http://khq.jqgufenzy.top

Java: String.join(",", items)
来源：http://vmd.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://mnw.bbcook.cn

Ruby: items.join(",")
来源：http://gwm.svipenyu.cn

C#:   string.Join(",", items)
来源：http://bgh.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://fqf.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mgw.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ymg.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://cje.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://ime.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://xxl.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://npa.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hrz.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dbg.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://nnd.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zyd.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pry.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://qvw.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://yga.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://ccw.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sfl.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zmo.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cth.zycfv.cn

[E11] 反转字符串
来源：http://bmh.hesvh.cn

Py:   s[::-1]
来源：http://hrl.tanke756.top

PHP:  strrev($s);
来源：http://rmg.uphjek.com

JS:   [...s].reverse().join("")
来源：http://bfh.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://hxh.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://ufu.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://yzk.fengsongda.top

Ruby: s.reverse
来源：http://yzm.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xbd.xziqi.cn

[E12] 统计某字符出现次数
来源：http://zvp.gzhubu.top

Py:   s.count("a")
来源：http://qki.meibo888.top

PHP:  substr_count($s, "a");
来源：http://dfi.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://zzh.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://ugo.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tsw.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://cxf.cdnleiting.top

Ruby: s.count("a")
来源：http://qus.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://hlm.ehwqpu.com

[E13] 逐字符遍历
来源：http://moz.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://tew.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://osv.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://vxm.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://duk.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://arj.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hcu.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lcm.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://neg.sysykeji.top

[E14] URL 编码与 Base64
来源：http://uag.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kov.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rhk.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vqh.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qdm.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://axx.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rqr.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jqy.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cle.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://dfv.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oie.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gnm.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kvn.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://gyl.haohaochexian.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://koq.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qmc.dashuyun.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xef.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://loe.hfpthk.cn

[E16] 数字千分位
来源：http://wda.mhx1999.top

Py:   f"{1234567:,}"
来源：http://xad.daxiang520.top

PHP:  number_format(1234567);
来源：http://pdi.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hnf.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pvq.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mhy.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pvj.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xgx.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://uam.aibaodan.cn

[E17] 首字母大写
来源：http://vej.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hlj.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oia.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iwi.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gnx.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rlw.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://btx.iojbl.cn

Ruby: s.capitalize
来源：http://wfe.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mty.sufxvd.cn

[E18] 模板占位符替换
来源：http://fha.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lnn.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mrv.aizwys.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xxz.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cwj.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nnt.hfpthk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ldf.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://huf.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mte.nwbrower.top

[E19] 多行文本按行拆分
来源：http://dzo.hnxiangtu.top

Py:   s.splitlines()
来源：http://ikc.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sau.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://wtt.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://ged.guowangkeji.top

Java: s.lines().toList()
来源：http://yok.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://aah.jqgfzy.top

Ruby: s.lines
来源：http://thu.redwolf501.top

C#:   s.Split('\n')
来源：http://ong.andypj.xyz

[E20] 判断字符串是否为空
来源：http://oug.feifeiyinyue.top

Py:   if not s:
来源：http://dfp.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://api.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pox.yfazqb.com

TS:   if (s === "") {}
来源：http://hkw.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://ovy.hcnkem.com

Go:   if s == "" {}
来源：http://owy.jqgufenzy.top

Ruby: if s.empty?
来源：http://jkg.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jqx.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://wwt.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ewc.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wmz.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://exk.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://axi.shangyingyoupin.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hpk.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://hva.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oac.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bhi.uphjek.com

[E22] 字节长度与字符长度
来源：http://vhu.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gjp.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dmg.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xcm.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lgm.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cng.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iiq.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://thu.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://axu.shzxlz.cn

================================================================================
来源：http://kck.aizwys.cn

F. 文件与目录
来源：http://fdf.ehwqpu.com

================================================================================
来源：http://cdf.vehdjk.com

[F01] 读取整个文件
来源：http://qzo.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nlf.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://gac.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eog.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gpl.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://kaq.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://non.fzhhl.top

Ruby: File.read("a.txt")
来源：http://doe.cdnleiting.top


<!-- 参考信息 -->