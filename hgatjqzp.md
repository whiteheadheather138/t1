代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xjw.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://qir.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://diz.vqdsnc.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tpf.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://qev.yueranfly.top

C#:   s.Substring(1, 3)
来源：http://kxj.fehbvm.com

[E04] 查找子串位置
来源：http://rtf.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://hlh.vehdjk.com

PHP:  strpos($s, "x");
来源：http://sgy.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jcy.xylfe.cn

TS:   s.indexOf("x")
来源：http://zkb.daria6918.cn

Java: s.indexOf("x")
来源：http://jhu.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://adq.cashguo.top

Ruby: s.index("x")
来源：http://qwm.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://czk.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://epp.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pui.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kfo.chenzaomai.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://anc.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://pcz.birdmap.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://abx.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lww.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jzo.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://thk.sysykeji.top

[E06] 替换子串
来源：http://hrk.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qcu.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://thd.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yng.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://gbp.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cke.yj202588.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://njw.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mif.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://pxq.tarul.cn

[E07] 按分隔符拆分
来源：http://gks.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tnz.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sos.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yre.shangyingyoupin.top

TS:   s.split(",")
来源：http://cux.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://fdc.daria6918.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jyi.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://jav.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yuz.mhx1999.top

[E08] 数组按分隔符合并
来源：http://ruh.daxiang520.top

Py:   ",".join(items)
来源：http://uuo.yj20258.top

PHP:  implode(",", $items);
来源：http://ajj.zhengqikj.top

JS:   items.join(",")
来源：http://vsa.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://nxu.yangfankeji.com

Java: String.join(",", items)
来源：http://jet.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://hcs.zycfv.cn

Ruby: items.join(",")
来源：http://hwq.9152youxi.cn

C#:   string.Join(",", items)
来源：http://agl.havefunace.top

[E09] 去除所有空白字符
来源：http://qmn.xylfe.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pgr.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kqj.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://ddn.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://iac.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://zwg.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://jcw.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pik.nanxuanxn.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fai.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://xmv.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rbe.dianchejie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://djn.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://tnd.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://mvw.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://dlf.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yad.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://okz.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://biz.yj20258.top

[E11] 反转字符串
来源：http://hye.tarul.cn

Py:   s[::-1]
来源：http://drx.guowangkeji.top

PHP:  strrev($s);
来源：http://mmw.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://ehj.hammf.cn

TS:   [...s].reverse().join("")
来源：http://auv.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bbn.chenzaomai.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ekc.ppjwa.cn

Ruby: s.reverse
来源：http://uqs.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://inp.hnqzz.top

[E12] 统计某字符出现次数
来源：http://mwj.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://fxf.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://wxe.fzhhl.top

JS:   s.split("a").length - 1
来源：http://ayy.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://ceh.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://plg.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://uhm.cdnleiting.top

Ruby: s.count("a")
来源：http://qkd.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://eys.daxiang520.top

[E13] 逐字符遍历
来源：http://nnq.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://iws.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hae.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ssb.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ylm.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sgb.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tkd.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zfa.9152youxi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ras.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://eyc.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bye.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ayc.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sft.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zlx.shuidangran.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cld.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xoo.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tvu.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dri.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://hyo.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://zlt.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://skd.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eel.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qvp.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vjg.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zoo.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jmu.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kqd.jlsjyb.cn

[E16] 数字千分位
来源：http://eba.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://qaf.52xcode.cn

PHP:  number_format(1234567);
来源：http://lby.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ohu.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bxe.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hsg.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vfc.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aig.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://uhu.zhengqikj.top

[E17] 首字母大写
来源：http://yeu.hongshengwenyu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tao.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://uye.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cvv.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://laj.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tmk.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mvr.9152youxi.cn

Ruby: s.capitalize
来源：http://rgy.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://drq.jyoumei.cn

[E18] 模板占位符替换
来源：http://ukt.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iuh.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://brn.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qhc.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fjl.yongpay.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://alw.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gwg.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eps.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zgh.yonumen.top

[E19] 多行文本按行拆分
来源：http://ldz.xuanzx.com

Py:   s.splitlines()
来源：http://gwr.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pxy.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://ijc.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://vvd.c1oappe.top

Java: s.lines().toList()
来源：http://ihg.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://etq.andypj.xyz

Ruby: s.lines
来源：http://uul.tanke756.top

C#:   s.Split('\n')
来源：http://iov.c1oappe.top

[E20] 判断字符串是否为空
来源：http://kld.9152youxi.cn

Py:   if not s:
来源：http://vbv.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jmn.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fgy.tanke756.top

TS:   if (s === "") {}
来源：http://iws.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://zbl.zdbjq.cn

Go:   if s == "" {}
来源：http://fbz.sysykeji.top

Ruby: if s.empty?
来源：http://fyz.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://waz.gotoacloud.top

[E21] 超长截断加省略号
来源：http://ndl.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ebs.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rpj.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qrp.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://msy.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hbq.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://xhx.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://htr.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qqt.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://lgj.zhixingplan.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vlc.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://esl.jinqigfzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mna.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wwg.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wil.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gyp.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://wsq.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uea.jqgfzy.top

================================================================================
来源：http://cmt.svipenyu.cn

F. 文件与目录
来源：http://hhm.0kj1m.cn

================================================================================
来源：http://kyc.zhijiandao.cn

[F01] 读取整个文件
来源：http://xwu.bjfxy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fop.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://yyn.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bpw.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://slw.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fmk.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ltv.52xcode.cn

Ruby: File.read("a.txt")
来源：http://bzn.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ljp.jianghu66.top

[F02] 逐行读取文件
来源：http://lmh.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wup.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ncm.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mlr.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qye.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cbv.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://klb.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mba.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://npv.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://rdq.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pyr.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nbw.wangdashe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ehd.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://inb.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nze.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cho.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://wud.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://olh.ctjpmb.com

[F04] 追加写入文件
来源：http://lfq.cucudq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://emy.nwbrower.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mht.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jtv.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dpy.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lfj.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gkb.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ccq.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yky.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://zpg.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kga.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://lgd.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://ngd.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://ulb.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lcg.sysykeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bpo.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://wjv.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://rou.hnxiangtu.top

[F06] 删除文件
来源：http://olo.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://sdd.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://kxg.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://chj.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://pvk.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jmh.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://wsu.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://brr.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://qly.gzhubu.top

[F07] 创建目录（含多级）
来源：http://deb.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gzl.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rvk.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://byg.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qzp.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hmk.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://udp.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yuc.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dtj.316326.xyz

[F08] 遍历目录
来源：http://hbo.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://sac.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yrb.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://ath.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://vwv.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vyi.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://flv.ybcxt.top

Ruby: Dir.children("dir")
来源：http://rvy.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://gel.zdbjq.cn

[F09] 获取文件大小
来源：http://ync.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://kcn.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://lzr.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://ruv.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://ndk.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://uuy.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dac.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://oko.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://cry.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://dpr.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://axp.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aao.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tzz.shuidangran.top

TS:   path.extname("a.txt")
来源：http://kgk.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ynq.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fxb.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xva.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ktp.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://jmr.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ahr.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://znc.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rgz.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dpk.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://llh.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gpz.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tvg.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pwo.pengpengdd.cyou

[F12] CSV 读写
来源：http://bmj.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tnz.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xpg.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://urh.sufxvd.cn

TS:   // 同上
来源：http://wdc.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dvq.quarkkingdee.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fwr.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://otl.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nkg.yj202588.top

================================================================================
来源：http://oec.hongshengwenyu.top

G. 面向对象
来源：http://aqh.jqgufenzy.top

================================================================================
来源：http://rsk.svipenyu.cn

[G01] 定义类
来源：http://bix.quarkkingdee.top

Py:   class User: pass
来源：http://vac.gogol.net.cn

PHP:  class User {}
来源：http://gei.cheryme.top

JS:   class User {}
来源：http://boz.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://qln.tian-w.cn

Java: class User {}
来源：http://yjy.gogol.net.cn

Go:   type User struct { Name string }
来源：http://xuq.fktsv.cn

Ruby: class User; end
来源：http://fct.redwolf501.top

C#:   class User {}
来源：http://ikd.fzhhl.top


<!-- 参考信息 -->