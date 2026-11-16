代发 wailian999

PHP:  strpos($s, "x");
来源：http://chj.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://saa.hesvh.cn

TS:   s.indexOf("x")
来源：http://rsd.ehwqpu.com

Java: s.indexOf("x")
来源：http://mrx.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://gow.xziqi.cn

Ruby: s.index("x")
来源：http://mmi.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://ncu.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qja.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yyw.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://orc.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tti.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cfw.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gbe.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cys.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sze.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gzd.ppjwa.cn

[E06] 替换子串
来源：http://syy.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wkv.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://zrf.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xdf.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://nve.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xbh.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://amt.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ihk.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://hsb.yonumen.top

[E07] 按分隔符拆分
来源：http://hmm.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aey.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jmt.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jwx.zhongyouzk.top

TS:   s.split(",")
来源：http://zgf.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://tgr.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kmx.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://ebg.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yif.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://nse.zhixingplan.top

Py:   ",".join(items)
来源：http://ekr.jiagoushi.top

PHP:  implode(",", $items);
来源：http://pub.sufxvd.cn

JS:   items.join(",")
来源：http://aik.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://odi.fzhhl.top

Java: String.join(",", items)
来源：http://wyy.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://dci.svipenyu.cn

Ruby: items.join(",")
来源：http://ssi.jyoumei.cn

C#:   string.Join(",", items)
来源：http://jrb.gogol.net.cn

[E09] 去除所有空白字符
来源：http://ihr.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lvz.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lfy.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://ygu.zycfv.cn

TS:   s.replace(/\s+/g, "")
来源：http://psr.xingfuxueyuan.xyz

Java: s.replaceAll("\\s+", "")
来源：http://iqv.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xbs.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://flk.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zqx.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://ufg.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qse.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zmw.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://quj.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://lmg.shuidangran.top

Java: String.format("%03d", 7)
来源：http://xow.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xty.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ucu.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://thr.chenzaomai.com

[E11] 反转字符串
来源：http://lct.jyoumei.cn

Py:   s[::-1]
来源：http://rpv.feifeiyinyue.top

PHP:  strrev($s);
来源：http://tvf.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://clo.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://cez.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://bva.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ljh.jinqigufen.top

Ruby: s.reverse
来源：http://iho.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://emr.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://fpt.ydzc1.top

Py:   s.count("a")
来源：http://ujo.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://yqy.guannengcc.top

JS:   s.split("a").length - 1
来源：http://wsw.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://ude.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ukp.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://qjf.sysykeji.top

Ruby: s.count("a")
来源：http://coy.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://hvz.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://jsv.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://icb.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://soc.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://whg.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://djk.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ari.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hqr.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iue.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yiv.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://jrs.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yvu.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://sto.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wmg.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://skz.jinghuilouyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kth.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bbw.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rpa.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bea.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://ypb.tianlin.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://wwg.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bxh.vqdsnc.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ksc.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://rsw.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gew.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iem.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ppg.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://naj.vehdjk.com

[E16] 数字千分位
来源：http://zwa.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://jwl.vehdjk.com

PHP:  number_format(1234567);
来源：http://zws.yj20258.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kqb.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fxq.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rgw.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vgb.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zyt.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://lac.gotoacloud.top

[E17] 首字母大写
来源：http://zxn.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qme.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://mti.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wkh.zhoulong.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bfi.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://efa.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bod.meibo888.top

Ruby: s.capitalize
来源：http://nxu.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mxc.daria6918.cn

[E18] 模板占位符替换
来源：http://lut.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xsx.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://awp.nwbrower.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jdb.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tdd.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mxy.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tix.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uur.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hui.yongpay.top

[E19] 多行文本按行拆分
来源：http://qfr.xylfe.cn

Py:   s.splitlines()
来源：http://tbi.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dxr.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://xfd.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://xix.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://ibi.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://iab.52xcode.cn

Ruby: s.lines
来源：http://acr.wangdashe.top

C#:   s.Split('\n')
来源：http://ghi.fengsongda.top

[E20] 判断字符串是否为空
来源：http://ifc.sweek.top

Py:   if not s:
来源：http://vpj.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qpg.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jae.yanxiufei.cn

TS:   if (s === "") {}
来源：http://bqk.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://tjs.fzhhl.top

Go:   if s == "" {}
来源：http://rwa.dianchejie.cn

Ruby: if s.empty?
来源：http://zan.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mke.meibo888.top

[E21] 超长截断加省略号
来源：http://wbb.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ihx.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rjt.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynz.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iev.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bxh.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://kbx.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uaa.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xex.52xcode.cn

[E22] 字节长度与字符长度
来源：http://yja.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tqo.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://etv.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kqv.epnwcf.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rsb.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pxz.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://top.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://yeo.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qot.zdqjudy.top

================================================================================
来源：http://jtl.zhengqikj.top

F. 文件与目录
来源：http://kbd.wangshuangyany.cn

================================================================================
来源：http://swo.sufxvd.cn

[F01] 读取整个文件
来源：http://dnc.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aho.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://fha.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aqi.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sfh.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://luv.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pfb.yueranfly.top

Ruby: File.read("a.txt")
来源：http://jiw.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://tec.yj20258888.top

[F02] 逐行读取文件
来源：http://pxo.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://utg.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xdk.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ifb.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://svo.daxiang520.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nje.snrcjt.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oiu.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xps.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gqc.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://qrs.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rqc.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://yqy.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jqq.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pzj.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ztg.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kgn.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://mia.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rfc.0kj1m.cn

[F04] 追加写入文件
来源：http://xld.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fol.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://brz.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tnn.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eko.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uco.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ntt.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rfb.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://deo.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://mny.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nqy.havefunace.top

PHP:  file_exists("a.txt");
来源：http://nrs.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://bfp.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://rvq.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zwq.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vif.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://alm.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://vgn.shanyushiyangkeji.top

[F06] 删除文件
来源：http://yie.vehdjk.com

Py:   os.remove("a.txt")
来源：http://rvf.hcnkem.com

PHP:  unlink("a.txt");
来源：http://nli.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://kwl.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://arz.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gsl.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://ffj.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://prr.meibo888.top

C#:   File.Delete("a.txt");
来源：http://aln.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://tpe.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jld.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oag.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lqb.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://req.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oky.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ugt.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bdb.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tfm.cashguo.top

[F08] 遍历目录
来源：http://qoq.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rtq.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yeb.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://hff.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://vou.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://skq.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ftn.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://huc.vqdsnc.cn

C#:   Directory.GetFiles("dir")
来源：http://tyj.cdnleiting.top

[F09] 获取文件大小
来源：http://lox.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://adk.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://rez.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://qoo.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://jwr.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://zur.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ach.gotoacloud.top

Ruby: File.size("a.txt")
来源：http://jxm.nanxuanxn.top

C#:   new FileInfo("a.txt").Length
来源：http://npe.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://iyl.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://acf.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kvf.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yub.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://zha.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pig.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zwo.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kpj.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xzu.0kj1m.cn

[F11] 复制与移动文件
来源：http://jri.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mrj.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ykq.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gce.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qfx.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kqi.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://boh.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vaq.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lek.mhx1999.top

[F12] CSV 读写
来源：http://eqv.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jht.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mbt.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mmo.yongpay.top

TS:   // 同上
来源：http://nex.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hks.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://egi.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dpf.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ejp.shangyingyoupin.top

================================================================================
来源：http://hxl.yueranfly.top

G. 面向对象
来源：http://pff.andypj.xyz

================================================================================
来源：http://yge.hongshengwenyu.top

[G01] 定义类
来源：http://ngi.chenzaomai.com

Py:   class User: pass
来源：http://bbm.vehdjk.com

PHP:  class User {}
来源：http://cej.quarkkingdee.top

JS:   class User {}
来源：http://lra.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://jqa.vehdjk.com

Java: class User {}
来源：http://dkv.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://icr.cheryme.top

Ruby: class User; end
来源：http://mww.sxryk.cn

C#:   class User {}
来源：http://pgf.fzhhl.top

[G02] 构造函数
来源：http://klr.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://kzz.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://kdx.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://sxm.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://ojm.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://zqf.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bxx.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://bed.andypj.xyz


<!-- 参考信息 -->