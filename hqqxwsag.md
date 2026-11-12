代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nfe.pycfn.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ndi.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://upl.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oze.hcnkem.com

[E02] 重复字符串
来源：http://dsz.andypj.xyz

Py:   "ab" * 3
来源：http://ipz.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://sgg.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://vxs.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://ftk.jiagoushi.top

Java: "ab".repeat(3)
来源：http://qfk.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://xci.aizwys.cn

Ruby: "ab" * 3
来源：http://ski.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://txs.yangfankeji.com

[E03] 截取子串
来源：http://dqe.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zgp.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vub.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ymk.zycfv.cn

TS:   s.slice(1, 4)
来源：http://nxg.c1oappe.top

Java: s.substring(1, 4)
来源：http://ydt.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tro.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://eno.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://alz.haohaochexian.top

[E04] 查找子串位置
来源：http://tyq.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://nwg.uphjek.com

PHP:  strpos($s, "x");
来源：http://ndl.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://knh.yfazqb.com

TS:   s.indexOf("x")
来源：http://nuj.gogol.net.cn

Java: s.indexOf("x")
来源：http://exf.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://vkl.xylfe.cn

Ruby: s.index("x")
来源：http://uxa.bbcook.cn

C#:   s.IndexOf("x")
来源：http://xas.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://waf.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uhb.havefunace.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aen.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ucf.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ono.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aad.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vjk.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://raf.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://psz.zdqjudy.top

[E06] 替换子串
来源：http://yuf.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uda.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://kli.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qjt.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://fyc.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qis.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vmf.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wlz.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://nvj.wangdashe.top

[E07] 按分隔符拆分
来源：http://edj.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fjw.hammf.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dsz.snrcjt.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wht.gotoacloud.top

TS:   s.split(",")
来源：http://pdd.gaohongyu789.top

Java: s.split(",");  s.split("\\s+")
来源：http://dcw.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://smk.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://uyf.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pdj.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://wjr.xuanzx.com

Py:   ",".join(items)
来源：http://vdo.pycfn.com

PHP:  implode(",", $items);
来源：http://wzq.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://wkz.hongshengwenyu.top

TS:   items.join(",")
来源：http://jze.nanxinkj.top

Java: String.join(",", items)
来源：http://nae.pycfn.com

Go:   strings.Join(items, ",")
来源：http://jqk.ybcxt.top

Ruby: items.join(",")
来源：http://xzi.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://uff.sxryk.cn

[E09] 去除所有空白字符
来源：http://sdn.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pvi.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wrj.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nbe.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://wyx.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://frd.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rqp.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://mry.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sgm.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://lho.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vdm.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ata.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://opu.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://lpx.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://tkq.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mdw.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rws.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kah.jqgfzy.top

[E11] 反转字符串
来源：http://zzf.hesvh.cn

Py:   s[::-1]
来源：http://coz.jqgfzy.top

PHP:  strrev($s);
来源：http://tpn.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://iyu.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://flj.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wvu.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://lce.feifeiyinyue.top

Ruby: s.reverse
来源：http://ioz.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fcp.yongpay.top

[E12] 统计某字符出现次数
来源：http://oyn.havefunace.top

Py:   s.count("a")
来源：http://lab.tian-w.cn

PHP:  substr_count($s, "a");
来源：http://bsw.52xcode.cn

JS:   s.split("a").length - 1
来源：http://iup.tanke756.top

TS:   s.split("a").length - 1
来源：http://asj.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://omp.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://doj.yongpay.top

Ruby: s.count("a")
来源：http://ore.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://ozy.cheryme.top

[E13] 逐字符遍历
来源：http://kvq.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://qao.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yks.vqdsnc.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xno.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fzx.aizwys.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wll.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dny.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://soc.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uqs.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://pdj.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fcp.aizwys.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fbw.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zbq.jqgfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hkc.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jup.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wyr.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dka.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wsu.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://jhy.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mrl.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tlo.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wea.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vrl.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://egt.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kwc.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rmh.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://osn.fanxiaobao.xyz

[E16] 数字千分位
来源：http://hxo.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://omb.yueranfly.top

PHP:  number_format(1234567);
来源：http://jpf.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://lxq.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dlp.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vkq.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hpj.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bcc.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://wch.ydzc1.top

[E17] 首字母大写
来源：http://zsb.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ufr.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://wkt.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mcu.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xtw.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fcz.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cxf.tian-w.cn

Ruby: s.capitalize
来源：http://oes.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zlj.tarul.cn

[E18] 模板占位符替换
来源：http://elv.316326.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xrf.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rjy.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mjm.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zyj.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cym.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mee.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://geo.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ehh.yvedp.cn

[E19] 多行文本按行拆分
来源：http://pmz.jinghuilouyu.cn

Py:   s.splitlines()
来源：http://dvm.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vip.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://lkj.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://uat.cucudq.cn

Java: s.lines().toList()
来源：http://otf.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://nqm.jqgfzy.top

Ruby: s.lines
来源：http://wfl.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://ntr.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://uuo.ydzc1.top

Py:   if not s:
来源：http://qit.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://len.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jaq.nanxinkj.top

TS:   if (s === "") {}
来源：http://puk.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://dtr.yongpay.top

Go:   if s == "" {}
来源：http://uxf.zhixingplan.top

Ruby: if s.empty?
来源：http://iml.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xhl.ydzc1.top

[E21] 超长截断加省略号
来源：http://svh.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yqa.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iuw.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zna.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tja.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zot.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://vtd.sjlbkw.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ukz.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://luj.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://eeh.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sla.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gpt.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://szh.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vkl.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uwt.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kug.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://usy.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cta.zhongyouzk.top

================================================================================
来源：http://due.hywenlv.cn

F. 文件与目录
来源：http://avr.fzhhl.top

================================================================================
来源：http://ots.yonumen.top

[F01] 读取整个文件
来源：http://djd.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://snp.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://vhs.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hhx.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://urc.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cno.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eds.jiagoushi.top

Ruby: File.read("a.txt")
来源：http://rgc.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://mwq.cqqwz.cn

[F02] 逐行读取文件
来源：http://bbj.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vuz.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ukh.quarkkingdee.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wii.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tkh.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qio.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jdo.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rce.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wxl.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://wbs.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cue.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jgs.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pou.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uia.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rze.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://seg.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://vxt.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eru.316326.xyz

[F04] 追加写入文件
来源：http://hzf.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vlf.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cey.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://now.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tpg.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uju.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lsr.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rbd.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wfz.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://zvd.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ftx.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://usy.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://bmq.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://ltu.fanxiaobao.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://mxq.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kuq.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://zev.kuanghao11.cn

C#:   File.Exists("a.txt")
来源：http://nyy.pengpengdd.cyou

[F06] 删除文件
来源：http://wos.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://nms.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://nzx.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://obb.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://pdq.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rio.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://ork.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://lje.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://epy.yanxiufei.cn

[F07] 创建目录（含多级）
来源：http://loz.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xzz.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://och.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ptf.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iin.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cha.fktsv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vtb.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bao.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wxh.jqgufenzy.top

[F08] 遍历目录
来源：http://sao.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://vvp.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://spu.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://lbi.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://qol.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mut.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://lwp.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://icz.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://pbw.haohaochexian.top

[F09] 获取文件大小
来源：http://fiz.shuidangran.top

Py:   os.path.getsize("a.txt")
来源：http://rnr.hammf.cn

PHP:  filesize("a.txt");
来源：http://xoz.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://epu.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://jmv.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://odx.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tdy.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://fou.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://nxm.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://guf.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qss.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rfe.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tcl.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://ynb.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qep.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xra.jlsjyb.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wzi.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cfw.ppjwa.cn

[F11] 复制与移动文件
来源：http://afa.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://biw.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://llq.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yfi.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rag.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qma.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fck.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://boy.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://prc.hysaishi.cn

[F12] CSV 读写
来源：http://xqj.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qbj.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pyf.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cqh.yfazqb.com

TS:   // 同上
来源：http://ldw.hnxiangtu.top


<!-- 参考信息 -->