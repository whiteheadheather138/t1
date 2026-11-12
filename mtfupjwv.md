代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ode.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://foj.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oev.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tdv.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bau.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kyb.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vkp.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lzr.9152youxi.cn

[E02] 重复字符串
来源：http://wsw.xylfe.cn

Py:   "ab" * 3
来源：http://bag.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://ngu.yuxming.cn

JS:   "ab".repeat(3)
来源：http://gnt.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://apx.tianlin.xyz

Java: "ab".repeat(3)
来源：http://uvr.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://qba.vehdjk.com

Ruby: "ab" * 3
来源：http://xhb.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ang.ehwqpu.com

[E03] 截取子串
来源：http://zfl.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kxa.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://efm.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ntd.zycfv.cn

TS:   s.slice(1, 4)
来源：http://tje.zhixingplan.top

Java: s.substring(1, 4)
来源：http://ooe.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lph.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fwl.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://gnh.havefunace.top

[E04] 查找子串位置
来源：http://hni.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://wtd.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://iaq.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vvw.zhixingplan.top

TS:   s.indexOf("x")
来源：http://oyl.daxiang520.top

Java: s.indexOf("x")
来源：http://ezf.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://tye.tianlin.xyz

Ruby: s.index("x")
来源：http://bxl.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://fvn.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rug.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cdf.aibaodan.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uzm.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://djf.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lcr.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://crq.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mby.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://equ.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cqx.tarul.cn

[E06] 替换子串
来源：http://uot.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jiq.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://bjj.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mll.cqqwz.cn

TS:   s.replaceAll("a", "b")
来源：http://nvh.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://orp.feifeiyinyue.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qbw.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jcl.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://ltk.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://mur.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kkn.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wto.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://xux.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://gqu.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://exa.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iam.meibo888.top

Ruby: s.split(",");  s.split
来源：http://jbr.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://osh.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://svz.tanke756.top

Py:   ",".join(items)
来源：http://zwa.havefunace.top

PHP:  implode(",", $items);
来源：http://vyv.cashguo.top

JS:   items.join(",")
来源：http://zrj.hesvh.cn

TS:   items.join(",")
来源：http://dbf.ydjk.org.cn

Java: String.join(",", items)
来源：http://dxv.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://opc.jiagoushi.top

Ruby: items.join(",")
来源：http://wzc.hcnkem.com

C#:   string.Join(",", items)
来源：http://vow.chenlongwang.top

[E09] 去除所有空白字符
来源：http://ujv.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ale.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uac.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://rsk.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://vgy.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://udy.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://srz.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://gpx.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://grq.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://hzn.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://txx.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://err.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://gzc.zhengqikj.top

TS:   "7".padStart(3, "0")
来源：http://osk.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://muj.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://kwc.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yps.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sda.jianghu66.top

[E11] 反转字符串
来源：http://wnm.ydzc1.top

Py:   s[::-1]
来源：http://pay.pengpengdd.cyou

PHP:  strrev($s);
来源：http://uyq.shanyushiyangtech.top

JS:   [...s].reverse().join("")
来源：http://mle.jqgfzy.top

TS:   [...s].reverse().join("")
来源：http://cbd.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://klg.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://llk.jiagoushi.top

Ruby: s.reverse
来源：http://mtp.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://eqq.aizwys.cn

[E12] 统计某字符出现次数
来源：http://mnu.yuanzhike.top

Py:   s.count("a")
来源：http://lnd.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://ies.jqgufenzy.top

JS:   s.split("a").length - 1
来源：http://ufj.cheryme.top

TS:   s.split("a").length - 1
来源：http://rfq.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tqm.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://dyb.ivvv.top

Ruby: s.count("a")
来源：http://hdy.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://qsb.hfpthk.cn

[E13] 逐字符遍历
来源：http://rxm.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://stx.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hup.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ewd.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://bmu.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tlc.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iwz.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ksf.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cof.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://qqk.jiagoushi.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uss.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rfz.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hba.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tdt.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://txa.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://naa.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xdb.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ajm.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://wus.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sai.hammf.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wnx.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rax.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://epi.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oce.zhoulong.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pgk.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lek.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vto.wangdashe.top

[E16] 数字千分位
来源：http://xye.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://uwg.ppjwa.cn

PHP:  number_format(1234567);
来源：http://wto.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pht.redwolf501.top

TS:   (1234567).toLocaleString("en-US")
来源：http://chb.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ffp.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oto.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ysb.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://ahb.ctjpmb.com

[E17] 首字母大写
来源：http://tsb.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qto.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://opg.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mcj.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qhw.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wvh.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aim.xylfe.cn

Ruby: s.capitalize
来源：http://afj.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gcw.ybcxt.top

[E18] 模板占位符替换
来源：http://jxy.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://clx.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://faw.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://iru.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dep.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://koh.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://shp.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qtn.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://coq.sysykeji.top

[E19] 多行文本按行拆分
来源：http://xnx.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://ygw.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mkn.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://ccf.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://wik.yanxiufei.cn

Java: s.lines().toList()
来源：http://ytx.cdnleiting.top

Go:   strings.Split(s, "\n")
来源：http://wqz.zdqjudy.top

Ruby: s.lines
来源：http://eic.c1oappe.top

C#:   s.Split('\n')
来源：http://zdu.daxiang520.top

[E20] 判断字符串是否为空
来源：http://lqt.shzxlz.cn

Py:   if not s:
来源：http://otf.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xgg.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iix.hcnkem.com

TS:   if (s === "") {}
来源：http://tlr.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://oyf.zhiwuduotai.top

Go:   if s == "" {}
来源：http://fnx.pycfn.com

Ruby: if s.empty?
来源：http://tcx.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yru.316326.xyz

[E21] 超长截断加省略号
来源：http://unw.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iuy.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xlx.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijm.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zce.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wbp.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://sqv.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gyz.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://and.aizwys.cn

[E22] 字节长度与字符长度
来源：http://luk.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jmd.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ynl.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xti.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gqy.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hxc.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zwe.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://ytw.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lje.daria6918.cn

================================================================================
来源：http://dnd.tian-w.cn

F. 文件与目录
来源：http://pwz.aibaodan.cn

================================================================================
来源：http://ano.jinqigufen.top

[F01] 读取整个文件
来源：http://cqa.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pyh.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://ime.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oqh.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qzi.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xmu.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hsh.jinghuilouyu.cn

Ruby: File.read("a.txt")
来源：http://zcg.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://fjx.vqdsnc.cn

[F02] 逐行读取文件
来源：http://krz.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oaa.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xlg.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jpf.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oao.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://egw.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jni.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tbm.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pap.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://rhx.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vzx.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xnb.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qgu.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rez.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ifl.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uts.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://zgc.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://knf.sysykeji.top

[F04] 追加写入文件
来源：http://rfo.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nci.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vzm.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rdj.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qmq.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cnc.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jbl.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xtv.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jxw.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://zen.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gzm.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://ovh.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://mhz.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://owv.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://klp.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tnd.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://gny.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://lkn.sweek.top

[F06] 删除文件
来源：http://vdb.316326.xyz

Py:   os.remove("a.txt")
来源：http://mko.uphjek.com

PHP:  unlink("a.txt");
来源：http://ptf.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://uqe.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zdb.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yjb.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://vec.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://ail.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://ley.aizwys.cn

[F07] 创建目录（含多级）
来源：http://zno.daxiang520.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oly.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tkh.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pqx.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cyv.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cuu.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uxj.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gdr.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xwk.xinyue.icu

[F08] 遍历目录
来源：http://cge.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vbm.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://irj.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://mjw.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://ulc.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tev.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://wjr.sweek.top

Ruby: Dir.children("dir")
来源：http://iva.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://tyk.tanke756.top

[F09] 获取文件大小
来源：http://lme.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://aiw.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://pag.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://yip.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://wwo.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://uzj.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://axo.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://tkk.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://rne.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://mxm.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ncj.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ngc.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dfs.tian-w.cn

TS:   path.extname("a.txt")
来源：http://vnv.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wmj.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kzb.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blg.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fmk.xylfe.cn

[F11] 复制与移动文件
来源：http://jla.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oip.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://axm.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ivk.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ljf.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vgi.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ftn.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mmu.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xed.svipenyu.cn

[F12] CSV 读写
来源：http://xmr.shuidangran.top


<!-- 参考信息 -->