代发 wailian999

PHP:  strpos($s, "x");
来源：http://uee.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rrk.epnwcf.com

TS:   s.indexOf("x")
来源：http://yvx.uphjek.com

Java: s.indexOf("x")
来源：http://dao.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://xby.tarul.cn

Ruby: s.index("x")
来源：http://txz.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://khx.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zqm.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bto.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xkd.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ehs.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://eqe.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dxg.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rtl.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dgx.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://god.zhijiandao.cn

[E06] 替换子串
来源：http://won.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gne.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://tkq.pycfn.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ahc.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://kyg.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://goo.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://joh.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jbn.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://ojm.hfpthk.cn

[E07] 按分隔符拆分
来源：http://lca.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sga.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uvn.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gap.9152youxi.cn

TS:   s.split(",")
来源：http://amp.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://tta.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dzt.cheryme.top

Ruby: s.split(",");  s.split
来源：http://bwc.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jms.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://wdw.ppjwa.cn

Py:   ",".join(items)
来源：http://kax.52xcode.cn

PHP:  implode(",", $items);
来源：http://guu.zdqjudy.top

JS:   items.join(",")
来源：http://ptl.hongshengwenyu.top

TS:   items.join(",")
来源：http://sis.yangfankeji.com

Java: String.join(",", items)
来源：http://yzs.sweek.top

Go:   strings.Join(items, ",")
来源：http://wxi.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://qxp.havefunace.top

C#:   string.Join(",", items)
来源：http://njb.gotoacloud.top

[E09] 去除所有空白字符
来源：http://qui.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bsv.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kfm.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://ygc.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://qjz.aibaodan.cn

Java: s.replaceAll("\\s+", "")
来源：http://xbo.ehwqpu.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://jti.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://xhm.haohaochexian.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ldt.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://sas.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wws.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://obl.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://eww.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://jyl.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://xeo.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pia.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kde.yuxming.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hvd.cheryme.top

[E11] 反转字符串
来源：http://xio.jinqigfzy.top

Py:   s[::-1]
来源：http://kjw.jyoumei.cn

PHP:  strrev($s);
来源：http://yrq.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://fpc.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://rix.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ovf.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rwb.mhx1999.top

Ruby: s.reverse
来源：http://mxc.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://lkk.sysykeji.top

[E12] 统计某字符出现次数
来源：http://bku.ehwqpu.com

Py:   s.count("a")
来源：http://rar.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://ryl.tarul.cn

JS:   s.split("a").length - 1
来源：http://jpp.meibo888.top

TS:   s.split("a").length - 1
来源：http://xex.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://awo.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://wkr.xinyue.icu

Ruby: s.count("a")
来源：http://azc.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://ieo.cqqwz.cn

[E13] 逐字符遍历
来源：http://yjn.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://kop.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://slj.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://iwx.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zeq.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kwa.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gtx.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://vib.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://muy.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://isg.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lki.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rvo.shanyushiyangtech.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xlc.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xvv.xziqi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ajm.hammf.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mei.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vga.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wrv.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://qxr.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fnt.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uqz.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vfn.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zof.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ncx.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iyb.feifeiyinyue.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hpa.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lvj.0kj1m.cn

[E16] 数字千分位
来源：http://aed.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://inw.shuidangran.top

PHP:  number_format(1234567);
来源：http://qcb.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://wms.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tvn.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gum.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zgd.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blw.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://gdt.snrcjt.cn

[E17] 首字母大写
来源：http://lne.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bqs.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kum.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jst.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ood.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ifn.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hta.yj20258.top

Ruby: s.capitalize
来源：http://fry.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ijl.havefunace.top

[E18] 模板占位符替换
来源：http://rng.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://toy.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fep.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yhb.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://epg.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sww.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xys.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://szg.yj20258888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zil.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://rxf.cdnleiting.top

Py:   s.splitlines()
来源：http://gab.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sdr.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://omr.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://qsh.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://snq.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://dit.meibo888.top

Ruby: s.lines
来源：http://yus.ctjpmb.com

C#:   s.Split('\n')
来源：http://apb.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://nko.tian-w.cn

Py:   if not s:
来源：http://jaz.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ink.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eam.ctjpmb.com

TS:   if (s === "") {}
来源：http://buy.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://dtw.hnqzz.top

Go:   if s == "" {}
来源：http://ycn.bjfxy.top

Ruby: if s.empty?
来源：http://fuv.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fgc.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://hvy.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pij.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://huz.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tqj.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ouy.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uht.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://fks.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ysj.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://del.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://zlw.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fso.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tlc.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gmu.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uku.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wxl.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eou.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://jkq.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kfp.daxiang520.top

================================================================================
来源：http://aky.aizwys.cn

F. 文件与目录
来源：http://dtd.meibo888.top

================================================================================
来源：http://esw.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://nhl.yonumen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wwz.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://dis.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fez.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ton.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yay.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vhs.hcnkem.com

Ruby: File.read("a.txt")
来源：http://nnd.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://szv.zhijiandao.cn

[F02] 逐行读取文件
来源：http://ffm.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jzi.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iow.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lqa.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bqs.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lyi.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zuf.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://flk.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iga.cashguo.top

[F03] 写入文件（覆盖）
来源：http://oqs.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ipr.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ghp.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kko.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bgz.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yvg.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ukx.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://stw.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://swq.xuetiantiany.cn

[F04] 追加写入文件
来源：http://edj.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gaw.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fcf.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://txy.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dpq.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dag.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tcm.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pxr.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rpn.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://jzq.nwbrower.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fnr.yonumen.top

PHP:  file_exists("a.txt");
来源：http://hda.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://wxw.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://vdo.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uwt.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hxy.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://jge.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://oyk.nanxinkj.top

[F06] 删除文件
来源：http://hbk.birdmap.top

Py:   os.remove("a.txt")
来源：http://bpc.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://yll.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jhc.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kle.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yxb.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://qba.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://nmq.yonumen.top

C#:   File.Delete("a.txt");
来源：http://krl.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://zkg.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dkn.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://znd.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxo.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nut.316326.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mjr.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aor.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://muk.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ntr.cqqwz.cn

[F08] 遍历目录
来源：http://tzj.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pod.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ten.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://bcb.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://jcl.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lbu.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mvk.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://jba.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://okh.yj20258888.top

[F09] 获取文件大小
来源：http://cys.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://you.tanke756.top

PHP:  filesize("a.txt");
来源：http://bqc.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://pkq.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://xqn.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://psp.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lxd.daria6918.cn

Ruby: File.size("a.txt")
来源：http://sbu.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://dhc.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://fjv.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bij.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vuo.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hig.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://ivz.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jef.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bdp.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dor.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pxk.gzhubu.top

[F11] 复制与移动文件
来源：http://zbi.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ipc.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lpw.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://teo.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eej.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nie.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ute.jianghu66.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jar.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pwp.zhaomingkeji.xyz

[F12] CSV 读写
来源：http://hxm.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tii.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uqh.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mks.sxryk.cn

TS:   // 同上
来源：http://lri.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hau.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hsw.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kwm.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://rwj.ywan-chungtsiang.top

================================================================================
来源：http://xis.hammf.cn

G. 面向对象
来源：http://wil.nanxuanxn.top

================================================================================
来源：http://agh.dianchejie.cn

[G01] 定义类
来源：http://thv.9152youxi.cn

Py:   class User: pass
来源：http://oge.chenlongwang.top

PHP:  class User {}
来源：http://gye.jlsjyb.cn

JS:   class User {}
来源：http://vss.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://zgj.mhx1999.top

Java: class User {}
来源：http://klr.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://heh.sjlbkw.cn

Ruby: class User; end
来源：http://onl.zhoulong.xyz

C#:   class User {}
来源：http://hsv.daxiang520.top

[G02] 构造函数
来源：http://bdx.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://qod.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://wnq.yfazqb.com

JS:   constructor(name) { this.name = name; }
来源：http://efq.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://pdw.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://gvg.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qwi.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://zce.sxryk.cn


<!-- 参考信息 -->