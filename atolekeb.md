代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://via.yongpay.top

Ruby: arr.max;  arr.min
来源：http://xee.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://atm.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://oyx.quarkkingdee.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iqb.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://wpj.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gty.andypj.xyz

TS:   nested.flat();
来源：http://rsc.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pia.ydzc1.top

Go:   // 手写双层循环
来源：http://hpw.havefunace.top

Ruby: nested.flatten
来源：http://qlt.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://waf.yongpay.top

[D19] 按字段分组
来源：http://jop.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hnt.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://clc.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sng.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://oud.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eoh.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://pbs.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://emn.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ceb.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://hkv.zhengqikj.top

Py:   Counter(arr)
来源：http://aha.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://wnl.jlsjyb.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rbx.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lcz.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gqa.guowangkeji.top

Go:   // 手写 map[T]int
来源：http://mqp.havefunace.top

Ruby: arr.tally
来源：http://ekp.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zfp.daxiang520.top

[D21] 判断是否包含某元素
来源：http://coh.ywan-chungtsiang.top

Py:   x in arr
来源：http://jjv.snrcjt.cn

PHP:  in_array($x, $arr, true);
来源：http://rbx.jianghu66.top

JS:   arr.includes(x)
来源：http://guj.yvedp.cn

TS:   arr.includes(x)
来源：http://ful.quarkkingdee.top

Java: list.contains(x)
来源：http://fvr.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://byr.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://ysk.tianlin.xyz

C#:   list.Contains(x)
来源：http://jmh.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://kyy.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lme.pengpengdd.cyou

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pmb.iojbl.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://izx.shuidangran.top

TS:   [...arr];
来源：http://swo.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://yxk.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ahl.fzhhl.top

Ruby: arr.dup;  arr.clone
来源：http://pwn.jinqigfzy.top

C#:   new List<int>(list);
来源：http://clc.cashguo.top

[D23] reduce 累积计算
来源：http://hbt.jqgufenzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://otg.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eil.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hgy.mhx1999.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lxw.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tyb.zhoulong.xyz

Go:   // 手写循环
来源：http://uqk.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xec.jianghu66.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zth.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://ije.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://off.yuanzhike.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ijp.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://faj.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qsm.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qxp.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://azu.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://irx.ehwqpu.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://prr.iojbl.cn

[D25] Set 集合去重与交并差
来源：http://qpu.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fdw.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qiw.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://exx.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://szx.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gcy.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ldt.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qoi.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xrd.wangdashe.top

[D26] 数组转字符串
来源：http://bio.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://emi.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://bqs.zhongyouzk.top

JS:   arr.join(", ")
来源：http://vjz.bjfxy.top

TS:   arr.join(", ")
来源：http://hhy.cucudq.cn

Java: String.join(", ", list)
来源：http://tiw.bbcook.cn

Go:   strings.Join(strs, ", ")
来源：http://qwn.jinqigufen.top

Ruby: arr.join(", ")
来源：http://ptb.haohaochexian.top

C#:   string.Join(", ", list)
来源：http://ohb.vehdjk.com

================================================================================
来源：http://xoe.jqgfzy.top

E. 字符串处理
来源：http://hey.jianghu66.top

================================================================================
来源：http://ins.cqqwz.cn

[E01] 拼接字符串
来源：http://hth.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://slo.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mfv.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://udz.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rxk.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kzj.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lro.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xpp.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mzg.xuanzx.com

[E02] 重复字符串
来源：http://uax.jiagoushi.top

Py:   "ab" * 3
来源：http://uqn.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://tuv.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://lmv.mhx1999.top

TS:   "ab".repeat(3)
来源：http://rls.daxiang520.top

Java: "ab".repeat(3)
来源：http://wbo.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://las.haohaochexian.top

Ruby: "ab" * 3
来源：http://mki.chenjidiqi.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vxj.gaohongyu789.top

[E03] 截取子串
来源：http://uxo.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fyr.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gjp.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vvx.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://ixm.jiagoushi.top

Java: s.substring(1, 4)
来源：http://zma.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fjy.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wbw.sweek.top

C#:   s.Substring(1, 3)
来源：http://pqz.xinyue.icu

[E04] 查找子串位置
来源：http://gnz.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://fbd.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://peo.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ltv.wangdashe.top

TS:   s.indexOf("x")
来源：http://dls.yonumen.top

Java: s.indexOf("x")
来源：http://tqw.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://lwc.chenjidiqi.icu

Ruby: s.index("x")
来源：http://lbd.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://fnj.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vux.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sar.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://srx.redwolf501.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ylh.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bkl.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aov.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nap.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://faa.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kod.snrcjt.cn

[E06] 替换子串
来源：http://mmr.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ldo.yj20258888.top

PHP:  str_replace("a", "b", $s);
来源：http://pzm.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gic.iojbl.cn

TS:   s.replaceAll("a", "b")
来源：http://goj.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lum.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rby.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://brw.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://vpp.zycfv.cn

[E07] 按分隔符拆分
来源：http://gjo.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ayy.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vnt.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://lyl.yuxming.cn

TS:   s.split(",")
来源：http://uxr.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zcg.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lhv.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://aid.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ntv.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://xfl.shzxlz.cn

Py:   ",".join(items)
来源：http://smw.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://jvu.xinyue.icu

JS:   items.join(",")
来源：http://ibh.yj20258888.top

TS:   items.join(",")
来源：http://tib.shzxlz.cn

Java: String.join(",", items)
来源：http://qob.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://cat.havefunace.top

Ruby: items.join(",")
来源：http://qnm.meibo888.top

C#:   string.Join(",", items)
来源：http://hsx.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://uoe.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oxl.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ovj.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://frl.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://afq.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://twb.ydzc1.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zuo.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://yqc.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ybe.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://bxr.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gyd.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://erx.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://dem.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://ukz.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://oez.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zyl.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vjc.xingfuxueyuan.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gsg.redwolf501.top

[E11] 反转字符串
来源：http://ttv.daxiang520.top

Py:   s[::-1]
来源：http://hze.aizwys.cn

PHP:  strrev($s);
来源：http://bvb.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://ggy.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://odq.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://avm.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://wlf.jianghu66.top

Ruby: s.reverse
来源：http://zms.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://vlc.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://sxu.cashguo.top

Py:   s.count("a")
来源：http://nnc.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://uix.jinghuilouyu.cn

JS:   s.split("a").length - 1
来源：http://fbb.yueranfly.top

TS:   s.split("a").length - 1
来源：http://orr.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ikx.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://mym.shangyingyoupin.top

Ruby: s.count("a")
来源：http://hmg.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://hki.redwolf501.top

[E13] 逐字符遍历
来源：http://fvm.yongpay.top

Py:   for ch in s: print(ch)
来源：http://yzk.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tjm.yj20258888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oxp.bjfxy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://llh.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kta.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wqh.jinqigfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wcf.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://red.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://cep.yueranfly.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://scf.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uhk.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aoc.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uer.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nvt.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kjj.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jky.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://byq.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://zof.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://peg.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tnh.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fsk.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uwr.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kcl.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qww.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hao.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uyr.yanxiufei.cn

[E16] 数字千分位
来源：http://xxl.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://tee.aibaodan.cn

PHP:  number_format(1234567);
来源：http://aju.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://iir.birdmap.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zmt.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uon.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iur.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iwd.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://vnw.zycfv.cn

[E17] 首字母大写
来源：http://yai.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jod.zhiwuduotai.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pnx.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://msf.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cmy.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aig.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ory.jianghu66.top

Ruby: s.capitalize
来源：http://cwx.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://plr.daria6918.cn

[E18] 模板占位符替换
来源：http://wjq.jlsjyb.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://say.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ogm.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fzw.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ixk.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tar.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ceg.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dxa.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://utq.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://zga.shangyingyoupin.top

Py:   s.splitlines()
来源：http://ysf.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eai.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://ikf.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://mkt.c1oappe.top

Java: s.lines().toList()
来源：http://wuj.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://rxs.yuanzhike.top

Ruby: s.lines
来源：http://fwb.hnxiangtu.top

C#:   s.Split('\n')
来源：http://qkq.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://rti.zhengqikj.top

Py:   if not s:
来源：http://nwe.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ptm.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xrt.sweek.top

TS:   if (s === "") {}
来源：http://tpi.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://prk.jiagoushi.top

Go:   if s == "" {}
来源：http://yvp.mhx1999.top

Ruby: if s.empty?
来源：http://igw.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mdh.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://mqa.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pjg.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dtf.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bfh.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://usy.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tik.hnxiangtu.top

Go:   // 按 rune 判断长度后截断
来源：http://wgb.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jga.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pxd.yfazqb.com

[E22] 字节长度与字符长度
来源：http://mdg.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kzd.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xzy.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hot.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mwo.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aeg.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xhf.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://zre.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://abj.xylfe.cn

================================================================================
来源：http://oqn.daxiang520.top

F. 文件与目录
来源：http://zdg.bjfxy.top

================================================================================
来源：http://mza.gotoacloud.top

[F01] 读取整个文件
来源：http://qdc.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ikq.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://bze.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gyu.quarkkingdee.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kjk.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://jbg.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yan.cucudq.cn

Ruby: File.read("a.txt")
来源：http://egg.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://oba.shzxlz.cn

[F02] 逐行读取文件
来源：http://mnf.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ouk.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gzr.wangshuangyany.cn


<!-- 参考信息 -->