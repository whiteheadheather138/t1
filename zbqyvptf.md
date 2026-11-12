代发 wailian999

================================================================================
来源：http://gbu.ywan-chungtsiang.top

E. 字符串处理
来源：http://caw.chenjidiqi.icu

================================================================================
来源：http://jiz.tanke756.top

[E01] 拼接字符串
来源：http://ava.ydzc1.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://asc.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wff.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rdo.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://juu.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vly.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wqi.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cdr.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nvr.fzhhl.top

[E02] 重复字符串
来源：http://svk.dashuyun.cn

Py:   "ab" * 3
来源：http://xru.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://dgp.sysykeji.top

JS:   "ab".repeat(3)
来源：http://dlv.cashguo.top

TS:   "ab".repeat(3)
来源：http://hdl.chenzaomai.com

Java: "ab".repeat(3)
来源：http://les.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://eeo.zhongyouzk.top

Ruby: "ab" * 3
来源：http://efq.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gtj.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://tfd.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dec.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cfu.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yap.mhx1999.top

TS:   s.slice(1, 4)
来源：http://qpk.yvedp.cn

Java: s.substring(1, 4)
来源：http://rqu.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tye.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://fru.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://ocu.andypj.xyz

[E04] 查找子串位置
来源：http://jzh.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://svz.sxryk.cn

PHP:  strpos($s, "x");
来源：http://ser.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gcs.c1oappe.top

TS:   s.indexOf("x")
来源：http://dfo.kuanghao11.cn

Java: s.indexOf("x")
来源：http://ofo.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://har.fktsv.cn

Ruby: s.index("x")
来源：http://pje.yj202588.top

C#:   s.IndexOf("x")
来源：http://epo.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://tom.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qfp.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://czu.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tik.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hwx.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://acu.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lsx.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qws.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nvb.ydzc1.top

[E06] 替换子串
来源：http://shj.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aam.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://nmr.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jex.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://mys.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xdw.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wfj.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://edt.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://tbs.tarul.cn

[E07] 按分隔符拆分
来源：http://wgb.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://abv.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pjo.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://dge.havefunace.top

TS:   s.split(",")
来源：http://epl.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kor.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qdf.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://nsh.sweek.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tsb.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://psx.fengsongda.top

Py:   ",".join(items)
来源：http://rds.shzxlz.cn

PHP:  implode(",", $items);
来源：http://zge.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://pej.hcnkem.com

TS:   items.join(",")
来源：http://aiw.bjfxy.top

Java: String.join(",", items)
来源：http://gtw.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://zkk.yvedp.cn

Ruby: items.join(",")
来源：http://xxs.zdbjq.cn

C#:   string.Join(",", items)
来源：http://sbw.ivvv.top

[E09] 去除所有空白字符
来源：http://xmi.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eno.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://srk.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://lrv.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://dge.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://tyw.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gxv.nwbrower.top

Ruby: s.gsub(/\s+/, "")
来源：http://bit.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gjg.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://vjs.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mbx.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://puo.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://thp.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://yob.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://vmq.havefunace.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://eml.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dnc.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uxt.aizwys.cn

[E11] 反转字符串
来源：http://snc.quarkkingdee.top

Py:   s[::-1]
来源：http://xfx.feifeiyinyue.top

PHP:  strrev($s);
来源：http://uij.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://xne.yj202588.top

TS:   [...s].reverse().join("")
来源：http://fcc.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xls.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ika.tarul.cn

Ruby: s.reverse
来源：http://xfq.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://afb.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://hze.xuetiantiany.cn

Py:   s.count("a")
来源：http://aza.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://qnf.bjfxy.top

JS:   s.split("a").length - 1
来源：http://tox.epnwcf.com

TS:   s.split("a").length - 1
来源：http://tep.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nxt.aibaodan.cn

Go:   strings.Count(s, "a")
来源：http://cmu.52xcode.cn

Ruby: s.count("a")
来源：http://qcb.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://gjo.tian-w.cn

[E13] 逐字符遍历
来源：http://zbg.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://yfx.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wam.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lao.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ueg.jinqigfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aws.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://awx.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lcc.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dgy.birdmap.top

[E14] URL 编码与 Base64
来源：http://inv.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xov.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ria.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ehq.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qzs.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://muy.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://osb.wangdashe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pcf.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://orp.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://nze.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lfj.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yss.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qru.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oif.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vsh.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rks.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eev.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kug.jqgufenzy.top

[E16] 数字千分位
来源：http://uwv.cucudq.cn

Py:   f"{1234567:,}"
来源：http://aya.nanxinkj.top

PHP:  number_format(1234567);
来源：http://drg.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sdj.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wpg.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bpb.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yxk.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mto.bjfxy.top

C#:   1234567.ToString("N0")
来源：http://tvq.xinyue.icu

[E17] 首字母大写
来源：http://ksp.ydjk.org.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vru.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rtt.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xpz.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dts.9152youxi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://btc.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fzi.tanke756.top

Ruby: s.capitalize
来源：http://cnu.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yyo.jyoumei.cn

[E18] 模板占位符替换
来源：http://emg.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yzp.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kcn.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ppz.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lgp.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://abo.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gaw.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ahd.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ccv.feifeiyinyue.top

[E19] 多行文本按行拆分
来源：http://eho.haohaochexian.top

Py:   s.splitlines()
来源：http://slc.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jfo.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://cnz.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://jjv.ppjwa.cn

Java: s.lines().toList()
来源：http://xcz.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://qfp.hnxiangtu.top

Ruby: s.lines
来源：http://sol.c1oappe.top

C#:   s.Split('\n')
来源：http://sbn.fengsongda.top

[E20] 判断字符串是否为空
来源：http://duf.shanyushiyangtech.top

Py:   if not s:
来源：http://aif.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ghk.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://viu.jqgufenzy.top

TS:   if (s === "") {}
来源：http://yhs.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://ssx.zhoulong.xyz

Go:   if s == "" {}
来源：http://ywq.snrcjt.cn

Ruby: if s.empty?
来源：http://zkk.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://spy.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://lys.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ory.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pao.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wvl.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ojh.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://goj.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ozn.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gjq.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://odq.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://ncd.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xsn.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hop.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lhb.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ykc.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vza.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jdp.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://yir.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kbd.shanyushiyangkeji.top

================================================================================
来源：http://kdl.jqgufenzy.top

F. 文件与目录
来源：http://scc.xingfuxueyuan.xyz

================================================================================
来源：http://uup.hcnkem.com

[F01] 读取整个文件
来源：http://kru.iojbl.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lon.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://qvw.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ckq.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xop.tian-w.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vmx.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bkr.wangdashe.top

Ruby: File.read("a.txt")
来源：http://mzd.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://php.sufxvd.cn

[F02] 逐行读取文件
来源：http://lee.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tzo.gaohongyu789.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fmk.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zbx.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ayd.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qgu.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://siv.sysykeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cil.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qxt.tarul.cn

[F03] 写入文件（覆盖）
来源：http://unc.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mvr.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hlc.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qzp.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kdz.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nca.sweek.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uab.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://lto.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iru.sysykeji.top

[F04] 追加写入文件
来源：http://jmw.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://skr.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rzc.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gew.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tij.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gdl.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qyq.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tep.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cxp.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://ynd.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wpn.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://jyw.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://eul.shzxlz.cn

TS:   fs.existsSync("a.txt")
来源：http://nlq.tianlin.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://qnj.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vhq.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://hag.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://ofu.yj20258888.top

[F06] 删除文件
来源：http://awk.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://axx.yuxming.cn

PHP:  unlink("a.txt");
来源：http://cif.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://wtm.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://gtr.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jtq.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://rek.fanxiaobao.xyz

Ruby: File.delete("a.txt")
来源：http://pil.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://pvl.yonumen.top

[F07] 创建目录（含多级）
来源：http://jih.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xob.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dfs.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gih.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mml.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uln.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jhq.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cje.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ign.fehbvm.com

[F08] 遍历目录
来源：http://hqh.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rnf.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wxt.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://qpv.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://mdn.jlsjyb.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cgy.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ede.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://jas.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://qyw.ppjwa.cn

[F09] 获取文件大小
来源：http://utp.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://oqw.bbcook.cn

PHP:  filesize("a.txt");
来源：http://ezs.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://ovc.yonumen.top

TS:   fs.statSync("a.txt").size
来源：http://yzr.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://gfn.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nhy.cucudq.cn

Ruby: File.size("a.txt")
来源：http://kuq.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://ntr.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://dnm.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ucx.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iqd.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lem.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://yrq.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pkk.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dtk.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fhd.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nir.ehwqpu.com

[F11] 复制与移动文件
来源：http://lim.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ubg.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jvg.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aqv.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jyd.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hhv.nwbrower.top


<!-- 参考信息 -->