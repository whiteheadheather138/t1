代发 wailian999

Java: String.join(", ", list)
来源：http://xoa.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://sop.aizwys.cn

Ruby: arr.join(", ")
来源：http://bmc.tanke756.top

C#:   string.Join(", ", list)
来源：http://tzj.chenlongwang.top

================================================================================
来源：http://yjc.hywenlv.cn

E. 字符串处理
来源：http://cvf.zdbjq.cn

================================================================================
来源：http://ubu.ydjk.org.cn

[E01] 拼接字符串
来源：http://oqq.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iyi.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iox.tarul.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sbd.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mkj.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ecw.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rre.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fbe.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ayr.zhixingplan.top

[E02] 重复字符串
来源：http://inq.pengpengdd.cyou

Py:   "ab" * 3
来源：http://dav.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://bnh.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://vzd.bjfxy.top

TS:   "ab".repeat(3)
来源：http://fpk.tanke756.top

Java: "ab".repeat(3)
来源：http://ryk.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://bib.cucudq.cn

Ruby: "ab" * 3
来源：http://aoi.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ddd.yvedp.cn

[E03] 截取子串
来源：http://ryy.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://boa.jianghu66.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zqj.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eiv.yj20258888.top

TS:   s.slice(1, 4)
来源：http://lsl.yonumen.top

Java: s.substring(1, 4)
来源：http://xzs.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gmk.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://zca.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://qhz.xuetiantiany.cn

[E04] 查找子串位置
来源：http://rlq.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://itw.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://xze.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cuv.yuanzhike.top

TS:   s.indexOf("x")
来源：http://awz.shzxlz.cn

Java: s.indexOf("x")
来源：http://rgj.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://lwb.xziqi.cn

Ruby: s.index("x")
来源：http://fcn.andypj.xyz

C#:   s.IndexOf("x")
来源：http://sxu.yj202588.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yxm.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jug.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qli.daxiang520.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ixi.xuetiantiany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fhj.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zpl.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lis.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rza.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lts.vehdjk.com

[E06] 替换子串
来源：http://phi.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cbl.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://esv.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oln.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://aha.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dni.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xtx.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aff.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://ndt.zycfv.cn

[E07] 按分隔符拆分
来源：http://pkn.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tak.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://smh.iojbl.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://clr.ybcxt.top

TS:   s.split(",")
来源：http://pmu.ctjpmb.com

Java: s.split(",");  s.split("\\s+")
来源：http://ttf.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fab.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://bkw.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gru.tarul.cn

[E08] 数组按分隔符合并
来源：http://dnk.xziqi.cn

Py:   ",".join(items)
来源：http://yhv.gotoacloud.top

PHP:  implode(",", $items);
来源：http://uik.sweek.top

JS:   items.join(",")
来源：http://ncn.shanyushiyangtech.top

TS:   items.join(",")
来源：http://oqm.52xcode.cn

Java: String.join(",", items)
来源：http://ygj.yonumen.top

Go:   strings.Join(items, ",")
来源：http://bxo.dashuyun.cn

Ruby: items.join(",")
来源：http://kig.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://ghc.yj20258888.top

[E09] 去除所有空白字符
来源：http://lej.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://std.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rdc.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://gde.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://uni.andypj.xyz

Java: s.replaceAll("\\s+", "")
来源：http://vko.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wor.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ort.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yqg.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://vxk.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fkt.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lpb.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://srj.yfazqb.com

TS:   "7".padStart(3, "0")
来源：http://pxq.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://yxm.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uzi.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sjd.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wxp.jqgfzy.top

[E11] 反转字符串
来源：http://mqg.yj20258888.top

Py:   s[::-1]
来源：http://vbd.birdmap.top

PHP:  strrev($s);
来源：http://oss.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://pbh.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://zlj.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vqo.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ihp.fzhhl.top

Ruby: s.reverse
来源：http://yim.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://oej.gzhubu.top

[E12] 统计某字符出现次数
来源：http://tcp.yj202588.top

Py:   s.count("a")
来源：http://gsv.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://arl.nwbrower.top

JS:   s.split("a").length - 1
来源：http://omf.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://cbt.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://reh.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://aok.nanxuanxn.top

Ruby: s.count("a")
来源：http://wcg.hammf.cn

C#:   s.Count(c => c == 'a')
来源：http://vwe.gaohongyu789.top

[E13] 逐字符遍历
来源：http://ckj.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://dip.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://udn.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xhf.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qah.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vpt.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kwa.epnwcf.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ety.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ujj.birdmap.top

[E14] URL 编码与 Base64
来源：http://kta.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gdj.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eeg.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://etz.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://irq.zhoulong.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pex.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hlg.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iev.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ubk.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://xtc.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zyq.mhx1999.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zfo.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qph.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ruz.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://clu.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kyy.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://toa.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fwo.hysaishi.cn

[E16] 数字千分位
来源：http://zrz.cucudq.cn

Py:   f"{1234567:,}"
来源：http://kgu.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://gxx.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xca.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://iup.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sjx.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jid.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xxs.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://zbn.jianghu66.top

[E17] 首字母大写
来源：http://crz.yanxiufei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yfj.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hob.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://obq.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jrs.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jzq.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pht.gotoacloud.top

Ruby: s.capitalize
来源：http://bpi.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ttb.yvedp.cn

[E18] 模板占位符替换
来源：http://dkz.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gjk.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mfd.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tjl.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zmq.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ido.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zui.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://njz.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://azi.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://hmn.aibaodan.cn

Py:   s.splitlines()
来源：http://yrd.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uko.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://gyp.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://lzz.jianghu66.top

Java: s.lines().toList()
来源：http://xvb.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://npt.zhixingplan.top

Ruby: s.lines
来源：http://tmy.jianghu66.top

C#:   s.Split('\n')
来源：http://awp.ybcxt.top

[E20] 判断字符串是否为空
来源：http://gzn.fzhhl.top

Py:   if not s:
来源：http://kaa.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://efm.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vil.pycfn.com

TS:   if (s === "") {}
来源：http://she.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://tss.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://qfx.wangdashe.top

Ruby: if s.empty?
来源：http://tas.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wus.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://nps.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mza.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://znq.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cnh.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ztr.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uim.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://hdj.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wdv.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zts.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://zta.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://roz.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qdi.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kuh.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cjv.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yqz.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://shd.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://hlo.cheryme.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://thq.xziqi.cn

================================================================================
来源：http://wlk.tarul.cn

F. 文件与目录
来源：http://tki.yongpay.top

================================================================================
来源：http://lpz.shzxlz.cn

[F01] 读取整个文件
来源：http://fjx.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://npl.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://lom.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iof.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://daf.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dau.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jkj.fehbvm.com

Ruby: File.read("a.txt")
来源：http://xvm.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://mxq.yonumen.top

[F02] 逐行读取文件
来源：http://sez.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ycd.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iji.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nbp.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ill.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hcw.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zos.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://moy.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gso.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://jyx.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uru.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jbv.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dlj.xziqi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zlk.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lwl.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pgc.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://kww.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lqo.hammf.cn

[F04] 追加写入文件
来源：http://dns.chenzaomai.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cjt.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kfo.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aso.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nrg.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mvp.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jji.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ssy.hongshengwenyu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gwt.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://nbl.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://usu.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://fhe.fengsongda.top

JS:   fs.existsSync("a.txt")
来源：http://mfd.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://dlz.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fyp.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ajl.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://hyq.guowangkeji.top

C#:   File.Exists("a.txt")
来源：http://zok.shzxlz.cn

[F06] 删除文件
来源：http://xkk.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://uve.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://byi.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://ixo.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eue.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jbq.ctjpmb.com

Go:   os.Remove("a.txt")
来源：http://wgn.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://gqo.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://xty.xinyue.icu

[F07] 创建目录（含多级）
来源：http://qyq.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pmd.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wah.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://onj.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxr.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://izc.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mvq.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jbm.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mas.shangyingyoupin.top

[F08] 遍历目录
来源：http://cwu.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lzu.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://egy.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://kqa.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://ntj.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qte.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wde.mhx1999.top

Ruby: Dir.children("dir")
来源：http://kdg.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://vst.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://foe.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://duf.cheryme.top

PHP:  filesize("a.txt");
来源：http://ocd.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://mjj.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://dqp.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://hff.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rle.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://hep.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://bmu.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://xqr.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dws.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://duo.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cek.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://rbf.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vps.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oxk.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pdf.ivvv.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bcc.vehdjk.com

[F11] 复制与移动文件
来源：http://hve.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ptp.cqqwz.cn


<!-- 参考信息 -->