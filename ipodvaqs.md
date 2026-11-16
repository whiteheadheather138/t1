代发 wailian999

Java: String.join(", ", list)
来源：http://pku.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://xly.yfazqb.com

Ruby: arr.join(", ")
来源：http://hoj.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://oux.andypj.xyz

================================================================================
来源：http://gym.mhx1999.top

E. 字符串处理
来源：http://qla.zycfv.cn

================================================================================
来源：http://azf.fktsv.cn

[E01] 拼接字符串
来源：http://yyh.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xtt.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ypm.aizwys.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://okv.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qvb.yj20258.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xhz.vqdsnc.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ldx.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kzh.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wba.yongpay.top

[E02] 重复字符串
来源：http://ngy.bjfxy.top

Py:   "ab" * 3
来源：http://nwu.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://dsi.yj202588.top

JS:   "ab".repeat(3)
来源：http://yav.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://ebf.zhixingplan.top

Java: "ab".repeat(3)
来源：http://btg.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://bwc.jqgfzy.top

Ruby: "ab" * 3
来源：http://cac.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tec.jianghu66.top

[E03] 截取子串
来源：http://pge.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aid.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wih.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vdv.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://rtk.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://jbx.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://urc.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://ykk.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://yzj.ydzc1.top

[E04] 查找子串位置
来源：http://brj.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://rlt.c1oappe.top

PHP:  strpos($s, "x");
来源：http://vbo.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cqb.hcnkem.com

TS:   s.indexOf("x")
来源：http://iri.gaohongyu789.top

Java: s.indexOf("x")
来源：http://lkz.zhoulong.xyz

Go:   strings.Index(s, "x")
来源：http://gdj.hnqzz.top

Ruby: s.index("x")
来源：http://fqh.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://rcc.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ijv.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ybe.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://slw.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nvo.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://anm.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zrk.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://off.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gdw.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fak.zhiwuduotai.top

[E06] 替换子串
来源：http://uup.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yop.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://vme.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hut.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://lca.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://giv.yuxming.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pmm.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mfs.yj20258.top

C#:   s.Replace("a", "b")
来源：http://glr.ivvv.top

[E07] 按分隔符拆分
来源：http://rqs.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vei.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kjb.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ckc.9152youxi.cn

TS:   s.split(",")
来源：http://wiw.jiagoushi.top

Java: s.split(",");  s.split("\\s+")
来源：http://wqx.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qen.yj20258.top

Ruby: s.split(",");  s.split
来源：http://kla.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://agi.shuidangran.top

[E08] 数组按分隔符合并
来源：http://xym.gzhubu.top

Py:   ",".join(items)
来源：http://fbe.ctjpmb.com

PHP:  implode(",", $items);
来源：http://fux.tianlin.xyz

JS:   items.join(",")
来源：http://llh.316326.xyz

TS:   items.join(",")
来源：http://pdv.sjlbkw.cn

Java: String.join(",", items)
来源：http://phv.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://sxk.feifeiyinyue.top

Ruby: items.join(",")
来源：http://jxm.wangdashe.top

C#:   string.Join(",", items)
来源：http://avg.jianghu66.top

[E09] 去除所有空白字符
来源：http://vby.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zzw.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tfa.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://zoq.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://nel.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://wef.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://wdr.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://muj.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://foh.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://tlb.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hvv.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://swr.sufxvd.cn

JS:   "7".padStart(3, "0")
来源：http://vnt.daria6918.cn

TS:   "7".padStart(3, "0")
来源：http://mfx.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://pov.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://lsc.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xfn.jinyuanbaomall.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eyu.jinqigufen.top

[E11] 反转字符串
来源：http://rod.yongpay.top

Py:   s[::-1]
来源：http://drl.fzhhl.top

PHP:  strrev($s);
来源：http://bnb.tanke756.top

JS:   [...s].reverse().join("")
来源：http://eit.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://qyz.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dkp.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tvd.haohaochexian.top

Ruby: s.reverse
来源：http://uiy.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://opa.daria6918.cn

[E12] 统计某字符出现次数
来源：http://ibm.fengsongda.top

Py:   s.count("a")
来源：http://sdh.sxryk.cn

PHP:  substr_count($s, "a");
来源：http://rju.gzhubu.top

JS:   s.split("a").length - 1
来源：http://mdc.316326.xyz

TS:   s.split("a").length - 1
来源：http://ziz.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gyh.ctjpmb.com

Go:   strings.Count(s, "a")
来源：http://qbh.hnxiangtu.top

Ruby: s.count("a")
来源：http://tis.guowangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://cxb.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://jow.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://wvh.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dlw.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nbe.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://khw.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kxe.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uzk.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://hai.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://psz.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://nuf.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zwe.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tuh.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dkr.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ijf.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hnb.chenzaomai.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tzb.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rto.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kgf.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://pwb.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kys.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jgz.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jhh.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sbt.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gil.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rsu.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://arr.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pqg.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://nad.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://mbn.zhiwuduotai.top

PHP:  number_format(1234567);
来源：http://cfm.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qsw.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zdj.yonumen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kfs.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jiu.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fny.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://rlu.fanxiaobao.xyz

[E17] 首字母大写
来源：http://csv.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://erc.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://max.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sef.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ykk.jinghuilouyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nut.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pry.wangdashe.top

Ruby: s.capitalize
来源：http://win.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jsk.havefunace.top

[E18] 模板占位符替换
来源：http://fzp.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://due.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://flj.zhengqikj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sxj.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tcj.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ywv.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vnh.shzxlz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jox.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ccq.zycfv.cn

[E19] 多行文本按行拆分
来源：http://gae.svipenyu.cn

Py:   s.splitlines()
来源：http://ixy.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qhx.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://ehj.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://nuh.dianchejie.cn

Java: s.lines().toList()
来源：http://bpw.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://oot.epnwcf.com

Ruby: s.lines
来源：http://zsc.tarul.cn

C#:   s.Split('\n')
来源：http://lay.uphjek.com

[E20] 判断字符串是否为空
来源：http://qtd.gotoacloud.top

Py:   if not s:
来源：http://srk.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dsb.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yqo.iojbl.cn

TS:   if (s === "") {}
来源：http://jmr.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://rnc.bbcook.cn

Go:   if s == "" {}
来源：http://pvf.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://acx.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://msm.yuxming.cn

[E21] 超长截断加省略号
来源：http://who.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zsi.wangshuangyany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wci.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lok.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsr.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cnx.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://drd.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hin.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ihc.svipenyu.cn

[E22] 字节长度与字符长度
来源：http://cpy.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gqg.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jrv.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uwz.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eib.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ftu.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wbt.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://brk.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ieh.xziqi.cn

================================================================================
来源：http://uus.chenzaomai.com

F. 文件与目录
来源：http://ygc.daxiang520.top

================================================================================
来源：http://kuh.jiagoushi.top

[F01] 读取整个文件
来源：http://zsf.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xpl.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://glr.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gww.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jwc.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xmx.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yed.meibo888.top

Ruby: File.read("a.txt")
来源：http://qfz.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://xch.redwolf501.top

[F02] 逐行读取文件
来源：http://krw.vehdjk.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bys.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xyn.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://koj.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kga.zhaomingkeji.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uaf.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wow.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jwg.jinqigufen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tsi.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://gel.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jzw.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://usy.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xbh.yj20258888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jhz.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://elw.zhengqikj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rco.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://ujg.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jin.quarkkingdee.top

[F04] 追加写入文件
来源：http://dxi.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lcw.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wdw.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cve.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dqa.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tov.ydjk.org.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hnn.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xzp.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lch.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://nku.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://enh.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://jua.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://leq.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://ojb.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zpa.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tgg.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://clv.tanke756.top

C#:   File.Exists("a.txt")
来源：http://hyv.tian-w.cn

[F06] 删除文件
来源：http://eeg.hcnkem.com

Py:   os.remove("a.txt")
来源：http://ykr.fktsv.cn

PHP:  unlink("a.txt");
来源：http://lqx.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://siy.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hxx.yfazqb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xop.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://ayr.birdmap.top

Ruby: File.delete("a.txt")
来源：http://xxb.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://pws.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://puy.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fth.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://omq.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jkg.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mix.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://alm.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://czq.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aen.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kap.aibaodan.cn

[F08] 遍历目录
来源：http://lpu.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lmd.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ohs.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://jef.yueranfly.top

TS:   fs.readdirSync("dir")
来源：http://gwn.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zod.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wpq.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://szr.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://unc.yuanzhike.top

[F09] 获取文件大小
来源：http://wjt.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://suw.tanke756.top

PHP:  filesize("a.txt");
来源：http://loo.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://umn.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://ysr.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://jdv.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hzx.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://qhx.316326.xyz

C#:   new FileInfo("a.txt").Length
来源：http://mqm.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://skt.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://opr.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xkl.yj20258.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xwk.aizwys.cn

TS:   path.extname("a.txt")
来源：http://ldo.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wqj.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lqq.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://inv.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vqf.yuxming.cn

[F11] 复制与移动文件
来源：http://cxh.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://htb.xinyue.icu


<!-- 参考信息 -->