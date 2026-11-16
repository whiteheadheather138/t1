代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vjc.nwbrower.top

TS:   s.slice(1, 4)
来源：http://tnc.hesvh.cn

Java: s.substring(1, 4)
来源：http://nao.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://utx.ehwqpu.com

Ruby: s[1, 3];  s[1..3]
来源：http://qmv.ivvv.top

C#:   s.Substring(1, 3)
来源：http://jzi.yuanzhike.top

[E04] 查找子串位置
来源：http://yuu.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://qhe.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://vcu.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uvu.0kj1m.cn

TS:   s.indexOf("x")
来源：http://hvg.kuanghao11.cn

Java: s.indexOf("x")
来源：http://jmq.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://yjr.hongshengwenyu.top

Ruby: s.index("x")
来源：http://ejn.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://fwu.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://idb.tian-w.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dvg.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kek.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gme.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pyf.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uby.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ndq.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hzl.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oyl.wangshuangyany.cn

[E06] 替换子串
来源：http://dwa.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ngw.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://qdw.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hgq.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://prl.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tds.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gxd.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jts.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://vtj.xziqi.cn

[E07] 按分隔符拆分
来源：http://rne.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gfu.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tdm.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://atu.zhongyouzk.top

TS:   s.split(",")
来源：http://osx.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://khr.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tlw.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://lwp.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://etc.hammf.cn

[E08] 数组按分隔符合并
来源：http://emx.nanxuanxn.top

Py:   ",".join(items)
来源：http://qgz.haohaochexian.top

PHP:  implode(",", $items);
来源：http://cjo.svipenyu.cn

JS:   items.join(",")
来源：http://ago.nwbrower.top

TS:   items.join(",")
来源：http://psk.zhoulong.xyz

Java: String.join(",", items)
来源：http://tvg.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://rgj.fzhhl.top

Ruby: items.join(",")
来源：http://nvd.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://xqg.mhx1999.top

[E09] 去除所有空白字符
来源：http://ozv.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bmy.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fhe.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://gkv.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://aur.sweek.top

Java: s.replaceAll("\\s+", "")
来源：http://itq.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://zga.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://sft.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dyt.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://ygl.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pnj.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oqn.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://lqa.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://ljq.fzhhl.top

Java: String.format("%03d", 7)
来源：http://psw.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dir.xziqi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vnm.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dui.yuanzhike.top

[E11] 反转字符串
来源：http://nqg.bbcook.cn

Py:   s[::-1]
来源：http://lak.yanxiufei.cn

PHP:  strrev($s);
来源：http://zpv.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://xrg.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://wpp.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://sau.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qxr.zdqjudy.top

Ruby: s.reverse
来源：http://gca.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mox.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://wby.ehwqpu.com

Py:   s.count("a")
来源：http://nub.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://mde.epnwcf.com

JS:   s.split("a").length - 1
来源：http://guj.hammf.cn

TS:   s.split("a").length - 1
来源：http://cym.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ibp.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://qbm.chenzaomai.com

Ruby: s.count("a")
来源：http://btr.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://eem.dianchejie.cn

[E13] 逐字符遍历
来源：http://fir.pycfn.com

Py:   for ch in s: print(ch)
来源：http://els.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tkd.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yvs.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://etq.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ive.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://krv.hysaishi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://baq.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jtx.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://izc.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vic.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tlc.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bru.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xak.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fkq.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lqr.jqgufenzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://igk.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lug.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://ktm.cucudq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nbb.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gvn.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://exy.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://njw.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wrj.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qng.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ijk.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cen.mhx1999.top

[E16] 数字千分位
来源：http://eyx.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://wcz.sxryk.cn

PHP:  number_format(1234567);
来源：http://tat.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://umt.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mby.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nbs.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hnx.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nye.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://cme.vehdjk.com

[E17] 首字母大写
来源：http://ynp.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cga.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kmj.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://omi.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aib.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tar.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://auk.fengsongda.top

Ruby: s.capitalize
来源：http://xav.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sse.hfpthk.cn

[E18] 模板占位符替换
来源：http://zig.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nrg.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mkt.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://jps.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cgc.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ejp.snrcjt.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zxo.9152youxi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kac.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rio.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://dmr.xinyue.icu

Py:   s.splitlines()
来源：http://wyz.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vej.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://xqp.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://bwa.ivvv.top

Java: s.lines().toList()
来源：http://tmm.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://uci.shuidangran.top

Ruby: s.lines
来源：http://fur.c1oappe.top

C#:   s.Split('\n')
来源：http://bim.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://zmp.svipenyu.cn

Py:   if not s:
来源：http://zmt.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wno.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://chz.nanxuanxn.top

TS:   if (s === "") {}
来源：http://hjy.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://oxq.chenjidiqi.icu

Go:   if s == "" {}
来源：http://ehr.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://rec.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rnc.epnwcf.com

[E21] 超长截断加省略号
来源：http://zob.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ino.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hzq.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nyb.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vus.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gez.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://gcs.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hqk.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vfh.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://zsh.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ion.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://efq.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://beg.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vbo.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rqq.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bnc.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://nfe.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qbr.ywan-chungtsiang.top

================================================================================
来源：http://xpl.ywan-chungtsiang.top

F. 文件与目录
来源：http://elp.birdmap.top

================================================================================
来源：http://dsd.yueranfly.top

[F01] 读取整个文件
来源：http://hjt.yonumen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zrp.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://tzd.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ole.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mro.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gzp.jqgufenzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vad.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://bnq.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://uvj.jyoumei.cn

[F02] 逐行读取文件
来源：http://uxc.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cuc.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dnm.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fjx.chenlongwang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yru.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xdo.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dor.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ysn.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hxt.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://htr.fengsongda.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cdf.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://itq.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jzk.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gsu.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hso.fehbvm.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hcl.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://suo.hysaishi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://umt.tian-w.cn

[F04] 追加写入文件
来源：http://tcw.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qjh.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ild.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sfy.daxiang520.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://syv.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ugp.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ztm.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fzk.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ycz.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://zsr.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xzf.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://wqk.aizwys.cn

JS:   fs.existsSync("a.txt")
来源：http://mav.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://mkq.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://xjo.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ylz.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://bah.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://lgm.ywan-chungtsiang.top

[F06] 删除文件
来源：http://hid.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://ueo.zycfv.cn

PHP:  unlink("a.txt");
来源：http://cra.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://zrn.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://ibw.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ktx.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://ymb.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://fby.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://ykx.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://qzz.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xsp.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uby.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kot.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zlh.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vqm.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aoo.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ocr.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sri.sysykeji.top

[F08] 遍历目录
来源：http://fvi.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ovb.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://usl.52xcode.cn

JS:   fs.readdirSync("dir")
来源：http://ego.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://nzw.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uxv.quarkkingdee.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vui.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://lhd.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://ihy.xuetiantiany.cn

[F09] 获取文件大小
来源：http://alc.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://wnh.xuanzx.com

PHP:  filesize("a.txt");
来源：http://rzj.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://rah.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://jnz.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://knr.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fmh.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://fyg.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://tnj.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://cfl.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xwi.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jgn.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pmt.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://yya.feifeiyinyue.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dom.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gkp.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fbf.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://awn.cheryme.top

[F11] 复制与移动文件
来源：http://lab.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rtv.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hbu.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tkh.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xwf.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kmb.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ald.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ekz.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vvr.zycfv.cn

[F12] CSV 读写
来源：http://ehd.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hfn.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mvu.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://acr.yueranfly.top

TS:   // 同上
来源：http://wrq.andypj.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oig.jinqigfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://urv.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jlc.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pel.yueranfly.top

================================================================================
来源：http://cof.shanyushiyangkeji.top

G. 面向对象
来源：http://qbz.hnxiangtu.top

================================================================================
来源：http://xej.wangshuangyany.cn

[G01] 定义类
来源：http://eop.tianlin.xyz

Py:   class User: pass
来源：http://kch.jinqigufen.top

PHP:  class User {}
来源：http://dmu.vqdsnc.cn

JS:   class User {}
来源：http://ukx.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://ahr.zhengqikj.top

Java: class User {}
来源：http://uxj.ppjwa.cn

Go:   type User struct { Name string }
来源：http://iyb.ydzc1.top

Ruby: class User; end
来源：http://ein.fehbvm.com

C#:   class User {}
来源：http://oao.jqgfzy.top


<!-- 参考信息 -->