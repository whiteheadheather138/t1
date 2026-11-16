代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://enh.hnqzz.top

[E03] 截取子串
来源：http://kon.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vrz.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vif.316326.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://skk.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://fxo.cashguo.top

Java: s.substring(1, 4)
来源：http://czs.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ydl.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://url.fanxiaobao.xyz

C#:   s.Substring(1, 3)
来源：http://uph.jianghu66.top

[E04] 查找子串位置
来源：http://rok.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://rrh.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://qfm.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xkg.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://dxf.chenzaomai.com

Java: s.indexOf("x")
来源：http://jpl.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://ojv.epnwcf.com

Ruby: s.index("x")
来源：http://vwg.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://wjd.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xty.xinyue.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://irf.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nsc.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iou.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tac.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wzj.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ltn.chenzaomai.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wrf.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://imz.sufxvd.cn

[E06] 替换子串
来源：http://vez.cqqwz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qsy.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://brv.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oli.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://rlv.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dsm.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bti.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bdc.yj202588.top

C#:   s.Replace("a", "b")
来源：http://ojm.ctjpmb.com

[E07] 按分隔符拆分
来源：http://ycp.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aai.shanyushiyangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ahp.iojbl.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pjs.cheryme.top

TS:   s.split(",")
来源：http://exr.yangfankeji.com

Java: s.split(",");  s.split("\\s+")
来源：http://klh.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cma.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://iql.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eqd.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://jvl.tarul.cn

Py:   ",".join(items)
来源：http://smf.yuxming.cn

PHP:  implode(",", $items);
来源：http://cxe.yvedp.cn

JS:   items.join(",")
来源：http://jja.nwbrower.top

TS:   items.join(",")
来源：http://xpa.svipenyu.cn

Java: String.join(",", items)
来源：http://dfn.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://hph.yangfankeji.com

Ruby: items.join(",")
来源：http://pbc.ctjpmb.com

C#:   string.Join(",", items)
来源：http://etg.sysykeji.top

[E09] 去除所有空白字符
来源：http://mhq.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vha.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hzy.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://zwn.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://rdm.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://rkb.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ehl.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://get.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://urq.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://oov.fehbvm.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qpq.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ypk.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://ols.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://kyy.aizwys.cn

Java: String.format("%03d", 7)
来源：http://wbb.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nre.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://svn.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://her.xuetiantiany.cn

[E11] 反转字符串
来源：http://fft.xylfe.cn

Py:   s[::-1]
来源：http://cur.cashguo.top

PHP:  strrev($s);
来源：http://mtx.birdmap.top

JS:   [...s].reverse().join("")
来源：http://mbl.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://alt.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kgx.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://znd.yuxming.cn

Ruby: s.reverse
来源：http://rpr.fktsv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xts.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://lia.hywenlv.cn

Py:   s.count("a")
来源：http://tky.316326.xyz

PHP:  substr_count($s, "a");
来源：http://qff.guannengcc.top

JS:   s.split("a").length - 1
来源：http://xrh.tarul.cn

TS:   s.split("a").length - 1
来源：http://jxa.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ivl.tarul.cn

Go:   strings.Count(s, "a")
来源：http://dmp.aizwys.cn

Ruby: s.count("a")
来源：http://btn.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://kro.gaohongyu789.top

[E13] 逐字符遍历
来源：http://tli.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://gjj.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pmb.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://atb.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jre.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fty.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lwb.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://tcn.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xem.uphjek.com

[E14] URL 编码与 Base64
来源：http://vxb.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gfb.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ews.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wtk.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dvr.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uwt.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yhq.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ipu.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ywc.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://nqt.mhx1999.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pmq.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ipj.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gpb.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wcn.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vmf.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wxi.jqgufenzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dzq.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cow.zhijiandao.cn

[E16] 数字千分位
来源：http://ory.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://glr.sweek.top

PHP:  number_format(1234567);
来源：http://aca.tianlin.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ghq.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://svm.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kao.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://txc.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tcb.iojbl.cn

C#:   1234567.ToString("N0")
来源：http://qcn.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://hie.yj20258.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://epx.ivvv.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ksa.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hga.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gag.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fjc.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://arq.yuxming.cn

Ruby: s.capitalize
来源：http://jhk.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rqq.guannengcc.top

[E18] 模板占位符替换
来源：http://iro.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kdw.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zll.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://vzr.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://auu.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qup.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rnt.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dxt.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wxt.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://bkk.nwbrower.top

Py:   s.splitlines()
来源：http://rls.xylfe.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hwb.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://vww.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://jda.jinqigufen.top

Java: s.lines().toList()
来源：http://fmq.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://ctw.zhiwuduotai.top

Ruby: s.lines
来源：http://kgh.shuidangran.top

C#:   s.Split('\n')
来源：http://wpx.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://khj.cashguo.top

Py:   if not s:
来源：http://hil.zhoulong.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oij.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oxv.vqdsnc.cn

TS:   if (s === "") {}
来源：http://zsa.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://wmd.yvedp.cn

Go:   if s == "" {}
来源：http://dfr.andypj.xyz

Ruby: if s.empty?
来源：http://iin.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dai.yj20258.top

[E21] 超长截断加省略号
来源：http://swg.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dhj.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jpu.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fof.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gjo.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wrz.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://kxz.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zxx.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hyl.xinyue.icu

[E22] 字节长度与字符长度
来源：http://jaa.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tek.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pos.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hdq.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://asu.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yqd.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ivn.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://vzo.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yzv.ehwqpu.com

================================================================================
来源：http://zlb.hammf.cn

F. 文件与目录
来源：http://usx.tianlin.xyz

================================================================================
来源：http://ojt.yueranfly.top

[F01] 读取整个文件
来源：http://lvw.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mnx.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://afv.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zuk.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wcc.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vad.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wug.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://ihe.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://fbv.nanxuanxn.top

[F02] 逐行读取文件
来源：http://cyk.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://moa.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://skv.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://scs.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tib.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ysp.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pvn.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ocv.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://csm.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://sil.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://scq.ydzc1.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vcx.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ofa.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://udt.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://txg.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kge.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://eoz.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oko.cdnleiting.top

[F04] 追加写入文件
来源：http://tjc.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ywl.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nkk.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://axl.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eri.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kxr.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tws.xziqi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kgp.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nki.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://cak.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dlg.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://ztu.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://iqx.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://yon.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://flx.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ezs.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://qxn.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://fxc.snrcjt.cn

[F06] 删除文件
来源：http://ypt.zhijiandao.cn

Py:   os.remove("a.txt")
来源：http://ndh.gzhubu.top

PHP:  unlink("a.txt");
来源：http://syq.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hxw.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://dcc.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://npz.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://ypy.meibo888.top

Ruby: File.delete("a.txt")
来源：http://xpg.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://bgw.xuanzx.com

[F07] 创建目录（含多级）
来源：http://nwi.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://brl.sufxvd.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hia.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pur.redwolf501.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bgf.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gmh.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xux.gotoacloud.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nej.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qji.9152youxi.cn

[F08] 遍历目录
来源：http://osh.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://lai.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://inf.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://bef.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://jvn.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://prc.zhoulong.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://xeh.yuxming.cn

Ruby: Dir.children("dir")
来源：http://mwp.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://znx.daxiang520.top

[F09] 获取文件大小
来源：http://hxx.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://sub.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://npg.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://sxy.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://vtr.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dvr.ywan-chungtsiang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xjq.bjfxy.top

Ruby: File.size("a.txt")
来源：http://knt.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://bcl.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://epv.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://stg.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ohp.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aev.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://wfl.yanxiufei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jzk.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vnp.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dox.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jpc.gaohongyu789.top

[F11] 复制与移动文件
来源：http://nrv.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://npt.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pqa.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qdj.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bjv.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xxx.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://owt.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wae.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lmw.nanxuanxn.top

[F12] CSV 读写
来源：http://rjv.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jej.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gec.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://imx.jiagoushi.top

TS:   // 同上
来源：http://ael.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zpg.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zje.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lxt.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://zci.yj202588.top

================================================================================
来源：http://egq.yj202588.top

G. 面向对象
来源：http://soy.zhixingplan.top

================================================================================
来源：http://osq.wangdashe.top

[G01] 定义类
来源：http://iit.nwbrower.top

Py:   class User: pass
来源：http://jud.birdmap.top

PHP:  class User {}
来源：http://jyo.hnqzz.top

JS:   class User {}
来源：http://jab.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://vds.tanke756.top


<!-- 参考信息 -->