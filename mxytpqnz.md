代发 wailian999

[E02] 重复字符串
来源：http://kof.hnqzz.top

Py:   "ab" * 3
来源：http://zqx.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://ovw.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://ljy.ybcxt.top

TS:   "ab".repeat(3)
来源：http://ftt.aizwys.cn

Java: "ab".repeat(3)
来源：http://kqq.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://ttm.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://beg.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iua.9152youxi.cn

[E03] 截取子串
来源：http://mwz.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bfo.dianchejie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yst.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lnt.yfazqb.com

TS:   s.slice(1, 4)
来源：http://blj.guannengcc.top

Java: s.substring(1, 4)
来源：http://vdo.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cbq.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://ubq.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://idd.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://gtx.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://uou.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://oxd.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fgm.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://qep.nanxinkj.top

Java: s.indexOf("x")
来源：http://rtv.uphjek.com

Go:   strings.Index(s, "x")
来源：http://kld.svipenyu.cn

Ruby: s.index("x")
来源：http://kef.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://rei.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zkg.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vmk.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qcd.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cuw.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xhp.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rld.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xva.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wff.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zwd.vqdsnc.cn

[E06] 替换子串
来源：http://van.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bha.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://mgy.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gpd.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://dwd.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sge.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://atb.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ibv.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://xsd.xylfe.cn

[E07] 按分隔符拆分
来源：http://tta.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wry.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ixc.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://azb.tian-w.cn

TS:   s.split(",")
来源：http://ydp.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://uxn.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tph.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://ixs.shanyushiyangtech.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hty.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://oav.shuidangran.top

Py:   ",".join(items)
来源：http://vpm.bbcook.cn

PHP:  implode(",", $items);
来源：http://eol.havefunace.top

JS:   items.join(",")
来源：http://dgx.cashguo.top

TS:   items.join(",")
来源：http://jtb.cashguo.top

Java: String.join(",", items)
来源：http://pmh.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://yge.guannengcc.top

Ruby: items.join(",")
来源：http://ahl.cheryme.top

C#:   string.Join(",", items)
来源：http://wjo.cucudq.cn

[E09] 去除所有空白字符
来源：http://blo.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rcy.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yni.ppjwa.cn

JS:   s.replace(/\s+/g, "")
来源：http://kws.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://yle.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://zkj.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://evw.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://gam.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sma.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://sxx.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mog.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rsa.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://daz.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://fir.vehdjk.com

Java: String.format("%03d", 7)
来源：http://oph.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rep.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dvw.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cfx.nwbrower.top

[E11] 反转字符串
来源：http://xbi.meibo888.top

Py:   s[::-1]
来源：http://lwb.zhongyouzk.top

PHP:  strrev($s);
来源：http://mzo.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://ijx.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://phw.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wfp.yongpay.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dsy.guowangkeji.top

Ruby: s.reverse
来源：http://vww.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://qyi.gzhubu.top

[E12] 统计某字符出现次数
来源：http://izc.zhijiandao.cn

Py:   s.count("a")
来源：http://iyw.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://bjs.smart0.xyz

JS:   s.split("a").length - 1
来源：http://eel.gzhubu.top

TS:   s.split("a").length - 1
来源：http://ham.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nwk.yj20258888.top

Go:   strings.Count(s, "a")
来源：http://tjn.aizwys.cn

Ruby: s.count("a")
来源：http://gyg.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://zvo.xuanzx.com

[E13] 逐字符遍历
来源：http://caf.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://bdr.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wrm.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sot.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gnc.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://icg.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tqy.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qkt.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dip.cucudq.cn

[E14] URL 编码与 Base64
来源：http://lgo.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iit.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ftg.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ntr.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wod.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lth.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qhl.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tym.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fji.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://jtv.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lfu.kuanghao11.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fwp.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hkc.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://zax.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yms.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nfb.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://peb.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nmv.yangfankeji.com

[E16] 数字千分位
来源：http://amf.hnqzz.top

Py:   f"{1234567:,}"
来源：http://dqj.aizwys.cn

PHP:  number_format(1234567);
来源：http://jye.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://vdn.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mif.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ihy.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tbr.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fts.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://uld.wangshuangyany.cn

[E17] 首字母大写
来源：http://vzj.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rww.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kyp.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jyp.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ary.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kfu.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bqy.feifeiyinyue.top

Ruby: s.capitalize
来源：http://ajs.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rci.zhoulong.xyz

[E18] 模板占位符替换
来源：http://ttv.jiagoushi.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ddp.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://txq.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bau.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zmk.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kgl.zhiwuduotai.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xky.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zko.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xjp.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://wcc.yanxiufei.cn

Py:   s.splitlines()
来源：http://mzb.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xya.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://caa.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://vlq.jqgufenzy.top

Java: s.lines().toList()
来源：http://wrc.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://utb.xinyue.icu

Ruby: s.lines
来源：http://ixu.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://wtn.haohaochexian.top

[E20] 判断字符串是否为空
来源：http://ucu.cashguo.top

Py:   if not s:
来源：http://kce.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oly.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://obk.ydjk.org.cn

TS:   if (s === "") {}
来源：http://pus.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://eha.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://wib.pengpengdd.cyou

Ruby: if s.empty?
来源：http://yod.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gkz.uphjek.com

[E21] 超长截断加省略号
来源：http://rqd.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uct.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xkw.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://azw.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zay.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://npu.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://kfl.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://omy.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dce.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://srg.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vem.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gui.nanxuanxn.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qno.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lkc.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bat.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kxb.sweek.top

Ruby: s.bytesize;  s.length
来源：http://osv.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lrx.pengpengdd.cyou

================================================================================
来源：http://bli.nwbrower.top

F. 文件与目录
来源：http://clp.birdmap.top

================================================================================
来源：http://kdr.kuanghao11.cn

[F01] 读取整个文件
来源：http://mmt.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uym.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://zij.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ypt.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yhc.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://swz.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lub.sysykeji.top

Ruby: File.read("a.txt")
来源：http://jtp.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://xuc.gzhubu.top

[F02] 逐行读取文件
来源：http://aug.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mtd.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kfi.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pwh.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pvq.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bin.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kbx.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jnw.bbcook.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jpi.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://mbp.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ivj.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hpr.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hxp.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cii.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mfc.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lol.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://zwx.sufxvd.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uvg.yonumen.top

[F04] 追加写入文件
来源：http://sap.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rfo.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jlo.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hud.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pcf.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rjp.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ljr.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jom.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qzb.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://hmw.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://znr.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://yat.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://sgo.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://hcj.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://zkj.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ewk.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://yqu.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://pbm.sufxvd.cn

[F06] 删除文件
来源：http://yzz.bjfxy.top

Py:   os.remove("a.txt")
来源：http://eiv.birdmap.top

PHP:  unlink("a.txt");
来源：http://iwq.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://btj.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://bno.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://apt.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://sxz.cheryme.top

Ruby: File.delete("a.txt")
来源：http://aad.yj20258.top

C#:   File.Delete("a.txt");
来源：http://jec.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://gqw.52xcode.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dtt.vehdjk.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gex.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mrz.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ocs.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ffx.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qsp.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kje.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mcq.bjfxy.top

[F08] 遍历目录
来源：http://lpb.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://jmt.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://spk.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://krg.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://xtr.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jnw.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://thr.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://kyc.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://yne.wangdashe.top

[F09] 获取文件大小
来源：http://noz.fanxiaobao.xyz

Py:   os.path.getsize("a.txt")
来源：http://ste.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://jvu.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://bvf.zycfv.cn

TS:   fs.statSync("a.txt").size
来源：http://ngr.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://uve.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fdj.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://kek.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://mzq.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://pbw.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jkm.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fai.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hpx.yvedp.cn

TS:   path.extname("a.txt")
来源：http://rno.zhongyouzk.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dge.kuanghao11.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hfa.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://obw.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ina.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://oqo.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uei.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://liz.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mzg.fengsongda.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nhb.tanke756.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://osq.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uko.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rwt.havefunace.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xzr.jqgfzy.top

[F12] CSV 读写
来源：http://lcf.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ros.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://stf.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ila.meibo888.top

TS:   // 同上
来源：http://owl.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nky.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cvm.cqqwz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wxr.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cvm.yj202588.top


<!-- 参考信息 -->