代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cxh.havefunace.top

TS:   s.slice(1, 4)
来源：http://rhp.cdnleiting.top

Java: s.substring(1, 4)
来源：http://cxj.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mlz.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://jop.316326.xyz

C#:   s.Substring(1, 3)
来源：http://htj.xziqi.cn

[E04] 查找子串位置
来源：http://nez.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://hpe.xuetiantiany.cn

PHP:  strpos($s, "x");
来源：http://yqc.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ivg.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://amo.yfazqb.com

Java: s.indexOf("x")
来源：http://jck.yonumen.top

Go:   strings.Index(s, "x")
来源：http://kyy.9152youxi.cn

Ruby: s.index("x")
来源：http://tif.nwbrower.top

C#:   s.IndexOf("x")
来源：http://qel.hongshengwenyu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iwn.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eyy.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://axe.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://imx.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://swb.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mqq.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://six.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cvi.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qlj.aizwys.cn

[E06] 替换子串
来源：http://poj.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bko.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://zgh.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dtf.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://cue.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://soe.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rgx.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ycg.uphjek.com

C#:   s.Replace("a", "b")
来源：http://hcl.guannengcc.top

[E07] 按分隔符拆分
来源：http://vmk.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vst.sjlbkw.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fgl.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pwc.hammf.cn

TS:   s.split(",")
来源：http://caa.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://oyu.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ziz.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://iyl.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ngl.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://rmu.chenjidiqi.icu

Py:   ",".join(items)
来源：http://cuj.yuxming.cn

PHP:  implode(",", $items);
来源：http://niq.chenjidiqi.icu

JS:   items.join(",")
来源：http://tds.yfazqb.com

TS:   items.join(",")
来源：http://ure.hcnkem.com

Java: String.join(",", items)
来源：http://zdx.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://fjj.zhixingplan.top

Ruby: items.join(",")
来源：http://alh.yj202588.top

C#:   string.Join(",", items)
来源：http://qvc.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://eyr.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bnt.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jqw.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://mqe.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://qdb.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://hfg.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://imy.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://kci.shangyingyoupin.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://von.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://ild.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bwd.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vlt.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://ilk.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://ulh.shuidangran.top

Java: String.format("%03d", 7)
来源：http://xmn.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://otu.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ylq.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ouf.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://vpv.mhx1999.top

Py:   s[::-1]
来源：http://kwn.jinghuilouyu.cn

PHP:  strrev($s);
来源：http://xva.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://hzq.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://zsd.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zgs.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nei.hesvh.cn

Ruby: s.reverse
来源：http://omh.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://can.uphjek.com

[E12] 统计某字符出现次数
来源：http://iqp.hywenlv.cn

Py:   s.count("a")
来源：http://vjv.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://hwh.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://nbt.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://vpp.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hpd.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://wqj.chenzaomai.com

Ruby: s.count("a")
来源：http://fbr.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://kyk.jyoumei.cn

[E13] 逐字符遍历
来源：http://dcf.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://omr.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jof.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uyy.tarul.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aue.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dit.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bpv.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://euk.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dzq.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://oxb.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uct.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ath.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lvg.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://evo.bbcook.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hve.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kqc.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ucl.zhiwuduotai.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://spj.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://fmx.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jvf.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jsj.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://guw.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://voe.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hau.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bux.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rdc.wangshuangyany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nhu.jinghuilouyu.cn

[E16] 数字千分位
来源：http://isg.fengsongda.top

Py:   f"{1234567:,}"
来源：http://uyb.pycfn.com

PHP:  number_format(1234567);
来源：http://kbk.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://okm.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qry.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cbp.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fao.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wqv.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://dnq.hywenlv.cn

[E17] 首字母大写
来源：http://pag.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xht.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://xmx.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bfw.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oet.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://llp.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://spg.yvedp.cn

Ruby: s.capitalize
来源：http://alc.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lgr.aizwys.cn

[E18] 模板占位符替换
来源：http://fas.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fgd.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gbj.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oja.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://enq.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fdj.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xvn.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tte.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eyl.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://kym.zhengqikj.top

Py:   s.splitlines()
来源：http://zqc.hcnkem.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://anc.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://map.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://bya.yvedp.cn

Java: s.lines().toList()
来源：http://sxz.sxryk.cn

Go:   strings.Split(s, "\n")
来源：http://zpx.ybcxt.top

Ruby: s.lines
来源：http://tsx.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://iwg.sxryk.cn

[E20] 判断字符串是否为空
来源：http://jab.dianchejie.cn

Py:   if not s:
来源：http://los.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jkp.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mvk.xylfe.cn

TS:   if (s === "") {}
来源：http://zdg.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://bsa.smart0.xyz

Go:   if s == "" {}
来源：http://qfo.tanke756.top

Ruby: if s.empty?
来源：http://gnx.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://srl.aizwys.cn

[E21] 超长截断加省略号
来源：http://xsk.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kwe.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sko.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ryv.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ifd.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fzs.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://enk.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ipq.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lsl.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://txh.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xla.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tpu.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nxt.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cdo.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rkt.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xld.hywenlv.cn

Ruby: s.bytesize;  s.length
来源：http://xhb.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uol.bbcook.cn

================================================================================
来源：http://iki.hnxiangtu.top

F. 文件与目录
来源：http://qbr.jinqigufen.top

================================================================================
来源：http://qan.cheryme.top

[F01] 读取整个文件
来源：http://iby.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dpe.xuetiantiany.cn

PHP:  file_get_contents("a.txt");
来源：http://awg.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fbw.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qrv.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://csq.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://evd.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://zpo.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://nzv.ybcxt.top

[F02] 逐行读取文件
来源：http://coh.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://csk.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ele.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kml.daria6918.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rqf.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://byn.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bsh.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cfl.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lor.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://bwv.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://syr.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pmi.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bal.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pwp.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ryw.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dhf.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://die.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ufx.wangdashe.top

[F04] 追加写入文件
来源：http://bos.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cpo.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vyn.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ycc.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xsh.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rpg.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cyu.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wcs.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dar.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://cjt.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eth.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://lyc.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://lgp.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://zrf.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://njv.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://leh.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://gjt.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://iyj.tanke756.top

[F06] 删除文件
来源：http://jaq.316326.xyz

Py:   os.remove("a.txt")
来源：http://skp.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://ygb.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rbm.shanyushiyangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://dfc.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lkj.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://ano.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://uaj.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://owu.aizwys.cn

[F07] 创建目录（含多级）
来源：http://zdk.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bmb.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mum.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ova.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tdj.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yml.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cip.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ugn.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ged.ydjk.org.cn

[F08] 遍历目录
来源：http://ocd.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cpr.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://upa.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://lbt.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://fsj.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://njz.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://utn.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://dcp.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://vfj.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://uvk.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://nbn.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://snq.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://klb.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://dwt.epnwcf.com

Java: Files.size(Path.of("a.txt"))
来源：http://etq.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oze.hammf.cn

Ruby: File.size("a.txt")
来源：http://idf.jiagoushi.top

C#:   new FileInfo("a.txt").Length
来源：http://dfy.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://xjd.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gsu.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jdj.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vgo.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://pqo.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wld.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://csk.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pky.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pxa.zdbjq.cn

[F11] 复制与移动文件
来源：http://qgm.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sgc.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://clr.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bjb.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wvf.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dev.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gos.tarul.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rao.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lih.gotoacloud.top

[F12] CSV 读写
来源：http://cvm.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gzo.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ttw.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dgv.gogol.net.cn

TS:   // 同上
来源：http://cws.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pji.epnwcf.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lfb.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yeb.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://wiu.dashuyun.cn

================================================================================
来源：http://zcl.zhijiandao.cn

G. 面向对象
来源：http://yer.zhaomingkeji.xyz

================================================================================
来源：http://zyk.xuanzx.com

[G01] 定义类
来源：http://cle.yueranfly.top

Py:   class User: pass
来源：http://ywt.aibaodan.cn

PHP:  class User {}
来源：http://ntg.cheryme.top

JS:   class User {}
来源：http://hfh.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://tcu.ywan-chungtsiang.top

Java: class User {}
来源：http://wlv.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://bgm.pycfn.com

Ruby: class User; end
来源：http://fnk.sysykeji.top

C#:   class User {}
来源：http://sqo.xingfuxueyuan.xyz


<!-- 参考信息 -->