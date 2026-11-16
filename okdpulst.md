代发 wailian999

[D23] reduce 累积计算
来源：http://ull.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fsj.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ozf.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gan.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://byt.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wqw.9152youxi.cn

Go:   // 手写循环
来源：http://gff.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tax.dianchejie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://okc.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://hem.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xoc.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mse.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dqc.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uvu.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://frc.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nsk.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sye.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vyy.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://pvq.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://okk.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://emw.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uho.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zmi.jianghu66.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kxo.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wdp.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yri.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fnl.shangyingyoupin.top

[D26] 数组转字符串
来源：http://fug.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://nvg.xuanzx.com

PHP:  implode(", ", $arr);
来源：http://sgl.jyoumei.cn

JS:   arr.join(", ")
来源：http://nfb.gogol.net.cn

TS:   arr.join(", ")
来源：http://iiy.jqgfzy.top

Java: String.join(", ", list)
来源：http://qyv.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://jun.0kj1m.cn

Ruby: arr.join(", ")
来源：http://ccu.guannengcc.top

C#:   string.Join(", ", list)
来源：http://dor.yj20258888.top

================================================================================
来源：http://lmg.svipenyu.cn

E. 字符串处理
来源：http://abu.daria6918.cn

================================================================================
来源：http://uay.yonumen.top

[E01] 拼接字符串
来源：http://sah.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ied.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qwj.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dao.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ril.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ktb.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zmm.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hwe.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nme.jiagoushi.top

[E02] 重复字符串
来源：http://muk.ydzc1.top

Py:   "ab" * 3
来源：http://hae.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://kmr.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://dqe.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://dpk.chenzaomai.com

Java: "ab".repeat(3)
来源：http://fnq.daria6918.cn

Go:   strings.Repeat("ab", 3)
来源：http://hbi.cucudq.cn

Ruby: "ab" * 3
来源：http://pwp.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xfg.fengsongda.top

[E03] 截取子串
来源：http://yan.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tcx.cucudq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://szt.ydjk.org.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wcf.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://sqk.hywenlv.cn

Java: s.substring(1, 4)
来源：http://lqk.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jzs.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qly.nanxinkj.top

C#:   s.Substring(1, 3)
来源：http://idt.yanxiufei.cn

[E04] 查找子串位置
来源：http://bvc.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://luj.andypj.xyz

PHP:  strpos($s, "x");
来源：http://yvh.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xgl.daria6918.cn

TS:   s.indexOf("x")
来源：http://yno.9152youxi.cn

Java: s.indexOf("x")
来源：http://pti.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://tcv.iojbl.cn

Ruby: s.index("x")
来源：http://zao.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://lpg.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lpx.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nkx.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sbh.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lzh.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mjm.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wpw.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://amv.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oet.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qfk.jinqigufen.top

[E06] 替换子串
来源：http://nzm.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qei.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://pdl.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wqe.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://crv.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ypm.ybcxt.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mzk.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dts.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://hyl.0kj1m.cn

[E07] 按分隔符拆分
来源：http://xmi.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sqn.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qtc.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gka.jinqigfzy.top

TS:   s.split(",")
来源：http://vua.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://rao.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wqc.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://hkw.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rwl.ydzc1.top

[E08] 数组按分隔符合并
来源：http://zvg.yonumen.top

Py:   ",".join(items)
来源：http://kbp.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://vij.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://fmw.yuanzhike.top

TS:   items.join(",")
来源：http://pvt.dianchejie.cn

Java: String.join(",", items)
来源：http://xxe.316326.xyz

Go:   strings.Join(items, ",")
来源：http://vdt.jlsjyb.cn

Ruby: items.join(",")
来源：http://bjj.yongpay.top

C#:   string.Join(",", items)
来源：http://rwc.redwolf501.top

[E09] 去除所有空白字符
来源：http://uyv.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gep.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oae.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://ujc.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://zui.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://ikr.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dlt.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://qki.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://reo.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://lml.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zvl.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pko.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://gvl.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://sak.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://uij.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fjc.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aun.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dyt.nanxinkj.top

[E11] 反转字符串
来源：http://idc.sufxvd.cn

Py:   s[::-1]
来源：http://uvy.yfazqb.com

PHP:  strrev($s);
来源：http://wsr.jqgufenzy.top

JS:   [...s].reverse().join("")
来源：http://stb.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://uzk.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cpi.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xqb.vehdjk.com

Ruby: s.reverse
来源：http://rje.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://oyz.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://xad.feifeiyinyue.top

Py:   s.count("a")
来源：http://dmv.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://ned.cheryme.top

JS:   s.split("a").length - 1
来源：http://xtj.ydzc1.top

TS:   s.split("a").length - 1
来源：http://ttc.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ufq.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://ilj.sweek.top

Ruby: s.count("a")
来源：http://ntr.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://niq.ydjk.org.cn

[E13] 逐字符遍历
来源：http://qyi.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://sfk.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://efu.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hhx.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bgu.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rwx.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nrb.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qmt.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rsd.hongshengwenyu.top

[E14] URL 编码与 Base64
来源：http://gxt.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mwb.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://evc.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wqu.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://owb.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://soh.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cex.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oqe.yanxiufei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bia.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://nxd.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zbz.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://daz.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jyc.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iss.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pgp.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kiq.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://paz.xylfe.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aki.fanxiaobao.xyz

[E16] 数字千分位
来源：http://vxc.sweek.top

Py:   f"{1234567:,}"
来源：http://zhr.tarul.cn

PHP:  number_format(1234567);
来源：http://jpo.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vjq.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pex.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rrd.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zjo.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kys.bbcook.cn

C#:   1234567.ToString("N0")
来源：http://ldq.guowangkeji.top

[E17] 首字母大写
来源：http://ywf.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ijs.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lxa.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://htw.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://chp.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hni.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eav.yuxming.cn

Ruby: s.capitalize
来源：http://uam.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://urg.ybcxt.top

[E18] 模板占位符替换
来源：http://ngj.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://olf.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ezc.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oui.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lba.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://taj.ivvv.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://paa.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://adp.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ktg.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://ucj.zhoulong.xyz

Py:   s.splitlines()
来源：http://trv.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hba.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://uyn.chenlongwang.top

TS:   s.split(/\r?\n/)
来源：http://vpl.dianchejie.cn

Java: s.lines().toList()
来源：http://ckf.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://rjw.snrcjt.cn

Ruby: s.lines
来源：http://nhn.zhongyouzk.top

C#:   s.Split('\n')
来源：http://cfx.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://syd.yonumen.top

Py:   if not s:
来源：http://jvo.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bxs.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://itx.fktsv.cn

TS:   if (s === "") {}
来源：http://mhr.fzhhl.top

Java: if (s.isEmpty()) {}
来源：http://ghn.yj20258888.top

Go:   if s == "" {}
来源：http://kjy.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://usl.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wql.sxryk.cn

[E21] 超长截断加省略号
来源：http://txh.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://edd.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://clj.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fte.0kj1m.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ucp.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://evm.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://gxx.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hwm.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://taq.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://ytg.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rcj.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wug.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lel.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://udd.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://obo.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sqs.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://bya.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dje.chenlongwang.top

================================================================================
来源：http://ssp.fengsongda.top

F. 文件与目录
来源：http://xky.feifeiyinyue.top

================================================================================
来源：http://orc.shangyingyoupin.top

[F01] 读取整个文件
来源：http://aho.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gaw.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://ven.tarul.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://umc.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sxu.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ckq.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zsh.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://qgd.gogol.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://jby.nwbrower.top

[F02] 逐行读取文件
来源：http://yge.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nrd.gaohongyu789.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oqg.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywg.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lij.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sax.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://don.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dhm.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ukh.ehwqpu.com

[F03] 写入文件（覆盖）
来源：http://oft.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jpd.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mxu.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wsp.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bbs.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://buw.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jji.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://qjs.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kwl.fktsv.cn

[F04] 追加写入文件
来源：http://bit.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://azi.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nus.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sux.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://opz.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ogb.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lhi.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nmq.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yyz.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://kdk.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aoq.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://oak.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://rhs.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://ddk.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ykr.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ztw.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://sqr.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://ffu.zhengqikj.top

[F06] 删除文件
来源：http://udl.yueranfly.top

Py:   os.remove("a.txt")
来源：http://xtj.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://mfs.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://xtw.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://epk.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://flm.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://jot.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://agi.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://nfv.yonumen.top

[F07] 创建目录（含多级）
来源：http://sgf.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xrn.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mdm.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ugp.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lqd.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gvk.sxryk.cn


<!-- 参考信息 -->