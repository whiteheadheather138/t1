代发 wailian999

[E02] 重复字符串
来源：http://oah.guowangkeji.top

Py:   "ab" * 3
来源：http://yze.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://tfl.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://wei.fktsv.cn

TS:   "ab".repeat(3)
来源：http://hpz.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://jyh.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://ngw.hcnkem.com

Ruby: "ab" * 3
来源：http://eqd.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cwg.vqdsnc.cn

[E03] 截取子串
来源：http://nkz.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hkx.epnwcf.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uza.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://obv.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://vrd.chenlongwang.top

Java: s.substring(1, 4)
来源：http://vmd.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lnu.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://tna.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://obt.xuanzx.com

[E04] 查找子串位置
来源：http://pwr.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://uty.cashguo.top

PHP:  strpos($s, "x");
来源：http://pda.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vqs.dashuyun.cn

TS:   s.indexOf("x")
来源：http://ygx.sysykeji.top

Java: s.indexOf("x")
来源：http://ezu.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://jen.wangshuangyany.cn

Ruby: s.index("x")
来源：http://ghz.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://bey.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jpf.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://thz.yongpay.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dpv.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bfm.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://rhk.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oyf.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rye.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tmt.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hat.shanyushiyangtech.top

[E06] 替换子串
来源：http://ucq.hywenlv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://npa.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://ksl.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wxk.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://hey.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nds.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ijl.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://skn.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://pxo.gogol.net.cn

[E07] 按分隔符拆分
来源：http://vvn.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mss.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://knm.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vpu.fanxiaobao.xyz

TS:   s.split(",")
来源：http://jcu.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://vjl.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uql.yonumen.top

Ruby: s.split(",");  s.split
来源：http://bzy.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sab.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://lmk.jyoumei.cn

Py:   ",".join(items)
来源：http://zuv.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://yat.guowangkeji.top

JS:   items.join(",")
来源：http://xpq.feifeiyinyue.top

TS:   items.join(",")
来源：http://gzl.kuanghao11.cn

Java: String.join(",", items)
来源：http://maj.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://zss.nanxuanxn.top

Ruby: items.join(",")
来源：http://fyd.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://wdt.cqqwz.cn

[E09] 去除所有空白字符
来源：http://rhv.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bpo.jlsjyb.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ypu.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://dav.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://qay.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://ksq.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tpf.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://nml.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ynr.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://ofv.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zrh.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eri.sufxvd.cn

JS:   "7".padStart(3, "0")
来源：http://tyu.yueranfly.top

TS:   "7".padStart(3, "0")
来源：http://nlc.epnwcf.com

Java: String.format("%03d", 7)
来源：http://qas.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mao.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tah.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hol.cucudq.cn

[E11] 反转字符串
来源：http://rqf.xziqi.cn

Py:   s[::-1]
来源：http://aha.cqqwz.cn

PHP:  strrev($s);
来源：http://zpv.guannengcc.top

JS:   [...s].reverse().join("")
来源：http://yqn.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://fle.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wuy.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gox.pengpengdd.cyou

Ruby: s.reverse
来源：http://tip.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://iun.daxiang520.top

[E12] 统计某字符出现次数
来源：http://wpm.bjfxy.top

Py:   s.count("a")
来源：http://dzv.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://vpc.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://xqt.cashguo.top

TS:   s.split("a").length - 1
来源：http://lim.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dsq.yueranfly.top

Go:   strings.Count(s, "a")
来源：http://maz.yj20258.top

Ruby: s.count("a")
来源：http://hqp.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://yhu.birdmap.top

[E13] 逐字符遍历
来源：http://juj.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://aqw.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://awj.vqdsnc.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nqc.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mrp.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ylc.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jeg.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kct.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tdg.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://jsw.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qxs.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wlz.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uno.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hca.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lih.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ush.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ryy.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kdb.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://ncb.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ftm.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fuv.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fcr.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rzl.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vor.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jfb.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dho.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zqn.daxiang520.top

[E16] 数字千分位
来源：http://kes.andypj.xyz

Py:   f"{1234567:,}"
来源：http://zgn.ctjpmb.com

PHP:  number_format(1234567);
来源：http://dvb.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://qvy.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://amz.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uzi.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://csm.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rcs.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://hcm.chenzaomai.com

[E17] 首字母大写
来源：http://kyu.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fkc.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://rwn.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lpe.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cia.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ykg.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zuy.zhengqikj.top

Ruby: s.capitalize
来源：http://vze.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://twr.hywenlv.cn

[E18] 模板占位符替换
来源：http://efa.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://igd.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hqy.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pgy.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aya.zhijiandao.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yxt.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gac.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ian.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vga.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://psx.shanyushiyangtech.top

Py:   s.splitlines()
来源：http://req.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kfx.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://rpb.ydjk.org.cn

TS:   s.split(/\r?\n/)
来源：http://pyx.xinyue.icu

Java: s.lines().toList()
来源：http://kpk.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://jit.yvedp.cn

Ruby: s.lines
来源：http://ont.zhijiandao.cn

C#:   s.Split('\n')
来源：http://nlh.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://fdh.zhengqikj.top

Py:   if not s:
来源：http://rwh.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ybd.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vjq.yj20258.top

TS:   if (s === "") {}
来源：http://pcp.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://aoo.gogol.net.cn

Go:   if s == "" {}
来源：http://hbp.yvedp.cn

Ruby: if s.empty?
来源：http://ukc.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cbd.yfazqb.com

[E21] 超长截断加省略号
来源：http://eur.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qpz.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xcy.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://drd.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jij.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rwd.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://iga.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bsw.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kte.jianghu66.top

[E22] 字节长度与字符长度
来源：http://tjd.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ocg.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xgc.nanxinkj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qpz.chenlongwang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ftg.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gdm.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ozt.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://dhy.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rgm.tanke756.top

================================================================================
来源：http://ebv.gotoacloud.top

F. 文件与目录
来源：http://ybq.daxiang520.top

================================================================================
来源：http://qkl.yongpay.top

[F01] 读取整个文件
来源：http://qzl.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hvc.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://poc.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sbx.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cwx.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ysb.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://loh.yfazqb.com

Ruby: File.read("a.txt")
来源：http://dbr.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://yjf.yangfankeji.com

[F02] 逐行读取文件
来源：http://ceo.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jor.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nsx.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ptq.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://usq.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xga.hfpthk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hbo.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hgx.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mcs.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://lkr.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hxb.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rcy.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bsb.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://edr.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wed.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mow.xziqi.cn

Ruby: File.write("a.txt", "hi")
来源：http://xot.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pmd.jyoumei.cn

[F04] 追加写入文件
来源：http://xue.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dyj.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zly.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://esx.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ggs.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rks.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hgn.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hdw.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aol.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://ugn.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uew.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://juc.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://adr.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://fja.jinqigfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wld.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tfk.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://acf.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://bns.xuetiantiany.cn

[F06] 删除文件
来源：http://dnq.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://fwf.havefunace.top

PHP:  unlink("a.txt");
来源：http://iiq.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xeb.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hnr.zycfv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oft.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://mvp.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://ywp.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://emj.hesvh.cn

[F07] 创建目录（含多级）
来源：http://tgl.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hqj.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://toz.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://saa.bjfxy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wks.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xte.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lhy.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qty.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gvh.fktsv.cn

[F08] 遍历目录
来源：http://fry.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jem.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uzi.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://ttn.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://ecc.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://knb.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gvs.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://lnq.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://xal.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://fxg.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://hqj.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://cpw.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://zit.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://jaa.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://zpe.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://umx.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://gmt.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://ebt.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://jjl.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bxd.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rzn.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://swd.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://joz.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qqs.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aja.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fgz.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jnx.hnxiangtu.top

[F11] 复制与移动文件
来源：http://sca.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ljo.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iij.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aig.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://skk.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hsb.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kud.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rfx.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zem.jinghuilouyu.cn

[F12] CSV 读写
来源：http://sfk.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sbl.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gog.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rmt.snrcjt.cn

TS:   // 同上
来源：http://hpr.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cwr.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rav.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rap.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://und.yuxming.cn


<!-- 参考信息 -->