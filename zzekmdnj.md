代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hsf.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wmu.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pfq.daria6918.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pfu.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qke.vehdjk.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://goy.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jnl.9152youxi.cn

[D26] 数组转字符串
来源：http://lia.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://fcs.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://lqe.zhixingplan.top

JS:   arr.join(", ")
来源：http://kky.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://pcs.snrcjt.cn

Java: String.join(", ", list)
来源：http://uid.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://qby.aibaodan.cn

Ruby: arr.join(", ")
来源：http://xdk.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://gxj.bbcook.cn

================================================================================
来源：http://uzk.0kj1m.cn

E. 字符串处理
来源：http://kyb.fzhhl.top

================================================================================
来源：http://yur.yuxming.cn

[E01] 拼接字符串
来源：http://ncm.yueranfly.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uuz.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ykd.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ndb.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nta.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pjb.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ibz.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uog.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wdf.hcnkem.com

[E02] 重复字符串
来源：http://rej.aibaodan.cn

Py:   "ab" * 3
来源：http://ppm.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://fgm.epnwcf.com

JS:   "ab".repeat(3)
来源：http://fqs.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://ebs.fzhhl.top

Java: "ab".repeat(3)
来源：http://vou.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://stx.cashguo.top

Ruby: "ab" * 3
来源：http://ylh.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ogf.bjfxy.top

[E03] 截取子串
来源：http://mfl.meibo888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sdx.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xzm.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vji.yj20258.top

TS:   s.slice(1, 4)
来源：http://udy.9152youxi.cn

Java: s.substring(1, 4)
来源：http://cyl.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mgs.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://tul.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://dwg.ctjpmb.com

[E04] 查找子串位置
来源：http://rrl.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://vwl.xylfe.cn

PHP:  strpos($s, "x");
来源：http://kae.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sfj.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://dgq.sjlbkw.cn

Java: s.indexOf("x")
来源：http://uyr.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://fmj.xziqi.cn

Ruby: s.index("x")
来源：http://hbn.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://uhr.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rni.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qnx.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ccm.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jxs.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://tdz.jyoumei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://esa.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lhm.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ani.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mls.ehwqpu.com

[E06] 替换子串
来源：http://gim.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://izz.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://mhy.guowangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aoi.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://knc.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bob.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xzf.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rcf.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://mve.ydzc1.top

[E07] 按分隔符拆分
来源：http://fsu.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dcm.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uym.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ltu.gotoacloud.top

TS:   s.split(",")
来源：http://aey.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://zrw.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qdk.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://lcy.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mxw.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://vsi.zycfv.cn

Py:   ",".join(items)
来源：http://lon.tianlin.xyz

PHP:  implode(",", $items);
来源：http://aiy.yj20258.top

JS:   items.join(",")
来源：http://hlo.nanxinkj.top

TS:   items.join(",")
来源：http://hxu.yongpay.top

Java: String.join(",", items)
来源：http://zjn.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://bpf.meibo888.top

Ruby: items.join(",")
来源：http://poj.yj20258888.top

C#:   string.Join(",", items)
来源：http://dlp.yuxming.cn

[E09] 去除所有空白字符
来源：http://tnz.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vff.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wfu.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://tmj.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://ocz.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://apy.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://knd.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://xcv.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zzk.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://auu.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cqi.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jld.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://rqw.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://dtg.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://tsv.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://hbm.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rrj.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://twq.jinqigufen.top

[E11] 反转字符串
来源：http://glc.gzhubu.top

Py:   s[::-1]
来源：http://afk.sjlbkw.cn

PHP:  strrev($s);
来源：http://hcw.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://hts.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://ilw.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://xsc.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yvj.gaohongyu789.top

Ruby: s.reverse
来源：http://zes.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://urw.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://clm.shangyingyoupin.top

Py:   s.count("a")
来源：http://yiu.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://yvp.bbcook.cn

JS:   s.split("a").length - 1
来源：http://jot.fehbvm.com

TS:   s.split("a").length - 1
来源：http://isn.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fmj.zdbjq.cn

Go:   strings.Count(s, "a")
来源：http://yhs.jlsjyb.cn

Ruby: s.count("a")
来源：http://amo.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://zwj.meibo888.top

[E13] 逐字符遍历
来源：http://ryv.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://kdr.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sjr.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wkv.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wiv.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://usc.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pwg.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vdp.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cio.ydjk.org.cn

[E14] URL 编码与 Base64
来源：http://gkp.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hvq.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rnv.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fym.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://usq.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nqz.hammf.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jgk.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wvr.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zcn.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://fkf.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oqj.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://evc.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dgw.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://afu.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mpf.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zvr.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jdi.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yrc.svipenyu.cn

[E16] 数字千分位
来源：http://ymw.xuanzx.com

Py:   f"{1234567:,}"
来源：http://gsf.316326.xyz

PHP:  number_format(1234567);
来源：http://uea.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iup.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pmh.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://evs.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ftf.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nqx.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://yfc.tianlin.xyz

[E17] 首字母大写
来源：http://hep.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rxd.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fae.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://air.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fuq.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mxj.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aaz.chenlongwang.top

Ruby: s.capitalize
来源：http://xkv.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tfm.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://ljf.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://koy.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yuz.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cjj.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oaf.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eev.nanxinkj.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jwu.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://awa.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://euu.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://ham.cashguo.top

Py:   s.splitlines()
来源：http://tke.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jdj.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://jxk.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://ovo.52xcode.cn

Java: s.lines().toList()
来源：http://ape.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://eww.jyoumei.cn

Ruby: s.lines
来源：http://srb.sxryk.cn

C#:   s.Split('\n')
来源：http://yha.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://fsl.xuanzx.com

Py:   if not s:
来源：http://and.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ixl.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hnt.hnqzz.top

TS:   if (s === "") {}
来源：http://mit.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://kos.jiagoushi.top

Go:   if s == "" {}
来源：http://xfi.yueranfly.top

Ruby: if s.empty?
来源：http://lcz.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bze.jinqigfzy.top

[E21] 超长截断加省略号
来源：http://rbb.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vck.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qhq.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vbs.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://szg.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://afu.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://uet.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cps.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nda.jianghu66.top

[E22] 字节长度与字符长度
来源：http://pjl.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ftt.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ent.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uco.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wwh.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baq.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://okb.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://fbl.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://czb.feifeiyinyue.top

================================================================================
来源：http://vgq.shangyingyoupin.top

F. 文件与目录
来源：http://hjw.xuanzx.com

================================================================================
来源：http://ucg.yuanzhike.top

[F01] 读取整个文件
来源：http://azk.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://god.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://jzp.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xmt.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wbc.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://val.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wqg.redwolf501.top

Ruby: File.read("a.txt")
来源：http://dmj.yonumen.top

C#:   File.ReadAllText("a.txt");
来源：http://uag.tianlin.xyz

[F02] 逐行读取文件
来源：http://rgu.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bvk.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zze.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rqf.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://slo.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://evy.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nrm.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jor.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rna.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://xgv.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vpb.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hbt.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xbp.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fnl.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dbz.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://avv.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://myv.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://puj.yvedp.cn

[F04] 追加写入文件
来源：http://ifc.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jet.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gut.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://raf.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://puy.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qxe.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jmt.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uyw.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uwt.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://hoo.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iva.xuanzx.com

PHP:  file_exists("a.txt");
来源：http://tkg.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://aca.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://jzy.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vtx.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://toh.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://cja.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://poe.xuetiantiany.cn

[F06] 删除文件
来源：http://lwi.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://rpz.andypj.xyz

PHP:  unlink("a.txt");
来源：http://hvq.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://yxf.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qxu.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xkq.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://yzx.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://vwh.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://pqf.cashguo.top

[F07] 创建目录（含多级）
来源：http://wur.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hjy.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ccz.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ofv.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jvy.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vdx.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uth.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cln.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wvg.dashuyun.cn

[F08] 遍历目录
来源：http://xcu.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ipu.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vgz.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://bfn.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://nhs.uphjek.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fgp.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://uzd.ivvv.top

Ruby: Dir.children("dir")
来源：http://vkd.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://nmn.yj20258888.top

[F09] 获取文件大小
来源：http://nho.zhaomingkeji.xyz

Py:   os.path.getsize("a.txt")
来源：http://hbs.ybcxt.top

PHP:  filesize("a.txt");
来源：http://jhf.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://esj.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://cgw.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://yhl.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kgo.havefunace.top

Ruby: File.size("a.txt")
来源：http://txt.fanxiaobao.xyz


<!-- 参考信息 -->