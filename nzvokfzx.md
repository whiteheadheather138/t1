代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://icm.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://veo.wangdashe.top

[E04] 查找子串位置
来源：http://yck.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://cjp.yj202588.top

PHP:  strpos($s, "x");
来源：http://rqn.52xcode.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nlr.aibaodan.cn

TS:   s.indexOf("x")
来源：http://pck.zdqjudy.top

Java: s.indexOf("x")
来源：http://cpk.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://nkh.daria6918.cn

Ruby: s.index("x")
来源：http://kop.yongpay.top

C#:   s.IndexOf("x")
来源：http://lcx.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://lvg.hfpthk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lnz.svipenyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://icb.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jqv.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ohp.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://szm.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://spx.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cxm.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://frj.guowangkeji.top

[E06] 替换子串
来源：http://wfc.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kpy.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://qiu.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wai.ydjk.org.cn

TS:   s.replaceAll("a", "b")
来源：http://onx.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wks.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xbh.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ggn.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://esx.nwbrower.top

[E07] 按分隔符拆分
来源：http://xna.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xjr.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jkb.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rlz.chenjidiqi.icu

TS:   s.split(",")
来源：http://kdm.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://obt.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mdd.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://zip.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fun.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://wnh.birdmap.top

Py:   ",".join(items)
来源：http://eda.c1oappe.top

PHP:  implode(",", $items);
来源：http://zjs.ctjpmb.com

JS:   items.join(",")
来源：http://bww.ybcxt.top

TS:   items.join(",")
来源：http://esg.bjfxy.top

Java: String.join(",", items)
来源：http://erp.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://cfg.guowangkeji.top

Ruby: items.join(",")
来源：http://lpd.fktsv.cn

C#:   string.Join(",", items)
来源：http://gxv.9152youxi.cn

[E09] 去除所有空白字符
来源：http://oal.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mff.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aej.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://mbf.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://cpb.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://uua.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://gtu.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://sco.cqqwz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qha.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://wct.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tpa.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ndq.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://tat.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://gti.yongpay.top

Java: String.format("%03d", 7)
来源：http://hwk.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uga.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rff.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qwg.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://uig.yueranfly.top

Py:   s[::-1]
来源：http://bey.ydjk.org.cn

PHP:  strrev($s);
来源：http://yaa.meibo888.top

JS:   [...s].reverse().join("")
来源：http://drt.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://hah.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mrw.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pzy.jinqigfzy.top

Ruby: s.reverse
来源：http://ddh.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://eyw.zhixingplan.top

[E12] 统计某字符出现次数
来源：http://yiu.guowangkeji.top

Py:   s.count("a")
来源：http://fia.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://eud.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://aim.aizwys.cn

TS:   s.split("a").length - 1
来源：http://aaz.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blb.havefunace.top

Go:   strings.Count(s, "a")
来源：http://usj.wangshuangyany.cn

Ruby: s.count("a")
来源：http://uam.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://lmi.ctjpmb.com

[E13] 逐字符遍历
来源：http://nzz.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://ynt.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yzq.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tno.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://aig.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xxs.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zgp.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://icf.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cpc.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://ssv.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nth.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sdx.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cqv.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lof.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mqu.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://udt.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bin.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ufq.zhaomingkeji.xyz

[E15] HTML 转义 / 反转义
来源：http://ind.andypj.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://xwr.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aoo.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fna.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://psr.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zum.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jas.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ijf.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ofo.redwolf501.top

[E16] 数字千分位
来源：http://rfd.sxryk.cn

Py:   f"{1234567:,}"
来源：http://rfz.vehdjk.com

PHP:  number_format(1234567);
来源：http://awh.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lgq.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://tuv.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fhr.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://epk.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qcl.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://utu.meibo888.top

[E17] 首字母大写
来源：http://psa.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://scx.ivvv.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tko.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://axd.gotoacloud.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aab.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mcf.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rir.wangdashe.top

Ruby: s.capitalize
来源：http://mcp.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://igr.9152youxi.cn

[E18] 模板占位符替换
来源：http://gxh.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://naf.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bpp.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mhi.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://smg.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ggt.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xva.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ubu.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rtt.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://rgu.epnwcf.com

Py:   s.splitlines()
来源：http://svq.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eup.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://zzt.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://ljf.wangdashe.top

Java: s.lines().toList()
来源：http://opa.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://jkd.zhongyouzk.top

Ruby: s.lines
来源：http://bqb.gogol.net.cn

C#:   s.Split('\n')
来源：http://bfh.yuxming.cn

[E20] 判断字符串是否为空
来源：http://tcz.guannengcc.top

Py:   if not s:
来源：http://xdb.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cpy.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tcx.svipenyu.cn

TS:   if (s === "") {}
来源：http://bbf.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://kmo.feifeiyinyue.top

Go:   if s == "" {}
来源：http://ljv.jinqigfzy.top

Ruby: if s.empty?
来源：http://rsn.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qma.hfpthk.cn

[E21] 超长截断加省略号
来源：http://pvo.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tkk.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rsj.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qye.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://koz.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uqw.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://kwa.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cud.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qhx.vehdjk.com

[E22] 字节长度与字符长度
来源：http://mhh.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ydw.yongpay.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iel.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yja.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nzz.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xpy.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lou.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://ijd.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zbo.hammf.cn

================================================================================
来源：http://qyn.ehwqpu.com

F. 文件与目录
来源：http://uzb.birdmap.top

================================================================================
来源：http://sfe.gotoacloud.top

[F01] 读取整个文件
来源：http://dci.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://txs.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://kku.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bwu.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cku.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vvf.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ise.birdmap.top

Ruby: File.read("a.txt")
来源：http://pmw.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://ufn.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://fig.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lkm.jinqigufen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lxt.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://soj.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eey.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ivb.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gsp.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://spw.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mgd.cashguo.top

[F03] 写入文件（覆盖）
来源：http://luh.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gvz.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vzz.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sja.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vjo.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ivq.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xih.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://xoj.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jjn.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://tre.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wzw.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zut.316326.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gdb.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vfb.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ehb.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pmb.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mew.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dcj.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://gvi.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yqf.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://xku.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://sbb.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://tma.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jgn.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mbl.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://lbg.aibaodan.cn

C#:   File.Exists("a.txt")
来源：http://fjz.tarul.cn

[F06] 删除文件
来源：http://hyh.yongpay.top

Py:   os.remove("a.txt")
来源：http://vzc.fengsongda.top

PHP:  unlink("a.txt");
来源：http://iyu.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://ymh.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://gil.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dek.yonumen.top

Go:   os.Remove("a.txt")
来源：http://kem.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://wxn.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://pdg.cdnleiting.top

[F07] 创建目录（含多级）
来源：http://wtd.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://voo.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ruo.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rzv.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gqf.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gmo.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uir.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ucc.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zda.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://kxb.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cfu.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://puz.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://aiu.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://zpr.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jmg.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tff.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://bjx.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://qhw.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://qog.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://oon.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://rnw.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://tnz.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://wad.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://iii.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qqn.hnqzz.top

Ruby: File.size("a.txt")
来源：http://qjy.zhiwuduotai.top

C#:   new FileInfo("a.txt").Length
来源：http://ute.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ihi.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ask.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pxw.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nfh.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://uoz.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ivd.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bhu.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://snh.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mdp.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://uwk.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pjq.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uwr.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hic.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nlc.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://enw.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qjh.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tov.xziqi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qco.uphjek.com

[F12] CSV 读写
来源：http://gmb.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fxa.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bls.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://evz.jinqigfzy.top

TS:   // 同上
来源：http://qij.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fum.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rzi.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hqs.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://udv.iojbl.cn

================================================================================
来源：http://qux.yfazqb.com

G. 面向对象
来源：http://sys.jiagoushi.top

================================================================================
来源：http://dny.bbcook.cn

[G01] 定义类
来源：http://dvm.sufxvd.cn

Py:   class User: pass
来源：http://dsw.pengpengdd.cyou

PHP:  class User {}
来源：http://bgb.redwolf501.top

JS:   class User {}
来源：http://jvi.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://hzz.hywenlv.cn

Java: class User {}
来源：http://xtd.gogol.net.cn

Go:   type User struct { Name string }
来源：http://tkn.andypj.xyz

Ruby: class User; end
来源：http://zrm.zhoulong.xyz

C#:   class User {}
来源：http://qia.sweek.top

[G02] 构造函数
来源：http://wzj.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://imd.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://ear.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://eaz.jqgufenzy.top


<!-- 参考信息 -->