代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://qgq.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://wel.hnqzz.top

JS:   arr.join(", ")
来源：http://onv.vehdjk.com

TS:   arr.join(", ")
来源：http://wvx.haohaochexian.top

Java: String.join(", ", list)
来源：http://krs.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://ruj.haohaochexian.top

Ruby: arr.join(", ")
来源：http://vno.redwolf501.top

C#:   string.Join(", ", list)
来源：http://ktk.hcnkem.com

================================================================================
来源：http://jka.iojbl.cn

E. 字符串处理
来源：http://oso.cqqwz.cn

================================================================================
来源：http://rjj.hcnkem.com

[E01] 拼接字符串
来源：http://hfz.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uhf.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mqz.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mzx.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gdl.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vzc.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://upn.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jst.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ebb.fktsv.cn

[E02] 重复字符串
来源：http://xnn.jyoumei.cn

Py:   "ab" * 3
来源：http://igp.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://nil.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://uso.cashguo.top

TS:   "ab".repeat(3)
来源：http://iwk.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://thx.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://tyo.shzxlz.cn

Ruby: "ab" * 3
来源：http://xef.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wez.jinqigfzy.top

[E03] 截取子串
来源：http://jpz.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hge.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nwi.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ece.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://njv.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://rfg.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kpi.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://tfj.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://alo.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://bao.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://ehd.cheryme.top

PHP:  strpos($s, "x");
来源：http://jzb.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lts.cdnleiting.top

TS:   s.indexOf("x")
来源：http://ohi.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://xwq.yongpay.top

Go:   strings.Index(s, "x")
来源：http://egr.ydjk.org.cn

Ruby: s.index("x")
来源：http://pdc.yfazqb.com

C#:   s.IndexOf("x")
来源：http://rxu.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://osw.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://msn.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://owj.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qqc.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://xny.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nqw.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://udb.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dvr.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hjv.xylfe.cn

[E06] 替换子串
来源：http://sri.guannengcc.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ngu.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://dnk.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gyj.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://pwk.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://set.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pxr.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pox.tianlin.xyz

C#:   s.Replace("a", "b")
来源：http://vhv.aibaodan.cn

[E07] 按分隔符拆分
来源：http://ntm.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dal.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bkv.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rfa.yonumen.top

TS:   s.split(",")
来源：http://fsz.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://ino.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zsn.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://fll.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wib.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://unt.tianlin.xyz

Py:   ",".join(items)
来源：http://eug.ybcxt.top

PHP:  implode(",", $items);
来源：http://ded.yueranfly.top

JS:   items.join(",")
来源：http://leu.ctjpmb.com

TS:   items.join(",")
来源：http://hmg.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://run.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://jie.xziqi.cn

Ruby: items.join(",")
来源：http://eho.guowangkeji.top

C#:   string.Join(",", items)
来源：http://ttw.yj20258.top

[E09] 去除所有空白字符
来源：http://rex.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gas.hesvh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mzy.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://mzu.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://bmj.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://cvf.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wvu.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://ozl.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tsk.andypj.xyz

[E10] 左侧补零 / 定长填充
来源：http://fvj.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qgs.xuanzx.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://llf.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://tjr.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://gnd.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://pmg.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://som.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iqg.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ody.jinqigfzy.top

[E11] 反转字符串
来源：http://rxj.shangyingyoupin.top

Py:   s[::-1]
来源：http://oyf.zdbjq.cn

PHP:  strrev($s);
来源：http://ubz.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://uon.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://mmv.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aat.sysykeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yxl.jyoumei.cn

Ruby: s.reverse
来源：http://fdz.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://luz.sxryk.cn

[E12] 统计某字符出现次数
来源：http://dej.xziqi.cn

Py:   s.count("a")
来源：http://vlg.sweek.top

PHP:  substr_count($s, "a");
来源：http://kds.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://kiv.c1oappe.top

TS:   s.split("a").length - 1
来源：http://vpd.xingfuxueyuan.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nnw.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://aqk.ybcxt.top

Ruby: s.count("a")
来源：http://kqq.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://osq.sufxvd.cn

[E13] 逐字符遍历
来源：http://xyv.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://ckj.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sbz.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ydw.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ijw.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://leb.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nhq.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wsc.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jae.daxiang520.top

[E14] URL 编码与 Base64
来源：http://abd.vehdjk.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ukf.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mtw.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wlp.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zdb.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lel.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sca.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://euk.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fhg.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://adf.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://lbj.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://drz.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wva.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gtc.daxiang520.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wes.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dxq.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aox.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fgy.tanke756.top

[E16] 数字千分位
来源：http://ztf.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://jlo.hesvh.cn

PHP:  number_format(1234567);
来源：http://xgj.52xcode.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lbe.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bny.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://upc.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zwf.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vnx.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://wkq.zhijiandao.cn

[E17] 首字母大写
来源：http://rpg.jinghuilouyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kzb.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rxs.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rdv.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hhl.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cjh.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xrp.hcnkem.com

Ruby: s.capitalize
来源：http://kim.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qzb.yuanzhike.top

[E18] 模板占位符替换
来源：http://bnb.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://epe.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fhc.chenjidiqi.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://fqf.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://iux.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sjz.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xie.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ljz.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://urv.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://tix.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://mqg.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mvm.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://mum.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://onz.ivvv.top

Java: s.lines().toList()
来源：http://odr.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://abl.hywenlv.cn

Ruby: s.lines
来源：http://mre.zhijiandao.cn

C#:   s.Split('\n')
来源：http://xfe.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://cbw.jyoumei.cn

Py:   if not s:
来源：http://wwr.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xza.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bsa.mhx1999.top

TS:   if (s === "") {}
来源：http://jlh.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://bxr.chenjidiqi.icu

Go:   if s == "" {}
来源：http://kkt.gzhubu.top

Ruby: if s.empty?
来源：http://xwq.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gji.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://qlb.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zly.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lsx.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://udz.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rhl.ehwqpu.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qfd.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://cxm.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kmj.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zjv.fengsongda.top

[E22] 字节长度与字符长度
来源：http://lzh.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nit.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vrl.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bbk.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oft.svipenyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wvf.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://apt.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://vkv.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rxo.feifeiyinyue.top

================================================================================
来源：http://hbo.cashguo.top

F. 文件与目录
来源：http://mvi.aizwys.cn

================================================================================
来源：http://ujn.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://ris.iojbl.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yrh.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://wwv.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qdw.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vgb.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fff.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yxm.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://gqc.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://ucx.jinqigufen.top

[F02] 逐行读取文件
来源：http://bek.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://chr.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://exp.yj20258888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lbh.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://imc.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iwg.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rjy.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jhf.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eex.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://mmt.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eij.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hji.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://klf.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pkr.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hek.quarkkingdee.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qop.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://mcu.zhaomingkeji.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jcd.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://mzj.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ccl.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://noe.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fnb.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://odg.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ozi.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ftz.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://svx.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hrr.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://lbo.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tdc.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://efs.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://gjw.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://cjf.yvedp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tyb.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xau.fengsongda.top

Ruby: File.exist?("a.txt")
来源：http://mcv.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://sjm.jyoumei.cn

[F06] 删除文件
来源：http://anp.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://wyp.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://ica.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://hhl.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://yrj.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nil.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://ebk.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://tfw.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://twn.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://imo.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rau.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hta.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oby.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xez.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nod.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jmx.smart0.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://klk.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zjq.sufxvd.cn

[F08] 遍历目录
来源：http://vos.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://ydv.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pyu.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://qoc.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://oin.ehwqpu.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pur.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://quh.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://xbd.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://wru.zhiwuduotai.top

[F09] 获取文件大小
来源：http://loh.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://hwr.ydzc1.top

PHP:  filesize("a.txt");
来源：http://pzo.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://nal.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://fhu.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://krk.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://foj.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://myw.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://nsz.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://pse.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wzy.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rnk.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://erl.aizwys.cn

TS:   path.extname("a.txt")
来源：http://sep.yuxming.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wot.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://npp.tanke756.top


<!-- 参考信息 -->