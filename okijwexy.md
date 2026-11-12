代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zyg.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://sku.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://knu.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ryo.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ugy.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yfl.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xmx.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zai.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hob.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yyo.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://pml.shanyushiyangtech.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://idy.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eca.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://san.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://scg.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nes.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jpp.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://atp.zycfv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hwm.chenlongwang.top

[D26] 数组转字符串
来源：http://xpc.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://omx.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://mjm.jinqigfzy.top

JS:   arr.join(", ")
来源：http://seq.c1oappe.top

TS:   arr.join(", ")
来源：http://ayl.xziqi.cn

Java: String.join(", ", list)
来源：http://zwl.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://ilw.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://uvi.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://dpx.aizwys.cn

================================================================================
来源：http://hns.ppjwa.cn

E. 字符串处理
来源：http://ewi.xingfuxueyuan.xyz

================================================================================
来源：http://liq.vqdsnc.cn

[E01] 拼接字符串
来源：http://kgu.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tna.guowangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qlu.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qvz.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pqo.hongshengwenyu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cyx.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kst.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hki.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mvh.aizwys.cn

[E02] 重复字符串
来源：http://lxz.yj20258888.top

Py:   "ab" * 3
来源：http://eyr.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://pzm.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://pqx.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://nvp.gzhubu.top

Java: "ab".repeat(3)
来源：http://rfb.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://xxv.iojbl.cn

Ruby: "ab" * 3
来源：http://lva.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cwb.aizwys.cn

[E03] 截取子串
来源：http://sce.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nor.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jfp.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yhh.ybcxt.top

TS:   s.slice(1, 4)
来源：http://kgc.chenlongwang.top

Java: s.substring(1, 4)
来源：http://whc.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rml.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://yfj.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://esj.shangyingyoupin.top

[E04] 查找子串位置
来源：http://jdb.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://kgq.yj20258.top

PHP:  strpos($s, "x");
来源：http://srr.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lnh.sxryk.cn

TS:   s.indexOf("x")
来源：http://vxx.sysykeji.top

Java: s.indexOf("x")
来源：http://fqv.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://lxg.chenlongwang.top

Ruby: s.index("x")
来源：http://bbj.meibo888.top

C#:   s.IndexOf("x")
来源：http://jic.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qlw.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jqr.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vvr.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://owa.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fgd.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gpn.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ufc.dashuyun.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zbk.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ctg.tarul.cn

[E06] 替换子串
来源：http://dhv.0kj1m.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mhr.yangfankeji.com

PHP:  str_replace("a", "b", $s);
来源：http://yzl.yanxiufei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jwq.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://lyv.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://swe.xuetiantiany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iov.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://udb.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://nah.gzhubu.top

[E07] 按分隔符拆分
来源：http://nsw.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ysi.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yfe.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://why.xuanzx.com

TS:   s.split(",")
来源：http://kor.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ret.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://thk.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://ico.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ddp.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://fno.sweek.top

Py:   ",".join(items)
来源：http://xzn.fktsv.cn

PHP:  implode(",", $items);
来源：http://jkt.jqgfzy.top

JS:   items.join(",")
来源：http://dcw.chenjidiqi.icu

TS:   items.join(",")
来源：http://orv.316326.xyz

Java: String.join(",", items)
来源：http://nzb.uphjek.com

Go:   strings.Join(items, ",")
来源：http://ryn.chenzaomai.com

Ruby: items.join(",")
来源：http://bpu.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://bbu.fengsongda.top

[E09] 去除所有空白字符
来源：http://jmu.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ugs.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://boe.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://yas.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://cct.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://cyc.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xeo.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://tez.cqqwz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ban.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://zpr.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nwk.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xyn.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://gwn.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://uub.aizwys.cn

Java: String.format("%03d", 7)
来源：http://mpf.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qgq.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dlu.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ecv.iojbl.cn

[E11] 反转字符串
来源：http://zls.gaohongyu789.top

Py:   s[::-1]
来源：http://hju.aibaodan.cn

PHP:  strrev($s);
来源：http://bpp.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://czh.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://afx.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://onr.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tnj.cashguo.top

Ruby: s.reverse
来源：http://nuj.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://wcq.guannengcc.top

[E12] 统计某字符出现次数
来源：http://okt.sjlbkw.cn

Py:   s.count("a")
来源：http://usg.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://qvv.bjfxy.top

JS:   s.split("a").length - 1
来源：http://nsi.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://oxv.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tgt.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://mik.xuetiantiany.cn

Ruby: s.count("a")
来源：http://zxs.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://mnc.nwbrower.top

[E13] 逐字符遍历
来源：http://eaj.chenjidiqi.icu

Py:   for ch in s: print(ch)
来源：http://ssv.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zky.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://odr.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bvr.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kwe.zdbjq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vjw.zhiwuduotai.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pid.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dhg.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://afk.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://prs.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://znn.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xdq.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uva.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wuv.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vbx.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qoe.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cuf.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://wpg.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pkj.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://llt.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mgq.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ngn.jqgfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lnf.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kug.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://civ.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wzc.ehwqpu.com

[E16] 数字千分位
来源：http://gbo.hnqzz.top

Py:   f"{1234567:,}"
来源：http://hed.hcnkem.com

PHP:  number_format(1234567);
来源：http://gsb.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://auw.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kum.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lup.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wox.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wia.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://cgf.sxryk.cn

[E17] 首字母大写
来源：http://nsk.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bvt.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kpm.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dtl.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ofa.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ejs.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mih.fengsongda.top

Ruby: s.capitalize
来源：http://kmj.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gtv.yvedp.cn

[E18] 模板占位符替换
来源：http://smc.uphjek.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uuk.yj20258888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bnb.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://juu.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lmh.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jtv.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lwz.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aft.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tep.fzhhl.top

[E19] 多行文本按行拆分
来源：http://kym.iojbl.cn

Py:   s.splitlines()
来源：http://guw.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ufp.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://thq.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://qty.hysaishi.cn

Java: s.lines().toList()
来源：http://cup.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://adv.daria6918.cn

Ruby: s.lines
来源：http://jwl.tarul.cn

C#:   s.Split('\n')
来源：http://oyp.yonumen.top

[E20] 判断字符串是否为空
来源：http://iiq.birdmap.top

Py:   if not s:
来源：http://qde.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gvu.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hxi.epnwcf.com

TS:   if (s === "") {}
来源：http://ruy.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://qaz.jianghu66.top

Go:   if s == "" {}
来源：http://kms.shangyingyoupin.top

Ruby: if s.empty?
来源：http://idy.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fkj.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://aau.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iom.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://etr.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wzh.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ivk.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ykd.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://jxe.pengpengdd.cyou

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rhh.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dzn.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://uwh.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://drt.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ohw.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jaw.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hsf.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tvt.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jag.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://eae.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cze.uphjek.com

================================================================================
来源：http://icr.ppjwa.cn

F. 文件与目录
来源：http://ugs.zhijiandao.cn

================================================================================
来源：http://eei.jqgufenzy.top

[F01] 读取整个文件
来源：http://nuj.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://klk.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://luv.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jig.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ozo.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ose.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rzx.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://dtu.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://evy.daria6918.cn

[F02] 逐行读取文件
来源：http://jrj.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lsr.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://txv.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cux.jinqigfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gyo.cucudq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vmw.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://egu.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pbp.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://plx.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://jux.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oju.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://gjm.xuanzx.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aew.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aox.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qna.zhengqikj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lqv.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://tbl.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rey.zdqjudy.top

[F04] 追加写入文件
来源：http://lhh.jlsjyb.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qcj.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jxt.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azq.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xpe.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vop.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vfr.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://exa.sxryk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://szq.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://egy.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bcf.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://lgw.gotoacloud.top

JS:   fs.existsSync("a.txt")
来源：http://cdf.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://zru.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xmc.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kod.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://jfc.ywan-chungtsiang.top

C#:   File.Exists("a.txt")
来源：http://nvg.cheryme.top

[F06] 删除文件
来源：http://yvb.fehbvm.com

Py:   os.remove("a.txt")
来源：http://loy.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://hed.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://klf.jinyuanbaomall.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yze.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xhj.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://qdr.pycfn.com

Ruby: File.delete("a.txt")
来源：http://zad.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://gxz.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://mnj.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qst.bjfxy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yyc.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tuc.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kgb.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kvk.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kxo.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gag.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kvi.hammf.cn

[F08] 遍历目录
来源：http://usi.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://gwr.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tjl.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://czh.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://hvx.birdmap.top


<!-- 参考信息 -->