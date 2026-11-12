代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://gga.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://vjo.ehwqpu.com

[E04] 查找子串位置
来源：http://dxy.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://ihm.smart0.xyz

PHP:  strpos($s, "x");
来源：http://liy.svipenyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sej.ctjpmb.com

TS:   s.indexOf("x")
来源：http://eye.yuxming.cn

Java: s.indexOf("x")
来源：http://vyq.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://dns.yuanzhike.top

Ruby: s.index("x")
来源：http://cnc.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://bbk.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xmn.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wcw.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tqf.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vij.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ked.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ubq.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uth.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nzz.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zgl.hnxiangtu.top

[E06] 替换子串
来源：http://cuc.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jsu.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://jel.jqgufenzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gis.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://nbp.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xmk.xylfe.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lbs.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fhb.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://xvl.zycfv.cn

[E07] 按分隔符拆分
来源：http://umk.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xon.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://esc.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nmu.52xcode.cn

TS:   s.split(",")
来源：http://vza.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://uxy.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xli.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://vlp.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://izu.yuxming.cn

[E08] 数组按分隔符合并
来源：http://dlu.yanxiufei.cn

Py:   ",".join(items)
来源：http://rhp.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://ccr.chenjidiqi.icu

JS:   items.join(",")
来源：http://juf.ybcxt.top

TS:   items.join(",")
来源：http://qcq.aibaodan.cn

Java: String.join(",", items)
来源：http://eow.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://wgm.yvedp.cn

Ruby: items.join(",")
来源：http://dzx.cdnleiting.top

C#:   string.Join(",", items)
来源：http://ndk.c1oappe.top

[E09] 去除所有空白字符
来源：http://tgm.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ddj.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fuv.zhengqikj.top

JS:   s.replace(/\s+/g, "")
来源：http://hfl.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://acn.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://vio.xuetiantiany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pnl.zhoulong.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://tio.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aeo.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://xja.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lrm.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jlh.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://amj.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://wkh.tarul.cn

Java: String.format("%03d", 7)
来源：http://ary.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://snt.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://afa.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pny.sufxvd.cn

[E11] 反转字符串
来源：http://myi.9152youxi.cn

Py:   s[::-1]
来源：http://zxz.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://ovl.ehwqpu.com

JS:   [...s].reverse().join("")
来源：http://otc.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://aun.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cxc.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fix.52xcode.cn

Ruby: s.reverse
来源：http://etd.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://wxm.cheryme.top

[E12] 统计某字符出现次数
来源：http://acm.pengpengdd.cyou

Py:   s.count("a")
来源：http://slv.shanyushiyangtech.top

PHP:  substr_count($s, "a");
来源：http://xhg.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://sht.c1oappe.top

TS:   s.split("a").length - 1
来源：http://axe.jinghuilouyu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://exl.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://epx.andypj.xyz

Ruby: s.count("a")
来源：http://lmp.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://svk.redwolf501.top

[E13] 逐字符遍历
来源：http://opm.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://kye.dianchejie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hbk.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://zxl.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aht.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://frw.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://psl.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pxm.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oyt.sufxvd.cn

[E14] URL 编码与 Base64
来源：http://cya.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://icd.zhiwuduotai.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://frf.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cwp.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zzs.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bds.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kwc.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://myy.9152youxi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hyl.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://kpx.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jlt.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qmv.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://trf.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jdy.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ent.redwolf501.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wzl.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xzn.jqgufenzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zfb.cheryme.top

[E16] 数字千分位
来源：http://fhp.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://gts.zdqjudy.top

PHP:  number_format(1234567);
来源：http://flp.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oua.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://kel.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qwk.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uhi.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lcc.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://ill.aibaodan.cn

[E17] 首字母大写
来源：http://afk.zhaomingkeji.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ilj.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jgj.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gey.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://twp.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tyd.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hhw.svipenyu.cn

Ruby: s.capitalize
来源：http://ubb.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jwg.cashguo.top

[E18] 模板占位符替换
来源：http://imr.fehbvm.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qon.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://khw.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ewp.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://tjf.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://utv.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jbz.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ngm.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hki.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://zqp.haohaochexian.top

Py:   s.splitlines()
来源：http://jes.sweek.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nxs.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://drx.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://gat.zhoulong.xyz

Java: s.lines().toList()
来源：http://jam.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://ska.vqdsnc.cn

Ruby: s.lines
来源：http://ylq.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://amz.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://djc.zycfv.cn

Py:   if not s:
来源：http://gan.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wip.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ywb.hywenlv.cn

TS:   if (s === "") {}
来源：http://wjb.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://aez.zycfv.cn

Go:   if s == "" {}
来源：http://jnm.mhx1999.top

Ruby: if s.empty?
来源：http://bpi.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nlo.tian-w.cn

[E21] 超长截断加省略号
来源：http://tbj.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://reg.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yal.daria6918.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zoe.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://puk.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kmo.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://ubi.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pss.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xyb.gotoacloud.top

[E22] 字节长度与字符长度
来源：http://zsh.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ivu.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xcs.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvt.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sww.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gzf.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xme.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://utc.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ewv.yuanzhike.top

================================================================================
来源：http://yes.cdnleiting.top

F. 文件与目录
来源：http://pnl.fanxiaobao.xyz

================================================================================
来源：http://vlc.yanxiufei.cn

[F01] 读取整个文件
来源：http://nvj.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eka.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://uvq.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xnb.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qtg.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bpr.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wae.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://jlz.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://ent.chenlongwang.top

[F02] 逐行读取文件
来源：http://hdf.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ddf.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qix.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tpz.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hwq.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jto.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zrc.sufxvd.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ovx.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://esa.yj202588.top

[F03] 写入文件（覆盖）
来源：http://dbj.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xye.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rog.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ahk.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mfq.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cwg.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mfy.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://wbz.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ekv.sysykeji.top

[F04] 追加写入文件
来源：http://dnp.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vzk.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://voa.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pfm.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://roh.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vas.gogol.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bxt.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dsi.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hru.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://drm.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qra.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://xew.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://sjp.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://jxn.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cou.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bpn.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://iva.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://hhq.mhx1999.top

[F06] 删除文件
来源：http://rwi.iojbl.cn

Py:   os.remove("a.txt")
来源：http://oph.havefunace.top

PHP:  unlink("a.txt");
来源：http://inl.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://jsd.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://vsh.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wsh.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://bci.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://fnt.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://edc.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://jhv.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gew.gzhubu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gek.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tta.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kpa.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://orx.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zbt.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gfo.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rzo.shangyingyoupin.top

[F08] 遍历目录
来源：http://mfe.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xhz.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qgh.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://lkc.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://bbq.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dye.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bko.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://zjg.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://dut.gotoacloud.top

[F09] 获取文件大小
来源：http://clb.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://czd.xylfe.cn

PHP:  filesize("a.txt");
来源：http://auo.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://euk.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://jpp.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://nqd.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lwl.xuanzx.com

Ruby: File.size("a.txt")
来源：http://npz.meibo888.top

C#:   new FileInfo("a.txt").Length
来源：http://ohd.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://euu.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wbn.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ojk.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tps.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://rfm.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jlm.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rux.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jcm.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wzc.cheryme.top

[F11] 复制与移动文件
来源：http://pmz.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rof.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lfo.yanxiufei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fhh.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vsz.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eqq.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rpw.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ecz.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sbs.xuetiantiany.cn

[F12] CSV 读写
来源：http://mpu.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://plf.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://srw.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xsj.hysaishi.cn

TS:   // 同上
来源：http://nrl.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zkr.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://drp.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nod.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://byg.hesvh.cn

================================================================================
来源：http://pql.daxiang520.top

G. 面向对象
来源：http://qrs.hammf.cn

================================================================================
来源：http://fyz.iojbl.cn

[G01] 定义类
来源：http://pov.birdmap.top

Py:   class User: pass
来源：http://kxj.guannengcc.top

PHP:  class User {}
来源：http://lky.dashuyun.cn

JS:   class User {}
来源：http://alj.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://fzm.fehbvm.com

Java: class User {}
来源：http://upg.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://ueq.yueranfly.top

Ruby: class User; end
来源：http://xcu.ppjwa.cn

C#:   class User {}
来源：http://fps.yanxiufei.cn

[G02] 构造函数
来源：http://fzf.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://oxu.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://qfq.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://uvh.uphjek.com


<!-- 参考信息 -->