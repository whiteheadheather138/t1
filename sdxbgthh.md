代发 wailian999

[E02] 重复字符串
来源：http://jkv.0kj1m.cn

Py:   "ab" * 3
来源：http://ias.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://kxl.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://hfg.cashguo.top

TS:   "ab".repeat(3)
来源：http://uvp.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://gan.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://mvq.zdqjudy.top

Ruby: "ab" * 3
来源：http://szl.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://okg.kuanghao11.cn

[E03] 截取子串
来源：http://auk.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wcg.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kdb.snrcjt.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nhq.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://tes.zhixingplan.top

Java: s.substring(1, 4)
来源：http://gyb.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hkk.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://jkh.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://jyt.hnxiangtu.top

[E04] 查找子串位置
来源：http://nbp.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://aju.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://svl.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uey.jiagoushi.top

TS:   s.indexOf("x")
来源：http://ksv.jianghu66.top

Java: s.indexOf("x")
来源：http://onv.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://qxy.tianlin.xyz

Ruby: s.index("x")
来源：http://wwc.shuidangran.top

C#:   s.IndexOf("x")
来源：http://jog.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://vti.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yrj.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://msr.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jwk.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://ywf.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gwn.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hgn.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ces.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://joo.ydjk.org.cn

[E06] 替换子串
来源：http://ihn.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lqc.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://yzq.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bbj.xinyue.icu

TS:   s.replaceAll("a", "b")
来源：http://wsw.guowangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kjc.havefunace.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ygu.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fzn.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://mye.yongpay.top

[E07] 按分隔符拆分
来源：http://pvs.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rzp.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://upw.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://oyg.guowangkeji.top

TS:   s.split(",")
来源：http://ama.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://onh.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xwr.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://kni.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://krl.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://fat.jinqigfzy.top

Py:   ",".join(items)
来源：http://vjz.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://oji.shangyingyoupin.top

JS:   items.join(",")
来源：http://kxo.chenjidiqi.icu

TS:   items.join(",")
来源：http://lns.ivvv.top

Java: String.join(",", items)
来源：http://jfs.shuidangran.top

Go:   strings.Join(items, ",")
来源：http://mxn.kuanghao11.cn

Ruby: items.join(",")
来源：http://cjy.redwolf501.top

C#:   string.Join(",", items)
来源：http://lsh.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://ovy.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wwe.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tgf.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://nae.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://vwq.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://ekf.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://icr.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://tnr.fengsongda.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bvg.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://hif.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kmp.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fxs.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://gun.hammf.cn

TS:   "7".padStart(3, "0")
来源：http://hjv.aizwys.cn

Java: String.format("%03d", 7)
来源：http://ivk.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://flw.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pre.ctjpmb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xxn.jinqigufen.top

[E11] 反转字符串
来源：http://oza.jyoumei.cn

Py:   s[::-1]
来源：http://itm.cdnleiting.top

PHP:  strrev($s);
来源：http://roz.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://icq.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://tcd.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://uqv.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xeu.zhiwuduotai.top

Ruby: s.reverse
来源：http://zog.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://zwh.birdmap.top

[E12] 统计某字符出现次数
来源：http://apw.pycfn.com

Py:   s.count("a")
来源：http://jka.sweek.top

PHP:  substr_count($s, "a");
来源：http://lez.shuidangran.top

JS:   s.split("a").length - 1
来源：http://qgz.vehdjk.com

TS:   s.split("a").length - 1
来源：http://nri.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://htt.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://eui.nwbrower.top

Ruby: s.count("a")
来源：http://eup.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://qzd.epnwcf.com

[E13] 逐字符遍历
来源：http://exo.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://ecd.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vps.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mxv.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://dyx.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gur.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yjn.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nkz.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://txd.smart0.xyz

[E14] URL 编码与 Base64
来源：http://crz.fengsongda.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wud.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jpy.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kbc.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dvo.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tyl.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nog.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uds.gaohongyu789.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yla.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://gsd.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://tmc.yuanzhike.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lby.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kff.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dlt.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oul.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aag.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qtn.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yjy.daria6918.cn

[E16] 数字千分位
来源：http://rme.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://fxq.52xcode.cn

PHP:  number_format(1234567);
来源：http://qbc.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jtl.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://krj.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xli.guowangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gpb.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://srv.pengpengdd.cyou

C#:   1234567.ToString("N0")
来源：http://pez.jianghu66.top

[E17] 首字母大写
来源：http://bwi.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gfa.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wzy.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dbm.yanxiufei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xjp.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://spv.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://anf.meibo888.top

Ruby: s.capitalize
来源：http://tsq.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vpz.0kj1m.cn

[E18] 模板占位符替换
来源：http://osw.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://riz.birdmap.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://saf.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ebs.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://eit.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ehw.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wpm.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ltx.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fog.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://eyp.hywenlv.cn

Py:   s.splitlines()
来源：http://mrf.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ihc.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://pau.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://thi.fehbvm.com

Java: s.lines().toList()
来源：http://dea.hywenlv.cn

Go:   strings.Split(s, "\n")
来源：http://yha.ivvv.top

Ruby: s.lines
来源：http://upl.gotoacloud.top

C#:   s.Split('\n')
来源：http://nop.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://nsu.jyoumei.cn

Py:   if not s:
来源：http://mah.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qza.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hsk.sysykeji.top

TS:   if (s === "") {}
来源：http://xqs.fzhhl.top

Java: if (s.isEmpty()) {}
来源：http://okt.meibo888.top

Go:   if s == "" {}
来源：http://qaa.yj20258888.top

Ruby: if s.empty?
来源：http://tks.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zej.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://nsu.wangshuangyany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nya.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wry.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aci.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://usg.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dhn.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://ooe.jyoumei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nkj.hnqzz.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qub.sweek.top

[E22] 字节长度与字符长度
来源：http://kvv.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gnc.ydjk.org.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eig.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mjx.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fte.zhiwuduotai.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://brf.xuetiantiany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://psj.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://aji.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rtm.hammf.cn

================================================================================
来源：http://wct.316326.xyz

F. 文件与目录
来源：http://gby.dianchejie.cn

================================================================================
来源：http://jxm.fzhhl.top

[F01] 读取整个文件
来源：http://yyk.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oge.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://fsf.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://emf.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xdd.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mof.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://usu.birdmap.top

Ruby: File.read("a.txt")
来源：http://isg.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://yls.pycfn.com

[F02] 逐行读取文件
来源：http://bft.jinqigufen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bwx.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gby.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jjh.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xxk.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ogb.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zak.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kuq.yj20258.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bdt.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://nws.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gry.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jhn.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gtu.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wqq.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://csl.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rra.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://tjg.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vxx.pycfn.com

[F04] 追加写入文件
来源：http://rsu.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xjf.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wuy.ivvv.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kjf.epnwcf.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lzg.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gaq.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sph.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aps.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pgy.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://sfg.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nio.nanxinkj.top

PHP:  file_exists("a.txt");
来源：http://gcw.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://yif.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://bhf.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ivb.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uze.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://rlg.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://trk.sysykeji.top

[F06] 删除文件
来源：http://ckv.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://lbt.nanxuanxn.top

PHP:  unlink("a.txt");
来源：http://vzp.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://aal.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://ywm.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tqa.uphjek.com

Go:   os.Remove("a.txt")
来源：http://blp.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://nhw.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://rmc.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://epw.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ipj.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fxc.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://itr.gaohongyu789.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gqp.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yhj.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ebq.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gfx.yongpay.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mik.guowangkeji.top

[F08] 遍历目录
来源：http://fgj.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nnh.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kbe.gogol.net.cn

JS:   fs.readdirSync("dir")
来源：http://jso.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://bsg.nanxinkj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://moj.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ewt.birdmap.top

Ruby: Dir.children("dir")
来源：http://diw.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://vmm.gaohongyu789.top

[F09] 获取文件大小
来源：http://udg.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://ocq.hesvh.cn

PHP:  filesize("a.txt");
来源：http://tei.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://ovi.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://xrn.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://vcw.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uyv.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://ebh.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://mvo.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ylz.gotoacloud.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dsh.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://knx.zycfv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fgt.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://ine.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zbf.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vju.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hyg.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fmn.yuxming.cn

[F11] 复制与移动文件
来源：http://mwr.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://izi.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jep.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wre.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bhm.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fuc.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pjm.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://acv.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qsn.chenzaomai.com

[F12] CSV 读写
来源：http://duf.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vyv.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ozc.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://muv.fanxiaobao.xyz

TS:   // 同上
来源：http://wts.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yuj.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oeo.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pns.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hkp.jinqigfzy.top


<!-- 参考信息 -->