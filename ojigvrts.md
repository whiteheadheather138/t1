代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yhl.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://qku.yj20258.top

Py:   Counter(arr)
来源：http://wsi.tianlin.xyz

PHP:  array_count_values($arr);
来源：http://flr.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://alr.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lue.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://igc.ybcxt.top

Go:   // 手写 map[T]int
来源：http://oun.zdqjudy.top

Ruby: arr.tally
来源：http://rpz.sufxvd.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vii.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://ojs.dashuyun.cn

Py:   x in arr
来源：http://zsp.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://jvp.yvedp.cn

JS:   arr.includes(x)
来源：http://enu.gaohongyu789.top

TS:   arr.includes(x)
来源：http://cha.hesvh.cn

Java: list.contains(x)
来源：http://dyg.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://pgw.yj202588.top

Ruby: arr.include?(x)
来源：http://col.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://fir.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://uem.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://poh.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wha.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rso.havefunace.top

TS:   [...arr];
来源：http://vvs.hnqzz.top

Java: new ArrayList<>(list);
来源：http://smy.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sqa.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://mum.guannengcc.top

C#:   new List<int>(list);
来源：http://snk.jyoumei.cn

[D23] reduce 累积计算
来源：http://rzh.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uxt.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hqv.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pho.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pts.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gjg.yvedp.cn

Go:   // 手写循环
来源：http://ayn.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mqc.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iem.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://nxb.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sfo.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ctj.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qce.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hmi.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iqm.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://phj.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cnq.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oma.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://owx.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://swk.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://glp.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hmw.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rkz.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xgm.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ijw.haohaochexian.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://osj.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wtd.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://oog.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://oex.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://jgv.fzhhl.top

JS:   arr.join(", ")
来源：http://cod.aibaodan.cn

TS:   arr.join(", ")
来源：http://atv.yongpay.top

Java: String.join(", ", list)
来源：http://lzc.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://ept.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://jgd.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://ler.sysykeji.top

================================================================================
来源：http://iww.shangyingyoupin.top

E. 字符串处理
来源：http://imz.gzhubu.top

================================================================================
来源：http://vpt.hnqzz.top

[E01] 拼接字符串
来源：http://kcg.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sbe.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vxt.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ydj.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ses.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iho.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ips.epnwcf.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fwk.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jfa.guannengcc.top

[E02] 重复字符串
来源：http://hbz.0kj1m.cn

Py:   "ab" * 3
来源：http://rfe.jinghuilouyu.cn

PHP:  str_repeat("ab", 3);
来源：http://kxo.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://lnv.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://sep.hesvh.cn

Java: "ab".repeat(3)
来源：http://zru.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://nlg.yangfankeji.com

Ruby: "ab" * 3
来源：http://gzl.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ygr.ydzc1.top

[E03] 截取子串
来源：http://vys.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://shr.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uxt.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://haa.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://ctf.yj20258.top

Java: s.substring(1, 4)
来源：http://dza.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ynq.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://eux.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://syb.pycfn.com

[E04] 查找子串位置
来源：http://tgy.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://nhc.cashguo.top

PHP:  strpos($s, "x");
来源：http://cko.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://icw.sxryk.cn

TS:   s.indexOf("x")
来源：http://niy.pycfn.com

Java: s.indexOf("x")
来源：http://pcw.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://ybl.vehdjk.com

Ruby: s.index("x")
来源：http://jjp.gzhubu.top

C#:   s.IndexOf("x")
来源：http://yro.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bdb.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nqo.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fqa.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://thl.yangfankeji.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://obg.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bgj.zhoulong.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mya.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rmk.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ppc.yj20258888.top

[E06] 替换子串
来源：http://lmm.guannengcc.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hya.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://qij.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://khc.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://qcl.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gth.bbcook.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ozx.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hba.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://hyi.yj202588.top

[E07] 按分隔符拆分
来源：http://hdg.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bls.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rdb.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tjo.fehbvm.com

TS:   s.split(",")
来源：http://eah.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://aff.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zoo.sweek.top

Ruby: s.split(",");  s.split
来源：http://kmr.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.yvedp.cn

[E08] 数组按分隔符合并
来源：http://mwk.redwolf501.top

Py:   ",".join(items)
来源：http://ajy.nwbrower.top

PHP:  implode(",", $items);
来源：http://hxf.daria6918.cn

JS:   items.join(",")
来源：http://yhh.yangfankeji.com

TS:   items.join(",")
来源：http://nmf.aizwys.cn

Java: String.join(",", items)
来源：http://okh.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://iid.ppjwa.cn

Ruby: items.join(",")
来源：http://wil.fengsongda.top

C#:   string.Join(",", items)
来源：http://gnj.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://ypu.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fkt.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oml.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://rwh.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://rzi.ybcxt.top

Java: s.replaceAll("\\s+", "")
来源：http://kjn.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://zgp.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://xeu.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jcu.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://yjc.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ixq.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ggq.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://mrt.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://vnt.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://irq.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://htw.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oot.bjfxy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ugb.cheryme.top

[E11] 反转字符串
来源：http://ela.yonumen.top

Py:   s[::-1]
来源：http://tqa.zhoulong.xyz

PHP:  strrev($s);
来源：http://hvq.ehwqpu.com

JS:   [...s].reverse().join("")
来源：http://gxz.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://nyg.uphjek.com

Java: new StringBuilder(s).reverse().toString()
来源：http://dhl.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ywd.fanxiaobao.xyz

Ruby: s.reverse
来源：http://wch.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cnh.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://bwy.nanxuanxn.top

Py:   s.count("a")
来源：http://imi.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://esk.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://nby.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://qxo.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vhn.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://xez.shzxlz.cn

Ruby: s.count("a")
来源：http://bjh.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://lkh.vehdjk.com

[E13] 逐字符遍历
来源：http://zfe.yonumen.top

Py:   for ch in s: print(ch)
来源：http://vxl.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qsl.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pwh.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wic.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xwk.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lqg.nwbrower.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xbz.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mgv.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://ayb.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ouc.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://thu.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vmr.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zdt.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ktb.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xqg.chenzaomai.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yeg.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qoe.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://agu.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sxy.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ojw.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xey.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jdt.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bue.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mgc.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ngf.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://avb.shuidangran.top

[E16] 数字千分位
来源：http://rqb.ybcxt.top

Py:   f"{1234567:,}"
来源：http://loe.zhengqikj.top

PHP:  number_format(1234567);
来源：http://sxs.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sdm.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ynx.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dje.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bgn.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://owc.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://icu.nanxinkj.top

[E17] 首字母大写
来源：http://yqn.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iur.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://niy.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yih.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uww.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gtr.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mul.yongpay.top

Ruby: s.capitalize
来源：http://tas.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ddj.yj20258.top

[E18] 模板占位符替换
来源：http://eno.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://czo.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rzf.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qpr.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qxb.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://whl.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uyg.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://igd.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hds.sxryk.cn

[E19] 多行文本按行拆分
来源：http://xyn.cucudq.cn

Py:   s.splitlines()
来源：http://uor.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fcp.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://ypq.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://cej.jiagoushi.top

Java: s.lines().toList()
来源：http://cwj.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://bxd.epnwcf.com

Ruby: s.lines
来源：http://oag.guowangkeji.top

C#:   s.Split('\n')
来源：http://yll.fzhhl.top

[E20] 判断字符串是否为空
来源：http://hxd.vehdjk.com

Py:   if not s:
来源：http://qlh.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gev.feifeiyinyue.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mrj.jqgufenzy.top

TS:   if (s === "") {}
来源：http://shf.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://mlg.daria6918.cn

Go:   if s == "" {}
来源：http://dnf.yonumen.top

Ruby: if s.empty?
来源：http://sdi.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iev.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://sbv.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bqd.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gzv.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zek.bjfxy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kdc.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://emi.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://exd.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gwj.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tcg.iojbl.cn

[E22] 字节长度与字符长度
来源：http://hsb.tanke756.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://szn.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qfi.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hzx.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fac.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://beg.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pmz.52xcode.cn

Ruby: s.bytesize;  s.length
来源：http://wcd.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://srw.xinyue.icu

================================================================================
来源：http://ylh.sweek.top

F. 文件与目录
来源：http://zje.hesvh.cn

================================================================================
来源：http://suk.svipenyu.cn

[F01] 读取整个文件
来源：http://bqw.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lqp.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://hfm.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ttv.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hxe.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://pcp.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wuv.c1oappe.top

Ruby: File.read("a.txt")
来源：http://zcg.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://jrh.jianghu66.top

[F02] 逐行读取文件
来源：http://cwc.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fci.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bwy.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://otv.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gri.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ldl.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gpp.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://esy.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zxs.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://qfm.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dbh.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lps.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jej.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://php.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cpi.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ggt.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://imr.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bce.wangshuangyany.cn

[F04] 追加写入文件
来源：http://wqc.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pyn.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rxe.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xtg.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bji.nanxuanxn.top


<!-- 参考信息 -->