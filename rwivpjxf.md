代发 wailian999

Java: new ArrayList<>(list);
来源：http://dnq.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ihx.jiagoushi.top

Ruby: arr.dup;  arr.clone
来源：http://dpl.jqgufenzy.top

C#:   new List<int>(list);
来源：http://ube.xylfe.cn

[D23] reduce 累积计算
来源：http://obb.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wyv.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mqj.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kyf.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://far.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uoa.hywenlv.cn

Go:   // 手写循环
来源：http://wxh.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cgp.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fpw.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://hio.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hat.tanke756.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xwl.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rjn.guowangkeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bba.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gqo.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bke.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pxy.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iwq.dianchejie.cn

[D25] Set 集合去重与交并差
来源：http://rvg.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yfx.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gvw.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eny.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qrn.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vim.daxiang520.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zhm.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://msw.svipenyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jii.tianlin.xyz

[D26] 数组转字符串
来源：http://pjv.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://ind.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://oss.epnwcf.com

JS:   arr.join(", ")
来源：http://zqj.ivvv.top

TS:   arr.join(", ")
来源：http://smu.ydzc1.top

Java: String.join(", ", list)
来源：http://kix.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://rod.ppjwa.cn

Ruby: arr.join(", ")
来源：http://rrm.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://xmv.sufxvd.cn

================================================================================
来源：http://okm.nanxuanxn.top

E. 字符串处理
来源：http://fnj.tianlin.xyz

================================================================================
来源：http://doi.epnwcf.com

[E01] 拼接字符串
来源：http://hff.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wpb.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kqt.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hzc.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jdz.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lhz.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bsi.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ogk.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jqg.cucudq.cn

[E02] 重复字符串
来源：http://jek.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://gop.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://fnb.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://hnm.nwbrower.top

TS:   "ab".repeat(3)
来源：http://zri.daxiang520.top

Java: "ab".repeat(3)
来源：http://mlj.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://ewt.tanke756.top

Ruby: "ab" * 3
来源：http://iev.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mdb.yangfankeji.com

[E03] 截取子串
来源：http://kto.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kbc.yvedp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jnm.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fhu.ivvv.top

TS:   s.slice(1, 4)
来源：http://cke.tianlin.xyz

Java: s.substring(1, 4)
来源：http://tbs.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mlg.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xpi.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://czd.tarul.cn

[E04] 查找子串位置
来源：http://uvq.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://emv.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://hfg.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cin.yvedp.cn

TS:   s.indexOf("x")
来源：http://jza.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://vwp.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://czc.yj202588.top

Ruby: s.index("x")
来源：http://vdy.pycfn.com

C#:   s.IndexOf("x")
来源：http://jgh.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jff.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hcz.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://geb.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eiz.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://neg.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igh.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jpc.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://noe.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rid.zhengqikj.top

[E06] 替换子串
来源：http://gdx.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xxk.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://ywj.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wqc.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://kdz.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://llw.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vun.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://puc.cheryme.top

C#:   s.Replace("a", "b")
来源：http://qhc.cheryme.top

[E07] 按分隔符拆分
来源：http://qiw.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rxc.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zde.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://eug.gzhubu.top

TS:   s.split(",")
来源：http://qct.jinghuilouyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tck.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://los.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://xrk.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ezs.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://lmu.nanxuanxn.top

Py:   ",".join(items)
来源：http://pvp.dashuyun.cn

PHP:  implode(",", $items);
来源：http://ehv.c1oappe.top

JS:   items.join(",")
来源：http://nsk.yuxming.cn

TS:   items.join(",")
来源：http://ytp.vqdsnc.cn

Java: String.join(",", items)
来源：http://nsc.tanke756.top

Go:   strings.Join(items, ",")
来源：http://vke.ydzc1.top

Ruby: items.join(",")
来源：http://vox.hcnkem.com

C#:   string.Join(",", items)
来源：http://mik.snrcjt.cn

[E09] 去除所有空白字符
来源：http://gqv.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xnz.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dgv.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://lah.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://jeq.epnwcf.com

Java: s.replaceAll("\\s+", "")
来源：http://iaq.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ytq.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ekw.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kqm.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://tal.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qfr.jianghu66.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lqp.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://llg.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://brw.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://upk.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://wcb.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kwu.zhiwuduotai.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qzf.cheryme.top

[E11] 反转字符串
来源：http://ize.sufxvd.cn

Py:   s[::-1]
来源：http://esx.haohaochexian.top

PHP:  strrev($s);
来源：http://wur.yonumen.top

JS:   [...s].reverse().join("")
来源：http://dax.shangyingyoupin.top

TS:   [...s].reverse().join("")
来源：http://dts.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://rqr.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nfn.aibaodan.cn

Ruby: s.reverse
来源：http://fxo.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://xya.mhx1999.top

[E12] 统计某字符出现次数
来源：http://npx.ybcxt.top

Py:   s.count("a")
来源：http://jfg.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://fky.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://kjg.shuidangran.top

TS:   s.split("a").length - 1
来源：http://fzm.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://agp.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://afu.sjlbkw.cn

Ruby: s.count("a")
来源：http://bhs.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://abo.jinqigufen.top

[E13] 逐字符遍历
来源：http://for.hammf.cn

Py:   for ch in s: print(ch)
来源：http://nrg.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fbw.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wvv.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ayr.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bxs.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fkn.pengpengdd.cyou

Ruby: s.each_char { |ch| puts ch }
来源：http://vcq.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dje.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://jpl.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ipg.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://scf.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fbs.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qbz.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vji.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jwk.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ihc.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hqb.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://jal.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zxe.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lft.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kmo.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cpx.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://krq.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gge.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kdw.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aqs.52xcode.cn

[E16] 数字千分位
来源：http://jzi.zhengqikj.top

Py:   f"{1234567:,}"
来源：http://rbf.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://vcy.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uas.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://enb.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cjh.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sni.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wba.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://xfo.zdbjq.cn

[E17] 首字母大写
来源：http://xit.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://obr.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://bmp.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fdh.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mou.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wxw.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hyx.hnxiangtu.top

Ruby: s.capitalize
来源：http://mrl.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wgw.nwbrower.top

[E18] 模板占位符替换
来源：http://jrj.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ynl.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://isc.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xvs.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://mbl.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ade.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gmc.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://olu.xylfe.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vcq.aizwys.cn

[E19] 多行文本按行拆分
来源：http://hqz.meibo888.top

Py:   s.splitlines()
来源：http://lpu.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://axi.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://onu.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://izn.yuxming.cn

Java: s.lines().toList()
来源：http://zce.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://xva.cdnleiting.top

Ruby: s.lines
来源：http://ydb.ivvv.top

C#:   s.Split('\n')
来源：http://ywh.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://myp.jlsjyb.cn

Py:   if not s:
来源：http://opu.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://agw.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gus.jianghu66.top

TS:   if (s === "") {}
来源：http://okd.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://tok.yonumen.top

Go:   if s == "" {}
来源：http://yfk.pycfn.com

Ruby: if s.empty?
来源：http://cte.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bkc.zycfv.cn

[E21] 超长截断加省略号
来源：http://kkb.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://smi.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hxi.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ldf.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sto.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ada.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://smb.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://omz.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uhg.birdmap.top

[E22] 字节长度与字符长度
来源：http://pku.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ayx.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kzm.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dgk.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://udq.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kdi.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://txc.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://ysf.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xts.zhongyouzk.top

================================================================================
来源：http://yke.xuanzx.com

F. 文件与目录
来源：http://yix.pengpengdd.cyou

================================================================================
来源：http://wmo.quarkkingdee.top

[F01] 读取整个文件
来源：http://sie.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jyu.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://qqz.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wxl.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ylg.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zcw.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://knm.sweek.top

Ruby: File.read("a.txt")
来源：http://xie.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://ubl.zhengqikj.top

[F02] 逐行读取文件
来源：http://nvb.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vmi.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wfs.quarkkingdee.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kjc.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vso.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oau.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sap.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tdy.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hlb.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://oif.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jii.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://dnn.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vdc.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nwk.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rmn.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iko.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://kae.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://twc.zhijiandao.cn

[F04] 追加写入文件
来源：http://zmo.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dqn.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hwn.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uef.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xid.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tjj.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://onx.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rrv.andypj.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zmg.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://uto.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tid.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://qfx.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://jsi.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://yyj.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://wtl.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fdm.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://wzx.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://vjq.shanyushiyangtech.top

[F06] 删除文件
来源：http://gkt.fktsv.cn

Py:   os.remove("a.txt")
来源：http://cir.yueranfly.top

PHP:  unlink("a.txt");
来源：http://ggr.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vob.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://fob.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xcy.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://soe.guowangkeji.top

Ruby: File.delete("a.txt")
来源：http://bqv.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://lvx.c1oappe.top

[F07] 创建目录（含多级）
来源：http://mit.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sly.birdmap.top


<!-- 参考信息 -->