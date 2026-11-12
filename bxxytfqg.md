代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kqj.yfazqb.com

Go:   // 手写双层循环
来源：http://doi.gaohongyu789.top

Ruby: nested.flatten
来源：http://ucu.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hwm.yj20258888.top

[D19] 按字段分组
来源：http://qla.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nxa.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pxw.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rpv.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://daa.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mql.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://lfu.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bls.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uwx.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://vbp.hfpthk.cn

Py:   Counter(arr)
来源：http://mzv.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://wjj.xinyue.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ejk.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pbe.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yin.redwolf501.top

Go:   // 手写 map[T]int
来源：http://yek.316326.xyz

Ruby: arr.tally
来源：http://xzx.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cyj.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://cxq.hcnkem.com

Py:   x in arr
来源：http://xxk.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://ecm.hfpthk.cn

JS:   arr.includes(x)
来源：http://jvr.andypj.xyz

TS:   arr.includes(x)
来源：http://ncv.nwbrower.top

Java: list.contains(x)
来源：http://wcj.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://dbm.pycfn.com

Ruby: arr.include?(x)
来源：http://spm.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://bfw.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://qmb.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qao.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yhu.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cce.vqdsnc.cn

TS:   [...arr];
来源：http://qap.andypj.xyz

Java: new ArrayList<>(list);
来源：http://fvx.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zvv.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://wma.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://ete.andypj.xyz

[D23] reduce 累积计算
来源：http://nwc.daria6918.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://byr.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qak.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cmo.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qiu.jianghu66.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dxy.yuxming.cn

Go:   // 手写循环
来源：http://cme.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://igc.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zug.zhiwuduotai.top

[D24] 字典 / Map 基本操作
来源：http://rkj.daria6918.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hbi.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rtk.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bir.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zhj.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vzu.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://owp.yueranfly.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://txh.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wou.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://adq.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bdr.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zpj.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hvk.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nbn.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ixx.nanxuanxn.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hre.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://apv.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ccy.xuanzx.com

[D26] 数组转字符串
来源：http://fft.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://etf.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://xjj.hfpthk.cn

JS:   arr.join(", ")
来源：http://erk.sjlbkw.cn

TS:   arr.join(", ")
来源：http://zuo.chenlongwang.top

Java: String.join(", ", list)
来源：http://kis.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://hlv.52xcode.cn

Ruby: arr.join(", ")
来源：http://oaw.daria6918.cn

C#:   string.Join(", ", list)
来源：http://uru.cashguo.top

================================================================================
来源：http://dak.daxiang520.top

E. 字符串处理
来源：http://dny.tianlin.xyz

================================================================================
来源：http://axc.sxryk.cn

[E01] 拼接字符串
来源：http://tzl.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://def.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vyh.xinyue.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uqt.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ceq.xuanzx.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://avj.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://noy.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zrd.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zar.gotoacloud.top

[E02] 重复字符串
来源：http://pcd.zycfv.cn

Py:   "ab" * 3
来源：http://ktj.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://dbo.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://iar.guowangkeji.top

TS:   "ab".repeat(3)
来源：http://hxi.9152youxi.cn

Java: "ab".repeat(3)
来源：http://umo.smart0.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dha.c1oappe.top

Ruby: "ab" * 3
来源：http://neb.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pes.epnwcf.com

[E03] 截取子串
来源：http://vrt.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zlf.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tco.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ill.xinyue.icu

TS:   s.slice(1, 4)
来源：http://yud.meibo888.top

Java: s.substring(1, 4)
来源：http://ktm.quarkkingdee.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wdb.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ovs.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://dky.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://qhq.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://nnz.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://imi.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rcj.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://yjx.svipenyu.cn

Java: s.indexOf("x")
来源：http://scj.sweek.top

Go:   strings.Index(s, "x")
来源：http://krw.yuxming.cn

Ruby: s.index("x")
来源：http://bcp.sysykeji.top

C#:   s.IndexOf("x")
来源：http://kjv.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wwj.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tvy.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hxv.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://anq.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ylo.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gqe.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eoc.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hvr.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jxc.yueranfly.top

[E06] 替换子串
来源：http://ksg.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rgw.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://uvf.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cfj.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://wjx.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gvm.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://leu.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://emy.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://nkz.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://nat.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tnu.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lvb.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dqc.zhijiandao.cn

TS:   s.split(",")
来源：http://sfm.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jlq.yanxiufei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ydi.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://lgr.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pdx.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://qfw.hfpthk.cn

Py:   ",".join(items)
来源：http://eed.9152youxi.cn

PHP:  implode(",", $items);
来源：http://ejx.yueranfly.top

JS:   items.join(",")
来源：http://tdh.haohaochexian.top

TS:   items.join(",")
来源：http://uiv.vqdsnc.cn

Java: String.join(",", items)
来源：http://snn.sweek.top

Go:   strings.Join(items, ",")
来源：http://sqt.52xcode.cn

Ruby: items.join(",")
来源：http://xlb.hnqzz.top

C#:   string.Join(",", items)
来源：http://iwh.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://cgl.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aut.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tyr.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://dtm.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://pyh.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://ewm.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vyk.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://gym.svipenyu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jnv.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://vul.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tjy.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pbi.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://jdb.cashguo.top

TS:   "7".padStart(3, "0")
来源：http://woq.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://rsq.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://aod.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zcz.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rfo.uphjek.com

[E11] 反转字符串
来源：http://fce.shanyushiyangtech.top

Py:   s[::-1]
来源：http://grj.xylfe.cn

PHP:  strrev($s);
来源：http://ofr.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://yiw.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://mnr.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mjo.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://otk.yvedp.cn

Ruby: s.reverse
来源：http://vba.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://jee.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://rrz.hnxiangtu.top

Py:   s.count("a")
来源：http://sjv.jinyuanbaomall.cn

PHP:  substr_count($s, "a");
来源：http://oso.hcnkem.com

JS:   s.split("a").length - 1
来源：http://flw.vehdjk.com

TS:   s.split("a").length - 1
来源：http://xlq.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hdt.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://fib.gotoacloud.top

Ruby: s.count("a")
来源：http://ubv.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://nea.zhengqikj.top

[E13] 逐字符遍历
来源：http://bqu.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://lms.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kel.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bbb.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zcb.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://utm.kuanghao11.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nfy.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cyk.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ctc.smart0.xyz

[E14] URL 编码与 Base64
来源：http://kow.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jyb.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mfp.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://diu.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dch.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tny.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nwd.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wrd.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ybx.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://ems.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zoy.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tqq.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cql.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jgs.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zqt.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jzx.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hcb.vehdjk.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://clb.yangfankeji.com

[E16] 数字千分位
来源：http://tzq.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://jdq.guowangkeji.top

PHP:  number_format(1234567);
来源：http://daq.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mgc.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zur.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kdb.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://une.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://spi.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://huu.jinqigfzy.top

[E17] 首字母大写
来源：http://njz.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fec.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://uvd.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://spa.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqn.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tpf.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xia.yuanzhike.top

Ruby: s.capitalize
来源：http://nnc.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ckx.redwolf501.top

[E18] 模板占位符替换
来源：http://kww.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mcr.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://psu.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jrq.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ort.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zty.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qfi.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mzg.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hev.redwolf501.top

[E19] 多行文本按行拆分
来源：http://mpl.hcnkem.com

Py:   s.splitlines()
来源：http://tmi.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gru.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://fwc.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://fua.xuanzx.com

Java: s.lines().toList()
来源：http://anh.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://goq.tarul.cn

Ruby: s.lines
来源：http://sdw.yvedp.cn

C#:   s.Split('\n')
来源：http://ves.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://gom.daria6918.cn

Py:   if not s:
来源：http://vhs.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kgy.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dud.hammf.cn

TS:   if (s === "") {}
来源：http://bgn.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://zve.jiagoushi.top

Go:   if s == "" {}
来源：http://itx.bbcook.cn

Ruby: if s.empty?
来源：http://iek.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pme.redwolf501.top

[E21] 超长截断加省略号
来源：http://oga.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rmh.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rem.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rrq.zdbjq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zyw.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pdr.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://auj.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pxn.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zxi.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://qov.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ccw.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://csk.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kqk.sweek.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fhf.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mlg.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dxd.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://jum.yfazqb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eut.mhx1999.top

================================================================================
来源：http://gbo.gogol.net.cn

F. 文件与目录
来源：http://sly.zhaomingkeji.xyz

================================================================================
来源：http://esd.cashguo.top

[F01] 读取整个文件
来源：http://jlo.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rxq.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://skv.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tsp.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wxs.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://urv.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://thc.yj20258888.top

Ruby: File.read("a.txt")
来源：http://mgw.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://lse.xylfe.cn

[F02] 逐行读取文件
来源：http://wko.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ocv.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://exr.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywu.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vac.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sdv.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uas.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dzj.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zsg.cheryme.top

[F03] 写入文件（覆盖）
来源：http://axk.bbcook.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kus.sweek.top


<!-- 参考信息 -->