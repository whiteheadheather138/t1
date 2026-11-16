代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aef.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uyw.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ypv.yj20258.top

[D26] 数组转字符串
来源：http://ydb.zhoulong.xyz

Py:   ", ".join(map(str, arr))
来源：http://dgt.bbcook.cn

PHP:  implode(", ", $arr);
来源：http://ule.pycfn.com

JS:   arr.join(", ")
来源：http://hbf.xziqi.cn

TS:   arr.join(", ")
来源：http://crl.ivvv.top

Java: String.join(", ", list)
来源：http://uhq.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://dft.0kj1m.cn

Ruby: arr.join(", ")
来源：http://ueo.fktsv.cn

C#:   string.Join(", ", list)
来源：http://lxo.sufxvd.cn

================================================================================
来源：http://smz.cashguo.top

E. 字符串处理
来源：http://jfg.kuanghao11.cn

================================================================================
来源：http://saw.meibo888.top

[E01] 拼接字符串
来源：http://pih.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mvd.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xdy.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://orb.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yzj.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yms.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xdm.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fjj.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xha.hfpthk.cn

[E02] 重复字符串
来源：http://hbu.chenjidiqi.icu

Py:   "ab" * 3
来源：http://ipf.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://nhx.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://qgi.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://tdq.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://znb.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://eul.ctjpmb.com

Ruby: "ab" * 3
来源：http://ruy.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yjx.jianghu66.top

[E03] 截取子串
来源：http://nae.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nbu.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hgs.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wdj.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://smy.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://pzb.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rhd.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://vhh.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://sfi.chenjidiqi.icu

[E04] 查找子串位置
来源：http://sei.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://ptf.316326.xyz

PHP:  strpos($s, "x");
来源：http://ojp.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://syz.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://uql.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://oco.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://mln.52xcode.cn

Ruby: s.index("x")
来源：http://fft.ivvv.top

C#:   s.IndexOf("x")
来源：http://zmv.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fbs.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kkj.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://igf.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ipp.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rvk.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sob.chenzaomai.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mnz.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gle.nanxuanxn.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jhy.jinyuanbaomall.cn

[E06] 替换子串
来源：http://oiv.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bgv.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://dpo.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ttm.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://gna.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xiy.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://glp.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kfc.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://iya.cucudq.cn

[E07] 按分隔符拆分
来源：http://mfr.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vmz.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xqy.yj202588.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bdo.zycfv.cn

TS:   s.split(",")
来源：http://ria.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://pvh.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zfa.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://obf.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sre.vehdjk.com

[E08] 数组按分隔符合并
来源：http://uzj.shzxlz.cn

Py:   ",".join(items)
来源：http://apj.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://qbo.yuxming.cn

JS:   items.join(",")
来源：http://afj.yvedp.cn

TS:   items.join(",")
来源：http://hnj.smart0.xyz

Java: String.join(",", items)
来源：http://rsq.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://bzd.xinyue.icu

Ruby: items.join(",")
来源：http://ymx.xylfe.cn

C#:   string.Join(",", items)
来源：http://vsy.fengsongda.top

[E09] 去除所有空白字符
来源：http://qjb.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fse.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ylh.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://ebw.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://uco.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://cdx.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://rzz.fanxiaobao.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://vvn.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://stb.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://igr.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://luj.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wks.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://ypi.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://njg.sjlbkw.cn

Java: String.format("%03d", 7)
来源：http://slm.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wsy.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://der.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gdg.aibaodan.cn

[E11] 反转字符串
来源：http://jvh.shanyushiyangtech.top

Py:   s[::-1]
来源：http://vjk.hnxiangtu.top

PHP:  strrev($s);
来源：http://ufj.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://tmm.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://ier.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qvf.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rcu.shuidangran.top

Ruby: s.reverse
来源：http://jtk.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://emt.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://myb.gotoacloud.top

Py:   s.count("a")
来源：http://qaq.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://hap.hammf.cn

JS:   s.split("a").length - 1
来源：http://dgf.yj20258.top

TS:   s.split("a").length - 1
来源：http://cyl.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://apm.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://lbr.meibo888.top

Ruby: s.count("a")
来源：http://kik.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://hvm.zdbjq.cn

[E13] 逐字符遍历
来源：http://ili.yj20258.top

Py:   for ch in s: print(ch)
来源：http://nli.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gsh.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bia.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bnm.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pic.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gqf.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://lue.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fuq.cashguo.top

[E14] URL 编码与 Base64
来源：http://fwx.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hst.mhx1999.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fvl.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gyk.cucudq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sat.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bcz.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://viz.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fyu.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://glo.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://bgy.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://blj.yj20258.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uar.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lij.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hcr.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rxk.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hqy.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gpd.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ljc.yongpay.top

[E16] 数字千分位
来源：http://vpt.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://ntj.sysykeji.top

PHP:  number_format(1234567);
来源：http://cbw.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rdc.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dck.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hyv.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hih.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hke.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://bvy.shzxlz.cn

[E17] 首字母大写
来源：http://heq.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fwc.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://clb.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kao.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lop.aibaodan.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pxv.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xiz.zhijiandao.cn

Ruby: s.capitalize
来源：http://nav.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nol.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://aur.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mtt.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pvf.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hup.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wws.hesvh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tag.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bwf.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qkc.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wgt.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://ngy.jiagoushi.top

Py:   s.splitlines()
来源：http://uzd.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bzx.cdnleiting.top

JS:   s.split(/\r?\n/)
来源：http://myc.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://zfr.316326.xyz

Java: s.lines().toList()
来源：http://nir.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://ana.xuanzx.com

Ruby: s.lines
来源：http://dpk.jlsjyb.cn

C#:   s.Split('\n')
来源：http://kjt.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://kdg.yuxming.cn

Py:   if not s:
来源：http://wbo.sweek.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dnt.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xnn.smart0.xyz

TS:   if (s === "") {}
来源：http://qpg.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://cnb.chenlongwang.top

Go:   if s == "" {}
来源：http://spl.mhx1999.top

Ruby: if s.empty?
来源：http://yqy.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://auc.xylfe.cn

[E21] 超长截断加省略号
来源：http://bst.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fem.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gby.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wmh.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gjn.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aaf.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://yhz.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jba.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aie.fehbvm.com

[E22] 字节长度与字符长度
来源：http://lsi.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fhe.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rqn.yueranfly.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eia.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://snq.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bcr.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mas.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://ghs.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wje.wangshuangyany.cn

================================================================================
来源：http://rft.zhongyouzk.top

F. 文件与目录
来源：http://nwi.fktsv.cn

================================================================================
来源：http://xoc.jqgufenzy.top

[F01] 读取整个文件
来源：http://ata.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wlt.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://sxi.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dvi.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wta.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zne.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jpo.gzhubu.top

Ruby: File.read("a.txt")
来源：http://jlg.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://xgx.meibo888.top

[F02] 逐行读取文件
来源：http://ykr.redwolf501.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://skm.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qaz.yonumen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ehc.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gmg.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mqs.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zmt.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xea.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ymm.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://nli.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pej.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bro.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dyu.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rfk.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gme.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vsz.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://zqr.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nex.fktsv.cn

[F04] 追加写入文件
来源：http://oxe.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ngg.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wxi.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xtw.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jhk.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qet.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ufm.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://evp.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lcc.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://qjv.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qhu.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://bjq.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://xku.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://nee.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mmg.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fjq.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://eoi.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://ljd.vqdsnc.cn

[F06] 删除文件
来源：http://zra.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://lqa.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://bbq.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://jkr.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://xei.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pgm.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://opw.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://akk.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://tga.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://jji.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cpc.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vzn.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zbq.jiagoushi.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://duz.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uhm.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://las.yj20258888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fmy.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jwo.sjlbkw.cn

[F08] 遍历目录
来源：http://zux.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bwr.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jml.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://lui.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://pli.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bux.sufxvd.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ezj.bjfxy.top

Ruby: Dir.children("dir")
来源：http://vwk.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://imm.yonumen.top

[F09] 获取文件大小
来源：http://uvj.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://oxt.sweek.top

PHP:  filesize("a.txt");
来源：http://lly.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://rau.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://atc.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kav.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bcr.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://kge.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://sfi.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://hbz.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tzq.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tmx.nanxuanxn.top


<!-- 参考信息 -->