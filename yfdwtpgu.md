代发 wailian999

[D23] reduce 累积计算
来源：http://bjh.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vfu.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://heg.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hwi.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://omv.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://khg.yueranfly.top

Go:   // 手写循环
来源：http://aif.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jvx.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ybd.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://gdq.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bgo.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mwi.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kty.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hda.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ymr.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sat.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jgz.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mou.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://evt.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://thi.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hms.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yih.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lqp.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gsy.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qgx.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dqr.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yat.jinqigufen.top

[D26] 数组转字符串
来源：http://evs.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://iut.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://gvt.haohaochexian.top

JS:   arr.join(", ")
来源：http://wwv.shuidangran.top

TS:   arr.join(", ")
来源：http://lmi.iojbl.cn

Java: String.join(", ", list)
来源：http://ppt.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://kot.wangdashe.top

Ruby: arr.join(", ")
来源：http://vom.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://umv.hywenlv.cn

================================================================================
来源：http://koq.zhiwuduotai.top

E. 字符串处理
来源：http://thq.jlsjyb.cn

================================================================================
来源：http://wxb.jlsjyb.cn

[E01] 拼接字符串
来源：http://nuh.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rnn.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hdb.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bzd.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wdz.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xzb.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jim.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://owl.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sar.chenjidiqi.icu

[E02] 重复字符串
来源：http://ihw.sysykeji.top

Py:   "ab" * 3
来源：http://twh.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://xmi.guannengcc.top

JS:   "ab".repeat(3)
来源：http://mvy.hammf.cn

TS:   "ab".repeat(3)
来源：http://lem.hysaishi.cn

Java: "ab".repeat(3)
来源：http://ozi.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://iie.sweek.top

Ruby: "ab" * 3
来源：http://jjg.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bva.shzxlz.cn

[E03] 截取子串
来源：http://afz.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tpj.9152youxi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zhr.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bjn.tian-w.cn

TS:   s.slice(1, 4)
来源：http://lda.hnqzz.top

Java: s.substring(1, 4)
来源：http://vap.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ine.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://rdf.hammf.cn

C#:   s.Substring(1, 3)
来源：http://gpp.316326.xyz

[E04] 查找子串位置
来源：http://opz.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://crt.yongpay.top

PHP:  strpos($s, "x");
来源：http://ldd.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wgs.fehbvm.com

TS:   s.indexOf("x")
来源：http://oll.ctjpmb.com

Java: s.indexOf("x")
来源：http://mol.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://ujx.316326.xyz

Ruby: s.index("x")
来源：http://otj.epnwcf.com

C#:   s.IndexOf("x")
来源：http://smw.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ksb.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mvj.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://foo.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pbz.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://dyo.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zsg.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ejj.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iyi.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://opz.zhongyouzk.top

[E06] 替换子串
来源：http://wgw.zhoulong.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jdq.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://zth.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iyw.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://wyc.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nnu.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sbs.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hyk.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://uew.sufxvd.cn

[E07] 按分隔符拆分
来源：http://olh.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fwv.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://spa.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tnx.jiagoushi.top

TS:   s.split(",")
来源：http://dur.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://xmw.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mos.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://jvq.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qwp.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://mdy.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://vaw.yj20258888.top

PHP:  implode(",", $items);
来源：http://aal.zhixingplan.top

JS:   items.join(",")
来源：http://maj.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://zgg.jiagoushi.top

Java: String.join(",", items)
来源：http://gzr.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://pxh.hnxiangtu.top

Ruby: items.join(",")
来源：http://zuy.zdqjudy.top

C#:   string.Join(",", items)
来源：http://brv.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://wdz.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bdk.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zlp.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://uee.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://uhu.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://rmu.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eli.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kws.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wkb.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://klf.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://apg.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://los.hysaishi.cn

JS:   "7".padStart(3, "0")
来源：http://fgl.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://xjt.andypj.xyz

Java: String.format("%03d", 7)
来源：http://rfv.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://atw.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mxy.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vre.uphjek.com

[E11] 反转字符串
来源：http://cjp.zdbjq.cn

Py:   s[::-1]
来源：http://haw.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://bmn.316326.xyz

JS:   [...s].reverse().join("")
来源：http://lbr.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://cal.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gyj.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://aen.sweek.top

Ruby: s.reverse
来源：http://qum.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://mvw.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://sac.sjlbkw.cn

Py:   s.count("a")
来源：http://pqr.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://zcy.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://ruq.fktsv.cn

TS:   s.split("a").length - 1
来源：http://lwu.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jui.tarul.cn

Go:   strings.Count(s, "a")
来源：http://csw.xylfe.cn

Ruby: s.count("a")
来源：http://wfh.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://ptu.zhijiandao.cn

[E13] 逐字符遍历
来源：http://ilv.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://rbo.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uml.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uku.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yuo.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ggk.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qjb.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zmj.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zbr.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://ssa.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bex.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://hqi.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ujh.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kwe.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hwl.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zmo.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://utf.316326.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wzn.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://zkf.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nqr.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hpp.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lnv.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qop.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yef.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oud.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tbi.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eyy.redwolf501.top

[E16] 数字千分位
来源：http://pbo.xuanzx.com

Py:   f"{1234567:,}"
来源：http://cbd.jlsjyb.cn

PHP:  number_format(1234567);
来源：http://alv.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://trr.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://snt.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qhj.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sxu.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ggk.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://wko.yj20258.top

[E17] 首字母大写
来源：http://mgt.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://udp.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://nkw.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lct.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://muy.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://won.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mza.tarul.cn

Ruby: s.capitalize
来源：http://yxw.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rbi.jinqigfzy.top

[E18] 模板占位符替换
来源：http://ssn.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rvt.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://obe.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bki.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ama.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bsg.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nqj.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://glo.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jiy.yuxming.cn

[E19] 多行文本按行拆分
来源：http://iac.hfpthk.cn

Py:   s.splitlines()
来源：http://glx.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bcy.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://gxj.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://oml.tian-w.cn

Java: s.lines().toList()
来源：http://app.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://sgr.zhiwuduotai.top

Ruby: s.lines
来源：http://nuw.yfazqb.com

C#:   s.Split('\n')
来源：http://aik.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://cbz.iojbl.cn

Py:   if not s:
来源：http://wue.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ppz.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aom.quarkkingdee.top

TS:   if (s === "") {}
来源：http://ulz.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://pck.52xcode.cn

Go:   if s == "" {}
来源：http://lqa.jiagoushi.top

Ruby: if s.empty?
来源：http://ibe.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vgu.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://inl.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sir.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xro.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sgt.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://noa.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cja.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://ttn.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sxl.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dik.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://jmh.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tor.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwr.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dhw.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nyl.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yfw.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tqm.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://nqw.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pmp.zhijiandao.cn

================================================================================
来源：http://cbl.havefunace.top

F. 文件与目录
来源：http://iko.zdbjq.cn

================================================================================
来源：http://kng.c1oappe.top

[F01] 读取整个文件
来源：http://vnx.hcnkem.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://csz.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://ygj.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://okm.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yzf.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://lnw.chenlongwang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mgd.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://mtk.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://iaq.svipenyu.cn

[F02] 逐行读取文件
来源：http://ymd.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ljf.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hat.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://akj.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://agd.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jct.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iek.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jmc.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kot.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://bix.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mzj.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oxl.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vjn.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uce.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://npl.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qja.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://eia.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mpb.hongshengwenyu.top

[F04] 追加写入文件
来源：http://nzv.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://use.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qpd.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://haw.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vth.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://obs.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gwu.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fiy.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xnx.tarul.cn

[F05] 判断文件或目录是否存在
来源：http://dhj.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://quo.nanxinkj.top

PHP:  file_exists("a.txt");
来源：http://yer.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://pod.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://tpn.dashuyun.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://idt.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jsj.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://sxv.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://hjq.cheryme.top

[F06] 删除文件
来源：http://hcv.gzhubu.top

Py:   os.remove("a.txt")
来源：http://rvt.ydzc1.top

PHP:  unlink("a.txt");
来源：http://qwb.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://deb.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://zzd.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tgr.yongpay.top

Go:   os.Remove("a.txt")
来源：http://fnw.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://jxs.sweek.top

C#:   File.Delete("a.txt");
来源：http://pwx.jinqigufen.top

[F07] 创建目录（含多级）
来源：http://nor.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://izq.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://icr.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rzs.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aab.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yoc.shzxlz.cn


<!-- 参考信息 -->