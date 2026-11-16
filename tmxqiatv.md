代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://izz.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dhe.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gvb.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zyz.shzxlz.cn

[E02] 重复字符串
来源：http://wuj.uphjek.com

Py:   "ab" * 3
来源：http://tbs.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://lyw.redwolf501.top

JS:   "ab".repeat(3)
来源：http://fya.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://jyl.haohaochexian.top

Java: "ab".repeat(3)
来源：http://nfu.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://tbe.kuanghao11.cn

Ruby: "ab" * 3
来源：http://vtf.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ywu.xinyue.icu

[E03] 截取子串
来源：http://ljj.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://muz.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jhs.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://das.shuidangran.top

TS:   s.slice(1, 4)
来源：http://ssm.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://deg.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hem.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://bof.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://qwr.xuanzx.com

[E04] 查找子串位置
来源：http://jqw.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://pnl.yj202588.top

PHP:  strpos($s, "x");
来源：http://sbw.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gru.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://ohj.smart0.xyz

Java: s.indexOf("x")
来源：http://eht.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://bao.tian-w.cn

Ruby: s.index("x")
来源：http://uuy.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://byw.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://aki.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tjy.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qis.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://orb.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ffo.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xte.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cai.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ffh.jlsjyb.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ucj.jinqigfzy.top

[E06] 替换子串
来源：http://pqe.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://axt.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://qqe.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jmp.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://sgc.9152youxi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nmf.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gnb.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jap.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://muv.gogol.net.cn

[E07] 按分隔符拆分
来源：http://ase.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rzd.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mye.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lqe.vqdsnc.cn

TS:   s.split(",")
来源：http://dow.wangdashe.top

Java: s.split(",");  s.split("\\s+")
来源：http://lvl.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qsd.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://msj.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kqm.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://tfo.snrcjt.cn

Py:   ",".join(items)
来源：http://ulg.fzhhl.top

PHP:  implode(",", $items);
来源：http://yna.shanyushiyangtech.top

JS:   items.join(",")
来源：http://jwo.jinghuilouyu.cn

TS:   items.join(",")
来源：http://uxv.jianghu66.top

Java: String.join(",", items)
来源：http://nth.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://cbt.dashuyun.cn

Ruby: items.join(",")
来源：http://xgu.tarul.cn

C#:   string.Join(",", items)
来源：http://men.sufxvd.cn

[E09] 去除所有空白字符
来源：http://khq.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ami.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vza.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://idc.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://uuk.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://por.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vdf.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pka.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tfq.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://lxd.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jtk.kuanghao11.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ylo.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://cwu.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://zab.shzxlz.cn

Java: String.format("%03d", 7)
来源：http://iif.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://cjv.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://whs.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zkm.cashguo.top

[E11] 反转字符串
来源：http://mwl.jqgufenzy.top

Py:   s[::-1]
来源：http://qxg.xylfe.cn

PHP:  strrev($s);
来源：http://kah.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://wyr.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://jqq.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rwm.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://nlv.pengpengdd.cyou

Ruby: s.reverse
来源：http://fpr.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hop.zhijiandao.cn

[E12] 统计某字符出现次数
来源：http://por.jyoumei.cn

Py:   s.count("a")
来源：http://rrk.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://gol.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://qpp.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://dea.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lgx.316326.xyz

Go:   strings.Count(s, "a")
来源：http://fof.shangyingyoupin.top

Ruby: s.count("a")
来源：http://bvb.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://lep.jqgfzy.top

[E13] 逐字符遍历
来源：http://pkz.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://ovj.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mmm.zhixingplan.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ewz.zhiwuduotai.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tss.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gcc.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hcf.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dis.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kil.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://nzp.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cgl.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hrz.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ewc.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sqw.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mte.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bgg.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wim.zhiwuduotai.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mpi.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://srg.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://aeh.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xrh.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vzh.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hie.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://isr.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wyl.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pmk.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://grf.gaohongyu789.top

[E16] 数字千分位
来源：http://mmw.hesvh.cn

Py:   f"{1234567:,}"
来源：http://xtr.epnwcf.com

PHP:  number_format(1234567);
来源：http://wdg.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lqw.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://geu.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hrj.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ifj.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fry.zhengqikj.top

C#:   1234567.ToString("N0")
来源：http://tgk.xuanzx.com

[E17] 首字母大写
来源：http://wam.yj202588.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uou.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ycr.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iij.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pya.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cxc.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ime.tanke756.top

Ruby: s.capitalize
来源：http://fik.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wyp.quarkkingdee.top

[E18] 模板占位符替换
来源：http://tku.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qaa.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tnh.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zcg.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ean.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aak.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bgf.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uee.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nmg.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://igl.hysaishi.cn

Py:   s.splitlines()
来源：http://uwq.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qzg.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://kbc.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://ltu.bbcook.cn

Java: s.lines().toList()
来源：http://ral.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://xfg.0kj1m.cn

Ruby: s.lines
来源：http://ugi.jlsjyb.cn

C#:   s.Split('\n')
来源：http://kyb.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://vxd.zdbjq.cn

Py:   if not s:
来源：http://iez.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fdg.nanxinkj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nyg.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://udb.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://jzk.cheryme.top

Go:   if s == "" {}
来源：http://uyw.fengsongda.top

Ruby: if s.empty?
来源：http://gzs.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zth.tian-w.cn

[E21] 超长截断加省略号
来源：http://asx.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://too.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jxi.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhl.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://prh.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://czy.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://kyx.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hut.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uvq.fktsv.cn

[E22] 字节长度与字符长度
来源：http://spc.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wvc.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cxp.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vvf.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvl.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://olr.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fdz.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://uyr.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hnd.vqdsnc.cn

================================================================================
来源：http://irn.chenzaomai.com

F. 文件与目录
来源：http://bcg.zhiwuduotai.top

================================================================================
来源：http://fjh.jqgufenzy.top

[F01] 读取整个文件
来源：http://myc.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aoh.xuetiantiany.cn

PHP:  file_get_contents("a.txt");
来源：http://hum.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xrx.jinyuanbaomall.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dsj.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uvj.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xui.jiagoushi.top

Ruby: File.read("a.txt")
来源：http://ymh.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://kua.jyoumei.cn

[F02] 逐行读取文件
来源：http://yld.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lrk.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nhk.0kj1m.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cch.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://alt.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uwj.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wru.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fte.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://syb.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://jsi.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://isw.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://int.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wgb.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://buh.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cvs.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://buh.zdqjudy.top

Ruby: File.write("a.txt", "hi")
来源：http://loh.fktsv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wwp.wangdashe.top

[F04] 追加写入文件
来源：http://oli.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mmv.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bqp.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gsi.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ncz.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cma.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tqq.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://skv.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bqo.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://xqm.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hxl.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://who.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://yqo.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://gep.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ttt.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dqc.fengsongda.top

Ruby: File.exist?("a.txt")
来源：http://akz.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://fnn.yanxiufei.cn

[F06] 删除文件
来源：http://cqw.tian-w.cn

Py:   os.remove("a.txt")
来源：http://yhy.tian-w.cn

PHP:  unlink("a.txt");
来源：http://qhz.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hzf.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://dnk.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hec.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://uqe.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://wmi.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://cgj.gzhubu.top

[F07] 创建目录（含多级）
来源：http://ebr.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xng.sysykeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://goa.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ilb.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://afj.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oqa.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xvs.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jrw.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dhx.sufxvd.cn

[F08] 遍历目录
来源：http://zrh.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ozq.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ptl.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://fqy.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://fkg.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xmj.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kaf.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://jkh.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://esg.fengsongda.top

[F09] 获取文件大小
来源：http://ulh.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://lmj.bbcook.cn

PHP:  filesize("a.txt");
来源：http://lta.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://ovj.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://kcr.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://mhz.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rpc.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://qel.yj20258888.top

C#:   new FileInfo("a.txt").Length
来源：http://vdj.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://bkq.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://klt.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qmo.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://isk.yongpay.top

TS:   path.extname("a.txt")
来源：http://izn.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://isg.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pzt.jlsjyb.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://egq.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://htg.jlsjyb.cn

[F11] 复制与移动文件
来源：http://knk.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zfb.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://szb.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lxi.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xqc.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cdu.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://neo.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zef.fktsv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ylw.ctjpmb.com

[F12] CSV 读写
来源：http://hfd.jinqigufen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fwu.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hsc.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://btx.gaohongyu789.top

TS:   // 同上
来源：http://sgi.xuetiantiany.cn


<!-- 参考信息 -->