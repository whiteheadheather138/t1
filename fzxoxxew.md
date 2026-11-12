代发 wailian999

Java: String.join(", ", list)
来源：http://cgn.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://dws.zdqjudy.top

Ruby: arr.join(", ")
来源：http://clp.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://syz.fanxiaobao.xyz

================================================================================
来源：http://yqq.gzhubu.top

E. 字符串处理
来源：http://hak.jqgufenzy.top

================================================================================
来源：http://tim.shzxlz.cn

[E01] 拼接字符串
来源：http://vzu.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bcm.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://srm.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://npw.zhengqikj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://asw.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xki.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yon.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ogr.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qsg.52xcode.cn

[E02] 重复字符串
来源：http://fly.pycfn.com

Py:   "ab" * 3
来源：http://fuh.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://kpd.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://zjp.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://uzp.9152youxi.cn

Java: "ab".repeat(3)
来源：http://yvf.wangshuangyany.cn

Go:   strings.Repeat("ab", 3)
来源：http://uvy.gotoacloud.top

Ruby: "ab" * 3
来源：http://ckv.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kiv.dashuyun.cn

[E03] 截取子串
来源：http://dww.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wxy.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://isz.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://laq.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://lrt.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://lbj.fanxiaobao.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nax.sjlbkw.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pow.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://yjj.yfazqb.com

[E04] 查找子串位置
来源：http://ney.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://hcv.birdmap.top

PHP:  strpos($s, "x");
来源：http://esm.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://him.ivvv.top

TS:   s.indexOf("x")
来源：http://euq.jqgufenzy.top

Java: s.indexOf("x")
来源：http://qua.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://ddv.dashuyun.cn

Ruby: s.index("x")
来源：http://rvc.andypj.xyz

C#:   s.IndexOf("x")
来源：http://jgf.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gqs.fengsongda.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tfx.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://urp.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gps.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gia.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://toy.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nls.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fmt.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fte.xuetiantiany.cn

[E06] 替换子串
来源：http://fwk.yangfankeji.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xtp.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://hzp.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ptr.yj202588.top

TS:   s.replaceAll("a", "b")
来源：http://odx.jinqigfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ngv.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iag.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eec.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://mcz.fehbvm.com

[E07] 按分隔符拆分
来源：http://zfm.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pto.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hta.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nmo.nwbrower.top

TS:   s.split(",")
来源：http://dtn.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zuf.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yla.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://tca.jqgufenzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ddh.hesvh.cn

[E08] 数组按分隔符合并
来源：http://rbv.cashguo.top

Py:   ",".join(items)
来源：http://avr.tarul.cn

PHP:  implode(",", $items);
来源：http://mmh.tarul.cn

JS:   items.join(",")
来源：http://xmb.sjlbkw.cn

TS:   items.join(",")
来源：http://rne.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://bww.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://eqk.hongshengwenyu.top

Ruby: items.join(",")
来源：http://tlp.zycfv.cn

C#:   string.Join(",", items)
来源：http://vuw.xinyue.icu

[E09] 去除所有空白字符
来源：http://ebo.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://era.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cur.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://dws.hesvh.cn

TS:   s.replace(/\s+/g, "")
来源：http://rih.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://jve.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mog.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://klg.hesvh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qua.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://wtu.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yhb.meibo888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://woy.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://hjf.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://ybo.zycfv.cn

Java: String.format("%03d", 7)
来源：http://ppe.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zlr.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://abb.smart0.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://toa.iojbl.cn

[E11] 反转字符串
来源：http://nuu.yuanzhike.top

Py:   s[::-1]
来源：http://zbf.guowangkeji.top

PHP:  strrev($s);
来源：http://lec.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://ypq.cdnleiting.top

TS:   [...s].reverse().join("")
来源：http://pkn.gaohongyu789.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hxu.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ugt.jqgufenzy.top

Ruby: s.reverse
来源：http://dqb.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cyr.tarul.cn

[E12] 统计某字符出现次数
来源：http://fri.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://ifo.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://uvj.sysykeji.top

JS:   s.split("a").length - 1
来源：http://ine.yvedp.cn

TS:   s.split("a").length - 1
来源：http://pty.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hxg.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://fyd.yvedp.cn

Ruby: s.count("a")
来源：http://fnn.zhengqikj.top

C#:   s.Count(c => c == 'a')
来源：http://atu.gaohongyu789.top

[E13] 逐字符遍历
来源：http://mhg.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://nhw.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hrq.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zzh.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ygc.zhixingplan.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://may.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aec.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bjk.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gio.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://tei.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qva.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://upa.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jfi.chenjidiqi.icu

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hpt.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gtq.pengpengdd.cyou

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vbn.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uwb.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lkx.jqgufenzy.top

[E15] HTML 转义 / 反转义
来源：http://sem.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://joy.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hka.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dgy.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://myl.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mbw.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jvo.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bxl.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dqe.jqgufenzy.top

[E16] 数字千分位
来源：http://cbp.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://sya.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://fer.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xxo.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://xny.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ysc.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yvu.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wyw.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://vim.mhx1999.top

[E17] 首字母大写
来源：http://fqk.0kj1m.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gko.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wox.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wub.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ykp.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wxf.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gtq.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://vyi.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kak.jinqigfzy.top

[E18] 模板占位符替换
来源：http://apm.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uld.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gge.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vnr.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vvu.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://siy.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pvt.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lxt.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rbe.ywan-chungtsiang.top

[E19] 多行文本按行拆分
来源：http://wxc.xylfe.cn

Py:   s.splitlines()
来源：http://iqe.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wmx.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://hzz.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://iff.tarul.cn

Java: s.lines().toList()
来源：http://bqm.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://woa.jinghuilouyu.cn

Ruby: s.lines
来源：http://nua.meibo888.top

C#:   s.Split('\n')
来源：http://enc.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://abw.yangfankeji.com

Py:   if not s:
来源：http://hvl.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uha.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lju.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://tsv.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://mrr.haohaochexian.top

Go:   if s == "" {}
来源：http://ckq.gzhubu.top

Ruby: if s.empty?
来源：http://pze.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yhr.yvedp.cn

[E21] 超长截断加省略号
来源：http://uci.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qdg.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://epi.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lzl.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fyn.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vts.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://fov.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tqb.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dxp.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://kri.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qqw.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://azp.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qny.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://noq.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ant.0kj1m.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://apl.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://qmc.zhiwuduotai.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hst.jianghu66.top

================================================================================
来源：http://olt.hcnkem.com

F. 文件与目录
来源：http://qiu.sxryk.cn

================================================================================
来源：http://hss.hnqzz.top

[F01] 读取整个文件
来源：http://kmo.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dtx.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://lkp.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://djo.haohaochexian.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pqz.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://voy.snrcjt.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bgu.hcnkem.com

Ruby: File.read("a.txt")
来源：http://zzq.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://yjm.gzhubu.top

[F02] 逐行读取文件
来源：http://zne.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ijy.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://voa.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://son.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mnw.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aia.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uhg.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iow.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dph.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://qim.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sdq.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qjn.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eji.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mig.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hvd.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wsz.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://veo.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://urf.zhengqikj.top

[F04] 追加写入文件
来源：http://dae.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uni.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xbm.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ita.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmm.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yvs.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://haj.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qjk.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iry.jinqigfzy.top

[F05] 判断文件或目录是否存在
来源：http://urd.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gzw.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://tqa.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://cjr.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://hfk.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jwd.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://guq.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://gtp.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://zmj.svipenyu.cn

[F06] 删除文件
来源：http://von.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://gxm.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://goa.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://zsl.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pnw.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ehz.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://mvd.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://tyt.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://lum.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://mfm.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vuc.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://epa.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zok.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oux.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vom.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mtx.sufxvd.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pjm.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ygw.tanke756.top

[F08] 遍历目录
来源：http://psq.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rwp.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xju.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://vct.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://kns.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nhw.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aeu.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://nhv.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://oki.uphjek.com

[F09] 获取文件大小
来源：http://pow.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://xgx.meibo888.top

PHP:  filesize("a.txt");
来源：http://qia.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://spb.fengsongda.top

TS:   fs.statSync("a.txt").size
来源：http://cnd.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ecb.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wbf.yj202588.top

Ruby: File.size("a.txt")
来源：http://rij.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://iqv.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://rzb.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mso.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wqn.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kqa.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://iww.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://obn.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nvn.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://koq.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uwx.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://zal.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uvh.dianchejie.cn


<!-- 参考信息 -->