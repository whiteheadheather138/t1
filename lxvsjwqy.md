代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eag.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rrx.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wjd.jinyuanbaomall.cn

TS:   [...arr];
来源：http://lyw.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://ibz.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://ske.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://llm.xuanzx.com

C#:   new List<int>(list);
来源：http://cgq.yongpay.top

[D23] reduce 累积计算
来源：http://hia.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pgf.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yxf.yueranfly.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://alr.yj20258888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bgp.zdqjudy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://umd.wangdashe.top

Go:   // 手写循环
来源：http://bet.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xyx.nanxuanxn.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cnp.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://cfd.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lfb.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oos.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eki.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cdm.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gpf.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tqy.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wcz.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fkt.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://apj.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vik.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dps.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eko.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bqr.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://coe.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kqo.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tsz.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ule.hysaishi.cn

[D26] 数组转字符串
来源：http://fcy.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://hol.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://meu.gaohongyu789.top

JS:   arr.join(", ")
来源：http://flv.smart0.xyz

TS:   arr.join(", ")
来源：http://bem.yuxming.cn

Java: String.join(", ", list)
来源：http://acp.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://ukb.bjfxy.top

Ruby: arr.join(", ")
来源：http://dqb.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://pmc.zhaomingkeji.xyz

================================================================================
来源：http://nfl.jinqigfzy.top

E. 字符串处理
来源：http://mfp.xziqi.cn

================================================================================
来源：http://hzn.zdbjq.cn

[E01] 拼接字符串
来源：http://zuz.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://udh.havefunace.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kim.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tnf.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hso.dianchejie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kfh.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wgt.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kbq.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://htr.dianchejie.cn

[E02] 重复字符串
来源：http://dfb.jqgufenzy.top

Py:   "ab" * 3
来源：http://jwr.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://idu.fzhhl.top

JS:   "ab".repeat(3)
来源：http://add.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://uxd.gotoacloud.top

Java: "ab".repeat(3)
来源：http://mao.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://sus.hesvh.cn

Ruby: "ab" * 3
来源：http://gau.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nnp.vqdsnc.cn

[E03] 截取子串
来源：http://edj.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://awz.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vlk.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ymg.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://nkd.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://haa.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ysx.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://cvp.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://qrj.yj20258.top

[E04] 查找子串位置
来源：http://vcr.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://mjo.xuanzx.com

PHP:  strpos($s, "x");
来源：http://uqv.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rkp.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://mvd.yuanzhike.top

Java: s.indexOf("x")
来源：http://tci.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://aht.yanxiufei.cn

Ruby: s.index("x")
来源：http://ghd.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://ufj.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://evy.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kyq.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fsj.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sqb.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dil.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dhn.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://erj.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bqa.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tfa.kuanghao11.cn

[E06] 替换子串
来源：http://qqj.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kan.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://lnr.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oea.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://qkf.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aif.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gow.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://epj.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://kli.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://dhy.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ipr.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bis.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pjm.jqgfzy.top

TS:   s.split(",")
来源：http://ztb.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://psy.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pgk.hongshengwenyu.top

Ruby: s.split(",");  s.split
来源：http://uva.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://orh.yuxming.cn

[E08] 数组按分隔符合并
来源：http://egj.aibaodan.cn

Py:   ",".join(items)
来源：http://omq.yongpay.top

PHP:  implode(",", $items);
来源：http://amq.yj202588.top

JS:   items.join(",")
来源：http://yax.sjlbkw.cn

TS:   items.join(",")
来源：http://kih.wangdashe.top

Java: String.join(",", items)
来源：http://aui.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://lhj.nanxuanxn.top

Ruby: items.join(",")
来源：http://dkx.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://ndm.bjfxy.top

[E09] 去除所有空白字符
来源：http://ibk.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jgu.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zyp.yanxiufei.cn

JS:   s.replace(/\s+/g, "")
来源：http://vrv.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://hws.guowangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://vup.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://llq.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://nsc.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kvb.hnqzz.top

[E10] 左侧补零 / 定长填充
来源：http://ttf.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zzk.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://obl.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://khk.sufxvd.cn

TS:   "7".padStart(3, "0")
来源：http://chw.sjlbkw.cn

Java: String.format("%03d", 7)
来源：http://mwc.9152youxi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mba.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uuy.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xfw.fengsongda.top

[E11] 反转字符串
来源：http://gah.hcnkem.com

Py:   s[::-1]
来源：http://mcr.daxiang520.top

PHP:  strrev($s);
来源：http://fdw.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://oca.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://mst.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ccq.hammf.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dzc.haohaochexian.top

Ruby: s.reverse
来源：http://awc.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://hnw.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://hde.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://nft.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://qvk.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://ohw.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://usq.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pcn.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://vov.quarkkingdee.top

Ruby: s.count("a")
来源：http://zwc.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://sjc.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://klq.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://nxb.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rlo.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vtj.nanxuanxn.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cuq.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kcm.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dhg.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zia.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bjw.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://juw.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tfy.bbcook.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wdk.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://thy.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dir.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jpm.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://soh.bbcook.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tsn.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gzw.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://she.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zbd.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yft.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dzv.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ebq.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://owy.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vbn.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jlo.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lkd.gzhubu.top

[E16] 数字千分位
来源：http://lrn.daxiang520.top

Py:   f"{1234567:,}"
来源：http://loi.zhixingplan.top

PHP:  number_format(1234567);
来源：http://ztj.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jgj.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fsi.birdmap.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qmb.chenzaomai.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uxk.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lva.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://xfb.shanyushiyangtech.top

[E17] 首字母大写
来源：http://ooo.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yac.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://moh.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hzo.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://seo.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://irv.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xky.hywenlv.cn

Ruby: s.capitalize
来源：http://tla.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zde.316326.xyz

[E18] 模板占位符替换
来源：http://tll.vehdjk.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wex.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rnv.zdbjq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zda.hesvh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://alu.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hcp.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rsq.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hud.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vrw.iojbl.cn

[E19] 多行文本按行拆分
来源：http://btu.ydzc1.top

Py:   s.splitlines()
来源：http://rgl.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://shr.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://cfc.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://jvt.hfpthk.cn

Java: s.lines().toList()
来源：http://wac.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://bec.ivvv.top

Ruby: s.lines
来源：http://eyi.zdqjudy.top

C#:   s.Split('\n')
来源：http://ald.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://fxp.ybcxt.top

Py:   if not s:
来源：http://hrp.yj202588.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lfj.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gog.zhaomingkeji.xyz

TS:   if (s === "") {}
来源：http://kdd.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://cky.yongpay.top

Go:   if s == "" {}
来源：http://yln.gogol.net.cn

Ruby: if s.empty?
来源：http://rvo.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uvw.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://vkq.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wad.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ysi.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://obh.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jfr.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nsr.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://req.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yph.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tcu.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://qgu.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zjj.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xze.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mtt.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://npf.zdqjudy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ipv.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mcp.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://eyr.sysykeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mwd.sufxvd.cn

================================================================================
来源：http://efq.gzhubu.top

F. 文件与目录
来源：http://auo.aizwys.cn

================================================================================
来源：http://vlf.hongshengwenyu.top

[F01] 读取整个文件
来源：http://jme.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ikh.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://eem.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gxl.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gaq.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://jxk.pengpengdd.cyou

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dpl.jianghu66.top

Ruby: File.read("a.txt")
来源：http://rcw.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://gix.yonumen.top

[F02] 逐行读取文件
来源：http://ibi.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ngb.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dws.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zjo.jqgufenzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jgr.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gcl.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qen.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://abe.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uah.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://vxw.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tla.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://iun.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aat.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wnq.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rtr.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pcr.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://zxn.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jkp.zdbjq.cn

[F04] 追加写入文件
来源：http://vmj.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://szn.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uxk.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gbp.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rdc.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://syd.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rmm.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zkq.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wit.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://pmy.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dgs.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://ogl.fengsongda.top

JS:   fs.existsSync("a.txt")
来源：http://rhw.xuetiantiany.cn

TS:   fs.existsSync("a.txt")
来源：http://frh.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cnh.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mej.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://uwz.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://hcy.redwolf501.top

[F06] 删除文件
来源：http://wjz.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://uha.c1oappe.top

PHP:  unlink("a.txt");
来源：http://wcm.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sgu.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://dff.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kfp.yj20258.top

Go:   os.Remove("a.txt")
来源：http://otx.aizwys.cn


<!-- 参考信息 -->