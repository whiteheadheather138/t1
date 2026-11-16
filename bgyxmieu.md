代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wkh.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vwn.xuetiantiany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hpu.zhiwuduotai.top

TS:   [...arr];
来源：http://tfw.redwolf501.top

Java: new ArrayList<>(list);
来源：http://pzx.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qfc.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://jfd.jinqigufen.top

C#:   new List<int>(list);
来源：http://opt.cqqwz.cn

[D23] reduce 累积计算
来源：http://rfp.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://seq.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cmw.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kao.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kig.9152youxi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://olp.meibo888.top

Go:   // 手写循环
来源：http://eid.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wkr.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tjq.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://wcq.shanyushiyangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ydb.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rxy.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ter.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hqt.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lnq.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ywz.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://twt.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://giw.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://wcj.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fjy.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rfk.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://znv.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xcv.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bsg.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ybk.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iaj.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wqv.guowangkeji.top

[D26] 数组转字符串
来源：http://rib.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://gro.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://rqc.zdbjq.cn

JS:   arr.join(", ")
来源：http://aho.tian-w.cn

TS:   arr.join(", ")
来源：http://sne.zhengqikj.top

Java: String.join(", ", list)
来源：http://jxp.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://loh.fanxiaobao.xyz

Ruby: arr.join(", ")
来源：http://voq.cheryme.top

C#:   string.Join(", ", list)
来源：http://vrv.cashguo.top

================================================================================
来源：http://mhy.jinyuanbaomall.cn

E. 字符串处理
来源：http://viu.xinyue.icu

================================================================================
来源：http://xll.jlsjyb.cn

[E01] 拼接字符串
来源：http://hzo.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gts.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cgv.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://onl.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kkr.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ocb.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vjg.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yrb.aibaodan.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kmt.yangfankeji.com

[E02] 重复字符串
来源：http://itt.zdqjudy.top

Py:   "ab" * 3
来源：http://zqm.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://dle.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://fkr.yvedp.cn

TS:   "ab".repeat(3)
来源：http://xho.ydzc1.top

Java: "ab".repeat(3)
来源：http://eqa.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://tgr.dianchejie.cn

Ruby: "ab" * 3
来源：http://zvo.jqgufenzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hid.pycfn.com

[E03] 截取子串
来源：http://ehi.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zry.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://csg.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yqz.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://yot.52xcode.cn

Java: s.substring(1, 4)
来源：http://tbv.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ftm.xinyue.icu

Ruby: s[1, 3];  s[1..3]
来源：http://ttb.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://kxu.wangshuangyany.cn

[E04] 查找子串位置
来源：http://zzj.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://des.c1oappe.top

PHP:  strpos($s, "x");
来源：http://bff.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nye.xuanzx.com

TS:   s.indexOf("x")
来源：http://uui.fehbvm.com

Java: s.indexOf("x")
来源：http://rqv.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://ifc.ydzc1.top

Ruby: s.index("x")
来源：http://pie.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://cif.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ied.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eok.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uqm.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mbh.xingfuxueyuan.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://ekh.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nea.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ssm.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tpk.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hax.cqqwz.cn

[E06] 替换子串
来源：http://rfu.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://csl.yfazqb.com

PHP:  str_replace("a", "b", $s);
来源：http://apn.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iik.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://tmp.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lfn.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zms.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dhk.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://lmf.fehbvm.com

[E07] 按分隔符拆分
来源：http://rua.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://etf.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lfh.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ngz.yonumen.top

TS:   s.split(",")
来源：http://oli.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://aan.yj20258.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yvv.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://zlr.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kqx.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://kyl.feifeiyinyue.top

Py:   ",".join(items)
来源：http://uge.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://eqo.hesvh.cn

JS:   items.join(",")
来源：http://mmo.dashuyun.cn

TS:   items.join(",")
来源：http://wtj.ctjpmb.com

Java: String.join(",", items)
来源：http://uqu.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://nau.dianchejie.cn

Ruby: items.join(",")
来源：http://ghu.gogol.net.cn

C#:   string.Join(",", items)
来源：http://nug.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://fpk.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://plo.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nfa.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://sry.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://afu.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://kfs.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://eqj.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://aae.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jue.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://dhy.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ihm.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nxj.xuanzx.com

JS:   "7".padStart(3, "0")
来源：http://mip.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://auy.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://kjs.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zqp.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xuw.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gyb.dashuyun.cn

[E11] 反转字符串
来源：http://yhn.yueranfly.top

Py:   s[::-1]
来源：http://eet.hysaishi.cn

PHP:  strrev($s);
来源：http://ybh.xuanzx.com

JS:   [...s].reverse().join("")
来源：http://pes.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://bou.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://omp.sjlbkw.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jrq.daxiang520.top

Ruby: s.reverse
来源：http://ftq.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tfx.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://kek.jyoumei.cn

Py:   s.count("a")
来源：http://xkk.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://avf.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://mnq.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://gxz.bbcook.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dbt.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://hoo.tanke756.top

Ruby: s.count("a")
来源：http://znt.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://oqh.xinyue.icu

[E13] 逐字符遍历
来源：http://ing.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://bcv.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ulq.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xev.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yfb.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qym.chenzaomai.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kok.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cmp.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zax.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://yls.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vrh.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://lrx.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://epv.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ges.uphjek.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xpc.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fbc.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ses.yueranfly.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qjs.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://xhl.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ada.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yrj.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ata.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sbi.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kiq.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sxp.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jxh.redwolf501.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://prw.jianghu66.top

[E16] 数字千分位
来源：http://ndv.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://uxn.tian-w.cn

PHP:  number_format(1234567);
来源：http://vjg.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qec.aibaodan.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ffy.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qkd.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://syt.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nit.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://blj.jianghu66.top

[E17] 首字母大写
来源：http://dgp.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://chv.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mvp.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hkw.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mho.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ogp.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hsb.hysaishi.cn

Ruby: s.capitalize
来源：http://jxg.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qai.yj202588.top

[E18] 模板占位符替换
来源：http://bbm.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://afw.zycfv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fre.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ffi.feifeiyinyue.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hxb.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cfh.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tad.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kwl.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nvs.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://ngw.haohaochexian.top

Py:   s.splitlines()
来源：http://djb.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wld.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://leb.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://wwn.havefunace.top

Java: s.lines().toList()
来源：http://hwn.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://pmr.gaohongyu789.top

Ruby: s.lines
来源：http://bhk.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://bdo.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://dlq.xinyue.icu

Py:   if not s:
来源：http://hcd.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zcf.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pil.yuxming.cn

TS:   if (s === "") {}
来源：http://ute.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://rgg.hnxiangtu.top

Go:   if s == "" {}
来源：http://ggh.xuetiantiany.cn

Ruby: if s.empty?
来源：http://eql.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jhg.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://hhl.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qis.hcnkem.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vyn.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gmy.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lcw.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wgb.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://zwz.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zjy.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://smw.yj20258888.top

[E22] 字节长度与字符长度
来源：http://yvj.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://psk.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qzs.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kje.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ioi.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fkk.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gpn.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://qda.jyoumei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://klk.yuanzhike.top

================================================================================
来源：http://zkk.yuxming.cn

F. 文件与目录
来源：http://ewi.xingfuxueyuan.xyz

================================================================================
来源：http://fdy.epnwcf.com

[F01] 读取整个文件
来源：http://zgi.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vsb.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://rbk.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://olh.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tcw.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mzt.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gfy.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://ryc.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://rhu.jqgfzy.top

[F02] 逐行读取文件
来源：http://swj.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ept.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ghh.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://moa.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fyp.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uxg.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oqa.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://omy.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dek.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://mis.ehwqpu.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ggv.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ecl.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iin.xuanzx.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://knx.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bhr.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lct.hfpthk.cn

Ruby: File.write("a.txt", "hi")
来源：http://njo.ywan-chungtsiang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sqp.tian-w.cn

[F04] 追加写入文件
来源：http://myu.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xhi.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tiy.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://adu.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lpm.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zxu.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jgp.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vlg.jinghuilouyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ozz.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://zoo.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ryl.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://jxw.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://duv.316326.xyz

TS:   fs.existsSync("a.txt")
来源：http://nzc.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://akb.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://czx.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://uke.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://teb.9152youxi.cn

[F06] 删除文件
来源：http://iqg.meibo888.top

Py:   os.remove("a.txt")
来源：http://rvh.meibo888.top

PHP:  unlink("a.txt");
来源：http://fep.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jpd.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://rpa.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sfv.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://czd.cashguo.top


<!-- 参考信息 -->