代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iqq.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://qeg.yongpay.top

Go:   // 手写循环
来源：http://nzi.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qsz.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hbl.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://dln.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://loe.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://syx.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zka.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vel.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mxj.zhongyouzk.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://obx.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nex.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dso.yongpay.top

[D25] Set 集合去重与交并差
来源：http://suc.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cwh.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jpf.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jlk.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://azp.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://obk.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wqu.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hdk.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ldu.yangfankeji.com

[D26] 数组转字符串
来源：http://ggp.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://yvh.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://lke.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://icg.nanxinkj.top

TS:   arr.join(", ")
来源：http://nkb.zhongyouzk.top

Java: String.join(", ", list)
来源：http://shz.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://tee.zhengqikj.top

Ruby: arr.join(", ")
来源：http://zpf.tarul.cn

C#:   string.Join(", ", list)
来源：http://lbk.fengsongda.top

================================================================================
来源：http://qxj.guannengcc.top

E. 字符串处理
来源：http://ucw.vehdjk.com

================================================================================
来源：http://vdx.yfazqb.com

[E01] 拼接字符串
来源：http://kdq.ydjk.org.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eoq.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kjp.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oce.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nvp.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ixl.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yjt.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bsc.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yny.ppjwa.cn

[E02] 重复字符串
来源：http://hdx.yuanzhike.top

Py:   "ab" * 3
来源：http://iqb.ppjwa.cn

PHP:  str_repeat("ab", 3);
来源：http://kwo.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://txb.sxryk.cn

TS:   "ab".repeat(3)
来源：http://vnz.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://whq.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://hsq.zhixingplan.top

Ruby: "ab" * 3
来源：http://bap.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gjx.pengpengdd.cyou

[E03] 截取子串
来源：http://qol.daxiang520.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rta.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ttg.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tkq.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://wzu.316326.xyz

Java: s.substring(1, 4)
来源：http://gkt.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yjz.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://tod.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://vaz.svipenyu.cn

[E04] 查找子串位置
来源：http://ses.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://jnx.shuidangran.top

PHP:  strpos($s, "x");
来源：http://zzv.fanxiaobao.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ltv.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://owv.zhijiandao.cn

Java: s.indexOf("x")
来源：http://tay.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://bvg.quarkkingdee.top

Ruby: s.index("x")
来源：http://osc.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://kzy.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gpm.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aqr.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://soq.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://btj.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jbr.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yrf.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ayj.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qoo.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cuc.9152youxi.cn

[E06] 替换子串
来源：http://ycb.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://grh.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://bor.cashguo.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ppj.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://mqz.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://psl.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nyn.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lzy.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://nvg.bbcook.cn

[E07] 按分隔符拆分
来源：http://qaw.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eyz.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xuf.yuxming.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://atw.yuxming.cn

TS:   s.split(",")
来源：http://tez.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://vhz.zhoulong.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qpn.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://btx.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://det.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://eib.yueranfly.top

Py:   ",".join(items)
来源：http://tii.cqqwz.cn

PHP:  implode(",", $items);
来源：http://bxh.zhongyouzk.top

JS:   items.join(",")
来源：http://vbl.shangyingyoupin.top

TS:   items.join(",")
来源：http://mus.andypj.xyz

Java: String.join(",", items)
来源：http://zbc.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://oin.wangdashe.top

Ruby: items.join(",")
来源：http://ery.fehbvm.com

C#:   string.Join(",", items)
来源：http://bhp.sysykeji.top

[E09] 去除所有空白字符
来源：http://nig.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hhg.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wak.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://gwc.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://aid.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://fju.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://xsb.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://sru.yj20258.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zhk.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://ppm.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vyg.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fkk.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://pet.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://tib.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://fau.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://axh.cdnleiting.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://axh.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kcx.nanxinkj.top

[E11] 反转字符串
来源：http://scm.chenzaomai.com

Py:   s[::-1]
来源：http://wqk.vqdsnc.cn

PHP:  strrev($s);
来源：http://fia.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://grb.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://rwd.pengpengdd.cyou

Java: new StringBuilder(s).reverse().toString()
来源：http://bih.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://fez.cheryme.top

Ruby: s.reverse
来源：http://mux.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://fla.yuxming.cn

[E12] 统计某字符出现次数
来源：http://pdu.hysaishi.cn

Py:   s.count("a")
来源：http://zzx.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://kos.iojbl.cn

JS:   s.split("a").length - 1
来源：http://wce.smart0.xyz

TS:   s.split("a").length - 1
来源：http://lcb.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ujj.sweek.top

Go:   strings.Count(s, "a")
来源：http://eqm.52xcode.cn

Ruby: s.count("a")
来源：http://vjj.haohaochexian.top

C#:   s.Count(c => c == 'a')
来源：http://bsb.epnwcf.com

[E13] 逐字符遍历
来源：http://sbk.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://itq.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://djb.zhaomingkeji.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://czo.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://xcn.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lfv.jlsjyb.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wvo.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bmb.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pwq.hcnkem.com

[E14] URL 编码与 Base64
来源：http://ajp.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://stv.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jkz.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kfy.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://smd.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jqx.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vmf.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uwm.jinqigufen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hxq.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://qbs.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fdy.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://heh.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://peo.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ght.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bax.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://btc.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ils.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://thi.jqgufenzy.top

[E16] 数字千分位
来源：http://iqf.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://saa.aibaodan.cn

PHP:  number_format(1234567);
来源：http://eae.hnxiangtu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hhx.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ila.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gow.xuanzx.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jye.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mnv.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://eov.c1oappe.top

[E17] 首字母大写
来源：http://avg.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zzi.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vvc.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hsu.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iac.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sdy.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qfo.tanke756.top

Ruby: s.capitalize
来源：http://oyx.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vge.cashguo.top

[E18] 模板占位符替换
来源：http://ktx.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://the.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fac.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uuw.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://bhk.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rbz.ybcxt.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wnh.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kcu.nwbrower.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://afo.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://ein.fehbvm.com

Py:   s.splitlines()
来源：http://vbx.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://utp.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://xvh.wangdashe.top

TS:   s.split(/\r?\n/)
来源：http://ynf.gaohongyu789.top

Java: s.lines().toList()
来源：http://erz.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://vkn.zycfv.cn

Ruby: s.lines
来源：http://fer.sxryk.cn

C#:   s.Split('\n')
来源：http://lke.cashguo.top

[E20] 判断字符串是否为空
来源：http://qto.pengpengdd.cyou

Py:   if not s:
来源：http://utk.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ezc.nwbrower.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wep.wangdashe.top

TS:   if (s === "") {}
来源：http://mja.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://fmm.52xcode.cn

Go:   if s == "" {}
来源：http://uby.ctjpmb.com

Ruby: if s.empty?
来源：http://yeb.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dkc.ppjwa.cn

[E21] 超长截断加省略号
来源：http://exi.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xut.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cwv.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hlr.hnxiangtu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jtp.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dth.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://iyl.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lty.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sdv.hammf.cn

[E22] 字节长度与字符长度
来源：http://qwk.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://med.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vzz.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dag.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ipg.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kdb.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://afa.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://qpf.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zwp.cheryme.top

================================================================================
来源：http://gjg.bbcook.cn

F. 文件与目录
来源：http://sbs.redwolf501.top

================================================================================
来源：http://ywr.cashguo.top

[F01] 读取整个文件
来源：http://nee.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dde.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://seo.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://niw.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mnr.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://snj.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yug.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://siw.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://dgs.ehwqpu.com

[F02] 逐行读取文件
来源：http://qcb.hesvh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dhb.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dmc.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gwd.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yoy.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cny.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wbc.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jxb.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://prm.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://kek.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://spl.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sgx.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kmy.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://umi.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wnw.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nok.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://bsl.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nro.hywenlv.cn

[F04] 追加写入文件
来源：http://scu.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nic.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fpy.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fna.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sqe.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xic.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zuf.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yey.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ges.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://qtz.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vfk.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://qqd.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://ksx.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://qvh.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hje.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tch.feifeiyinyue.top

Ruby: File.exist?("a.txt")
来源：http://mlw.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://gcm.hcnkem.com

[F06] 删除文件
来源：http://ffq.iojbl.cn

Py:   os.remove("a.txt")
来源：http://acx.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://fec.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://vcw.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://hkd.shangyingyoupin.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cux.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://qms.yonumen.top

Ruby: File.delete("a.txt")
来源：http://tvy.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://iqt.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://ove.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eox.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dkt.gogol.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dqw.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yii.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://udk.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gln.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bud.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eme.zhiwuduotai.top

[F08] 遍历目录
来源：http://hgc.dianchejie.cn


<!-- 参考信息 -->