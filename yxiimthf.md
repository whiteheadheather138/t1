代发 wailian999

[E02] 重复字符串
来源：http://zlh.bbcook.cn

Py:   "ab" * 3
来源：http://qpm.ppjwa.cn

PHP:  str_repeat("ab", 3);
来源：http://tll.fzhhl.top

JS:   "ab".repeat(3)
来源：http://pto.fzhhl.top

TS:   "ab".repeat(3)
来源：http://eac.daxiang520.top

Java: "ab".repeat(3)
来源：http://jze.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://fqn.cashguo.top

Ruby: "ab" * 3
来源：http://ntt.bbcook.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://peq.jqgfzy.top

[E03] 截取子串
来源：http://hgc.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rix.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hoq.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ial.bbcook.cn

TS:   s.slice(1, 4)
来源：http://rnn.gotoacloud.top

Java: s.substring(1, 4)
来源：http://inc.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wce.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://udk.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://bhx.guowangkeji.top

[E04] 查找子串位置
来源：http://geg.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://umn.yueranfly.top

PHP:  strpos($s, "x");
来源：http://oyv.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fvo.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://ixj.zhixingplan.top

Java: s.indexOf("x")
来源：http://hxo.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://wwy.9152youxi.cn

Ruby: s.index("x")
来源：http://wjg.zdqjudy.top

C#:   s.IndexOf("x")
来源：http://gdw.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rbj.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ocs.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://olq.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rlz.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fnd.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ttz.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ttc.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ahk.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yid.yfazqb.com

[E06] 替换子串
来源：http://rfp.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vma.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://ocy.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rik.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://vzb.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tvk.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dpp.zhixingplan.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eep.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://azw.daria6918.cn

[E07] 按分隔符拆分
来源：http://auw.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pwu.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qvp.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://oxy.yuanzhike.top

TS:   s.split(",")
来源：http://zbq.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://wzy.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jkr.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://lvq.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zbu.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://ivt.svipenyu.cn

Py:   ",".join(items)
来源：http://mwm.fehbvm.com

PHP:  implode(",", $items);
来源：http://eyb.jqgfzy.top

JS:   items.join(",")
来源：http://fsr.gaohongyu789.top

TS:   items.join(",")
来源：http://koy.dashuyun.cn

Java: String.join(",", items)
来源：http://wel.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://lqx.ctjpmb.com

Ruby: items.join(",")
来源：http://kih.9152youxi.cn

C#:   string.Join(",", items)
来源：http://hiq.vehdjk.com

[E09] 去除所有空白字符
来源：http://jrk.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xbr.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ioh.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://kqs.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://lrg.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://fkm.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://emk.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://djh.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sng.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://gag.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cfx.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yvt.daxiang520.top

JS:   "7".padStart(3, "0")
来源：http://cqm.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://jcz.mhx1999.top

Java: String.format("%03d", 7)
来源：http://jiw.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gnb.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nhk.bjfxy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://glh.zycfv.cn

[E11] 反转字符串
来源：http://afd.hongshengwenyu.top

Py:   s[::-1]
来源：http://xax.zhixingplan.top

PHP:  strrev($s);
来源：http://lhe.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://kek.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://cty.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mrg.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://npg.yueranfly.top

Ruby: s.reverse
来源：http://pwl.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wnj.fktsv.cn

[E12] 统计某字符出现次数
来源：http://laf.ybcxt.top

Py:   s.count("a")
来源：http://qhy.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://fdx.0kj1m.cn

JS:   s.split("a").length - 1
来源：http://ies.hesvh.cn

TS:   s.split("a").length - 1
来源：http://yfm.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vcv.ivvv.top

Go:   strings.Count(s, "a")
来源：http://hgt.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://hff.zhaomingkeji.xyz

C#:   s.Count(c => c == 'a')
来源：http://scc.tianlin.xyz

[E13] 逐字符遍历
来源：http://chi.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://ytl.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://acy.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qwy.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hhc.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jam.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cel.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rsm.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ice.sxryk.cn

[E14] URL 编码与 Base64
来源：http://fil.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jfp.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://aqz.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jcq.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qlc.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cwq.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mlc.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ngc.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qsi.zhijiandao.cn

[E15] HTML 转义 / 反转义
来源：http://vpt.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lix.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iou.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://daj.cqqwz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zng.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://odc.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wun.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kmr.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tpd.yanxiufei.cn

[E16] 数字千分位
来源：http://eoj.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://wwr.birdmap.top

PHP:  number_format(1234567);
来源：http://tvz.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://rzf.jinyuanbaomall.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rvl.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dxl.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zlo.meibo888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jyg.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://jpe.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://gld.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hln.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://ytt.yj20258888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yhc.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lti.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://txa.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://irp.birdmap.top

Ruby: s.capitalize
来源：http://yih.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wxa.hesvh.cn

[E18] 模板占位符替换
来源：http://hiv.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ayi.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gmp.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tjc.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mro.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lkw.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lge.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vly.hnqzz.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jbo.hammf.cn

[E19] 多行文本按行拆分
来源：http://szl.cheryme.top

Py:   s.splitlines()
来源：http://rfr.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yjn.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://hen.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://sxf.0kj1m.cn

Java: s.lines().toList()
来源：http://dnu.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://rbl.cqqwz.cn

Ruby: s.lines
来源：http://biz.tanke756.top

C#:   s.Split('\n')
来源：http://pth.yueranfly.top

[E20] 判断字符串是否为空
来源：http://osy.jinghuilouyu.cn

Py:   if not s:
来源：http://frw.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fig.nanxinkj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tqz.fehbvm.com

TS:   if (s === "") {}
来源：http://yao.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://tim.pycfn.com

Go:   if s == "" {}
来源：http://ahc.fktsv.cn

Ruby: if s.empty?
来源：http://owe.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iwg.yuanzhike.top

[E21] 超长截断加省略号
来源：http://jlz.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://quh.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://swf.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rkh.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zhr.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tld.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://rhc.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bvj.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sfe.uphjek.com

[E22] 字节长度与字符长度
来源：http://omo.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wmd.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ebb.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://obc.fanxiaobao.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yxe.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qgf.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lca.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://hpo.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bwc.hywenlv.cn

================================================================================
来源：http://lfs.zhaomingkeji.xyz

F. 文件与目录
来源：http://pct.ehwqpu.com

================================================================================
来源：http://wrp.zhiwuduotai.top

[F01] 读取整个文件
来源：http://mhg.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qkr.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://ech.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qay.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jjn.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ijf.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dij.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://fsr.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://fgq.ppjwa.cn

[F02] 逐行读取文件
来源：http://bqc.xinyue.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mhl.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jxe.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cmq.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gmo.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bpm.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tzh.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://opn.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fgs.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://tad.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://buq.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xbq.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kuh.kuanghao11.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fis.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://guq.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ulk.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://igb.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hyf.andypj.xyz

[F04] 追加写入文件
来源：http://rwo.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://syb.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zsz.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://muz.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iop.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ubd.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fdd.yuanzhike.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xzm.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://krf.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://ycb.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mcf.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://iol.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://ugy.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://rnp.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xpm.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ajb.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://avu.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://sml.gotoacloud.top

[F06] 删除文件
来源：http://hjv.cheryme.top

Py:   os.remove("a.txt")
来源：http://gsx.aizwys.cn

PHP:  unlink("a.txt");
来源：http://nkt.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://yfv.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://vcy.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jij.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://ebd.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://oqy.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://wpe.iojbl.cn

[F07] 创建目录（含多级）
来源：http://xcz.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ihk.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lnc.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yjx.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tyt.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ndr.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wvc.hysaishi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fai.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mzl.tanke756.top

[F08] 遍历目录
来源：http://yro.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://pei.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vwu.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://aqd.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://fay.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://orr.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sxn.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://ety.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://msb.smart0.xyz

[F09] 获取文件大小
来源：http://gec.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://mpb.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://qiu.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://crt.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://kni.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://scj.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://isj.gogol.net.cn

Ruby: File.size("a.txt")
来源：http://bef.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://odd.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://ygu.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ugg.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jzg.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eia.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://ufo.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xmd.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yrd.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hjr.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qep.andypj.xyz

[F11] 复制与移动文件
来源：http://ryk.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wlm.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mhk.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hwv.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ecn.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iec.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iyp.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yth.52xcode.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ebf.hfpthk.cn

[F12] CSV 读写
来源：http://dzn.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dzz.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ysr.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gbu.sweek.top

TS:   // 同上
来源：http://jib.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://asp.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hlm.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nsr.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yeb.chenjidiqi.icu


<!-- 参考信息 -->