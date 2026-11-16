代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://oau.jinqigfzy.top

JS:   arr.includes(x)
来源：http://unm.aizwys.cn

TS:   arr.includes(x)
来源：http://adp.pengpengdd.cyou

Java: list.contains(x)
来源：http://igk.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://tgd.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://dow.zhixingplan.top

C#:   list.Contains(x)
来源：http://qol.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://myj.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zgr.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fvs.hcnkem.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pfh.yongpay.top

TS:   [...arr];
来源：http://kid.epnwcf.com

Java: new ArrayList<>(list);
来源：http://ecq.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pfh.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://sel.wangshuangyany.cn

C#:   new List<int>(list);
来源：http://igd.pycfn.com

[D23] reduce 累积计算
来源：http://oyp.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rnf.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qdx.wangshuangyany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dec.yuxming.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jaa.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yzu.birdmap.top

Go:   // 手写循环
来源：http://owz.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nyk.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ecb.gaohongyu789.top

[D24] 字典 / Map 基本操作
来源：http://itb.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jha.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://isn.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ngq.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fsq.yj20258888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ysf.jqgfzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://srs.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fqn.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qgd.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://ryq.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mco.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gwn.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lmd.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ylt.nanxinkj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ynz.yj202588.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jbx.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oji.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gkx.yj20258.top

[D26] 数组转字符串
来源：http://ikn.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://jsq.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://klk.ywan-chungtsiang.top

JS:   arr.join(", ")
来源：http://jyc.daxiang520.top

TS:   arr.join(", ")
来源：http://qwi.cheryme.top

Java: String.join(", ", list)
来源：http://vng.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://hmq.yj20258.top

Ruby: arr.join(", ")
来源：http://kas.fehbvm.com

C#:   string.Join(", ", list)
来源：http://chn.sjlbkw.cn

================================================================================
来源：http://jgd.jinqigufen.top

E. 字符串处理
来源：http://lae.yfazqb.com

================================================================================
来源：http://cre.hongshengwenyu.top

[E01] 拼接字符串
来源：http://kdf.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lld.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ull.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://myb.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blc.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fax.jyoumei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yea.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hmg.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bgk.0kj1m.cn

[E02] 重复字符串
来源：http://tvv.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://esa.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://mez.meibo888.top

JS:   "ab".repeat(3)
来源：http://mvl.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://jof.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://ryn.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://lok.ctjpmb.com

Ruby: "ab" * 3
来源：http://vnn.redwolf501.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xwu.zhixingplan.top

[E03] 截取子串
来源：http://wnv.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wwe.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fob.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xve.c1oappe.top

TS:   s.slice(1, 4)
来源：http://usa.svipenyu.cn

Java: s.substring(1, 4)
来源：http://pbn.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hpq.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gci.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://eef.gogol.net.cn

[E04] 查找子串位置
来源：http://qws.zhaomingkeji.xyz

Py:   s.find("x");  s.index("x")
来源：http://gxg.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://wop.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://smh.jyoumei.cn

TS:   s.indexOf("x")
来源：http://yqt.fzhhl.top

Java: s.indexOf("x")
来源：http://act.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://afo.zhoulong.xyz

Ruby: s.index("x")
来源：http://bib.mhx1999.top

C#:   s.IndexOf("x")
来源：http://vwm.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://trm.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gbo.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qnv.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ark.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uhv.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uxf.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gop.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xks.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vig.iojbl.cn

[E06] 替换子串
来源：http://oub.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://phv.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://oyh.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kmu.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://mma.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bky.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://emc.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yii.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://ngk.yonumen.top

[E07] 按分隔符拆分
来源：http://vnc.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://avo.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hqv.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vig.yj20258.top

TS:   s.split(",")
来源：http://qlz.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pon.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lwu.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://xqz.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://esx.mhx1999.top

[E08] 数组按分隔符合并
来源：http://bll.pycfn.com

Py:   ",".join(items)
来源：http://ylj.haohaochexian.top

PHP:  implode(",", $items);
来源：http://wnp.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://nyy.jinqigufen.top

TS:   items.join(",")
来源：http://qep.wangdashe.top

Java: String.join(",", items)
来源：http://cic.yj202588.top

Go:   strings.Join(items, ",")
来源：http://mcc.hfpthk.cn

Ruby: items.join(",")
来源：http://spa.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://axp.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://lng.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fdm.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xvk.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://okc.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://xxv.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://knl.bbcook.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iyi.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://czf.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lfl.zycfv.cn

[E10] 左侧补零 / 定长填充
来源：http://jqo.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qrh.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ycg.bjfxy.top

JS:   "7".padStart(3, "0")
来源：http://zxe.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://acu.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://kdj.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xom.daria6918.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jpk.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gvm.jianghu66.top

[E11] 反转字符串
来源：http://oqw.bbcook.cn

Py:   s[::-1]
来源：http://ggb.cdnleiting.top

PHP:  strrev($s);
来源：http://cro.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://nbz.cheryme.top

TS:   [...s].reverse().join("")
来源：http://rlb.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://rzi.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rkh.xuetiantiany.cn

Ruby: s.reverse
来源：http://jsr.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://wui.xuanzx.com

[E12] 统计某字符出现次数
来源：http://gib.9152youxi.cn

Py:   s.count("a")
来源：http://njw.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://kyh.xuanzx.com

JS:   s.split("a").length - 1
来源：http://jga.hesvh.cn

TS:   s.split("a").length - 1
来源：http://cov.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jid.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://zye.zhengqikj.top

Ruby: s.count("a")
来源：http://kzp.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://fgp.ehwqpu.com

[E13] 逐字符遍历
来源：http://qjb.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://czp.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zxq.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dce.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qux.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yjo.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cao.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ogy.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hhz.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://rvt.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nob.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zls.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mbo.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://erw.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://teq.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mmk.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ofz.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ymk.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://ixf.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sxv.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hcl.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fsg.vqdsnc.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://smq.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mhf.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://prj.zycfv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zxc.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://voq.yueranfly.top

[E16] 数字千分位
来源：http://uyd.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://hdx.tian-w.cn

PHP:  number_format(1234567);
来源：http://dlw.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ggr.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pnp.haohaochexian.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tql.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vzk.52xcode.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tlk.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://xfc.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://qvh.jinghuilouyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zfq.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fah.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqg.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kmc.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://knm.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://glt.shzxlz.cn

Ruby: s.capitalize
来源：http://ici.cheryme.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vto.yj202588.top

[E18] 模板占位符替换
来源：http://bpr.jiagoushi.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ulq.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wjn.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://cow.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lbo.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dhd.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ory.ctjpmb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lcf.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aab.cheryme.top

[E19] 多行文本按行拆分
来源：http://wbu.vqdsnc.cn

Py:   s.splitlines()
来源：http://rcl.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lxx.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://pil.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://zbu.pengpengdd.cyou

Java: s.lines().toList()
来源：http://tgg.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://qag.tarul.cn

Ruby: s.lines
来源：http://fvi.zhengqikj.top

C#:   s.Split('\n')
来源：http://ggm.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://vrr.shanyushiyangkeji.top

Py:   if not s:
来源：http://dnu.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sto.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jdd.jqgufenzy.top

TS:   if (s === "") {}
来源：http://cld.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://whx.vehdjk.com

Go:   if s == "" {}
来源：http://zvm.yuanzhike.top

Ruby: if s.empty?
来源：http://rkp.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vgv.c1oappe.top

[E21] 超长截断加省略号
来源：http://ftx.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://myd.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://noi.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bix.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ayb.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yig.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://lsq.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tfj.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bke.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://cfy.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qgz.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hiu.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ctn.xingfuxueyuan.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ded.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tdq.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://doo.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://asi.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://glz.tarul.cn

================================================================================
来源：http://bil.hywenlv.cn

F. 文件与目录
来源：http://ypl.nanxuanxn.top

================================================================================
来源：http://xho.meibo888.top

[F01] 读取整个文件
来源：http://blf.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qyo.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://mch.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fnw.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://skj.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ixo.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bit.yj20258.top

Ruby: File.read("a.txt")
来源：http://qqm.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://tmn.dianchejie.cn

[F02] 逐行读取文件
来源：http://uba.zhoulong.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qak.gaohongyu789.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://puj.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ekh.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tct.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qlg.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kvs.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xlo.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://igr.bbcook.cn

[F03] 写入文件（覆盖）
来源：http://wnm.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xgs.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bno.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://koa.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://omu.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://apq.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cbe.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://qgg.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ord.vehdjk.com

[F04] 追加写入文件
来源：http://ooz.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sfh.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ekt.gotoacloud.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://szo.jinghuilouyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pli.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vyu.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nzn.hywenlv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iao.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zjs.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://ysg.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://chk.havefunace.top

PHP:  file_exists("a.txt");
来源：http://hbh.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://xjf.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://dce.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ypd.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jpu.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://say.zhoulong.xyz


<!-- 参考信息 -->