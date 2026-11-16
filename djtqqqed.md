代发 wailian999

TS:   "ab".repeat(3)
来源：http://yvz.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://xky.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://jlr.zdbjq.cn

Ruby: "ab" * 3
来源：http://tdy.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ixr.yangfankeji.com

[E03] 截取子串
来源：http://ftd.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jiq.yvedp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tkn.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eho.yj20258.top

TS:   s.slice(1, 4)
来源：http://vrf.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://rhn.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fih.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://dlh.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://pby.ivvv.top

[E04] 查找子串位置
来源：http://kbf.pycfn.com

Py:   s.find("x");  s.index("x")
来源：http://oap.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://ssp.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://azd.jianghu66.top

TS:   s.indexOf("x")
来源：http://buz.zhoulong.xyz

Java: s.indexOf("x")
来源：http://qsc.meibo888.top

Go:   strings.Index(s, "x")
来源：http://cxd.c1oappe.top

Ruby: s.index("x")
来源：http://fss.tian-w.cn

C#:   s.IndexOf("x")
来源：http://bqw.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ikm.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dar.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ash.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aff.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xgn.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rsd.fengsongda.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kpp.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qbo.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mkx.yj20258.top

[E06] 替换子串
来源：http://xdz.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qza.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://sng.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zql.bbcook.cn

TS:   s.replaceAll("a", "b")
来源：http://agw.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pzf.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oxm.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zql.gzhubu.top

C#:   s.Replace("a", "b")
来源：http://mgj.yj202588.top

[E07] 按分隔符拆分
来源：http://oyj.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://otk.hfpthk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://emd.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iwg.jlsjyb.cn

TS:   s.split(",")
来源：http://spm.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://xmx.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ktm.yj202588.top

Ruby: s.split(",");  s.split
来源：http://gro.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hsl.meibo888.top

[E08] 数组按分隔符合并
来源：http://fnv.chenjidiqi.icu

Py:   ",".join(items)
来源：http://hoz.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://vbb.shangyingyoupin.top

JS:   items.join(",")
来源：http://kjo.nanxinkj.top

TS:   items.join(",")
来源：http://qio.vqdsnc.cn

Java: String.join(",", items)
来源：http://dor.cashguo.top

Go:   strings.Join(items, ",")
来源：http://ktb.zhiwuduotai.top

Ruby: items.join(",")
来源：http://xma.yj202588.top

C#:   string.Join(",", items)
来源：http://zwd.jinqigufen.top

[E09] 去除所有空白字符
来源：http://rmy.sysykeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://joq.feifeiyinyue.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lnz.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://pni.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ieb.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://xty.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://baw.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://kqs.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ddw.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://oqi.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zff.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xhh.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://yue.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://chj.yongpay.top

Java: String.format("%03d", 7)
来源：http://ing.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fev.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jzb.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eck.cucudq.cn

[E11] 反转字符串
来源：http://zzi.mhx1999.top

Py:   s[::-1]
来源：http://fwr.zhengqikj.top

PHP:  strrev($s);
来源：http://xkl.jiagoushi.top

JS:   [...s].reverse().join("")
来源：http://krh.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://adb.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zev.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://nwr.svipenyu.cn

Ruby: s.reverse
来源：http://kxi.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hqc.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://gju.hnqzz.top

Py:   s.count("a")
来源：http://mab.tarul.cn

PHP:  substr_count($s, "a");
来源：http://dzm.shuidangran.top

JS:   s.split("a").length - 1
来源：http://yey.fktsv.cn

TS:   s.split("a").length - 1
来源：http://rwu.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zqc.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://dnv.shzxlz.cn

Ruby: s.count("a")
来源：http://jfr.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://qqb.zhongyouzk.top

[E13] 逐字符遍历
来源：http://bah.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://uev.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ghh.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xyw.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tyo.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zue.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oty.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ean.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dlt.fktsv.cn

[E14] URL 编码与 Base64
来源：http://uqb.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lsa.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://uhi.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vhs.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yql.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tpo.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wka.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dhk.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yar.ivvv.top

[E15] HTML 转义 / 反转义
来源：http://hjf.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lji.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lqk.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aer.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://znb.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zlr.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lzm.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uvb.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://guy.gotoacloud.top

[E16] 数字千分位
来源：http://pcz.316326.xyz

Py:   f"{1234567:,}"
来源：http://jer.hcnkem.com

PHP:  number_format(1234567);
来源：http://pzn.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wfl.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qal.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rza.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xej.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kge.quarkkingdee.top

C#:   1234567.ToString("N0")
来源：http://fzb.nwbrower.top

[E17] 首字母大写
来源：http://rqd.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fhu.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xot.yj20258888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ord.yfazqb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jkp.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kit.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fxe.quarkkingdee.top

Ruby: s.capitalize
来源：http://isb.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qch.0kj1m.cn

[E18] 模板占位符替换
来源：http://juf.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ylp.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ycn.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://ard.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rfy.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://szt.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pht.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://boq.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oxz.vehdjk.com

[E19] 多行文本按行拆分
来源：http://buh.iojbl.cn

Py:   s.splitlines()
来源：http://mlx.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ozl.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://ivu.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://spq.andypj.xyz

Java: s.lines().toList()
来源：http://osk.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://byt.vqdsnc.cn

Ruby: s.lines
来源：http://sod.zdbjq.cn

C#:   s.Split('\n')
来源：http://zob.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://rnw.zhaomingkeji.xyz

Py:   if not s:
来源：http://rph.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mfj.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://krh.sysykeji.top

TS:   if (s === "") {}
来源：http://zoc.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://tni.fehbvm.com

Go:   if s == "" {}
来源：http://qwi.wangshuangyany.cn

Ruby: if s.empty?
来源：http://ysv.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yhq.0kj1m.cn

[E21] 超长截断加省略号
来源：http://uwu.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gch.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vqu.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://srb.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pgw.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zot.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://dfk.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hpu.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jei.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://pdv.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qgt.mhx1999.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nfs.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rbm.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ugv.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cwp.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fzu.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://ljw.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sjh.vehdjk.com

================================================================================
来源：http://sst.cashguo.top

F. 文件与目录
来源：http://cxo.guowangkeji.top

================================================================================
来源：http://prl.sjlbkw.cn

[F01] 读取整个文件
来源：http://thw.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xsl.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://qkl.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://clj.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dbu.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xzp.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dot.birdmap.top

Ruby: File.read("a.txt")
来源：http://cuy.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://wfg.jinqigfzy.top

[F02] 逐行读取文件
来源：http://irl.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kkn.zhengqikj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gaq.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lkr.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kbl.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ywx.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vvs.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fuh.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nyy.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://scu.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uem.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://afv.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nqd.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nhd.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nbh.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uuo.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://boq.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nsc.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://osj.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wwc.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kqn.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jnl.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://are.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hbo.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eoh.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://byg.birdmap.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ctj.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://tyt.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uqw.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://ftq.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://aka.hysaishi.cn

TS:   fs.existsSync("a.txt")
来源：http://cfy.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://aqp.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aqh.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://ydt.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://uts.52xcode.cn

[F06] 删除文件
来源：http://ljn.xylfe.cn

Py:   os.remove("a.txt")
来源：http://zvt.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://msk.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://ygq.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://nav.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eik.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://ccc.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://ehm.yongpay.top

C#:   File.Delete("a.txt");
来源：http://qew.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://vku.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zeh.epnwcf.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://evk.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://roc.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vyj.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cqx.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cjv.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fnf.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://duy.hnqzz.top

[F08] 遍历目录
来源：http://jaa.0kj1m.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://alp.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ohl.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://qac.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://iqa.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vls.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dfc.quarkkingdee.top

Ruby: Dir.children("dir")
来源：http://ovn.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://wis.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://apm.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://boc.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://zne.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://asf.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://hte.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://tzb.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://utd.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://xkl.sysykeji.top

C#:   new FileInfo("a.txt").Length
来源：http://zts.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://mnk.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ruu.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dgd.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uty.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://klq.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xfg.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oed.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bhc.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ulh.hywenlv.cn

[F11] 复制与移动文件
来源：http://keo.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ayy.shanyushiyangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sxo.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cfc.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://keo.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jbt.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zim.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vqy.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rzr.wangdashe.top

[F12] CSV 读写
来源：http://xec.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qrf.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://txg.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kzj.zhiwuduotai.top

TS:   // 同上
来源：http://byl.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vdp.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hxi.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yfh.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://wsd.52xcode.cn

================================================================================
来源：http://vyp.jqgufenzy.top

G. 面向对象
来源：http://ntw.dianchejie.cn

================================================================================
来源：http://zvh.chenzaomai.com

[G01] 定义类
来源：http://fcz.ywan-chungtsiang.top


<!-- 参考信息 -->