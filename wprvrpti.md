代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jmu.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vnc.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gum.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lfj.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sda.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dit.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ysr.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://arc.shanyushiyangkeji.top

[E06] 替换子串
来源：http://oky.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zlh.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://ais.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dss.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://gmc.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://knp.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vvc.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://syd.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://huo.tanke756.top

[E07] 按分隔符拆分
来源：http://cwd.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gap.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rij.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fej.yuanzhike.top

TS:   s.split(",")
来源：http://dzk.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zzn.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bri.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://qbf.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zzt.xziqi.cn

[E08] 数组按分隔符合并
来源：http://xmd.ydzc1.top

Py:   ",".join(items)
来源：http://tcx.mhx1999.top

PHP:  implode(",", $items);
来源：http://gvs.jqgufenzy.top

JS:   items.join(",")
来源：http://brj.shanyushiyangtech.top

TS:   items.join(",")
来源：http://rtu.daxiang520.top

Java: String.join(",", items)
来源：http://riz.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://vme.guannengcc.top

Ruby: items.join(",")
来源：http://rfr.cdnleiting.top

C#:   string.Join(",", items)
来源：http://zvf.yangfankeji.com

[E09] 去除所有空白字符
来源：http://oyg.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bfd.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dxa.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://ubo.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://fqq.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://irl.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dpw.iojbl.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lcl.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yle.hnqzz.top

[E10] 左侧补零 / 定长填充
来源：http://nwu.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gso.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://utw.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://mzj.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://fmg.andypj.xyz

Java: String.format("%03d", 7)
来源：http://gjk.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cij.xziqi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jkz.zhengqikj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kdj.daria6918.cn

[E11] 反转字符串
来源：http://jyu.wangshuangyany.cn

Py:   s[::-1]
来源：http://bml.zhoulong.xyz

PHP:  strrev($s);
来源：http://tod.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://zor.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://bsb.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ybm.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ufj.jinghuilouyu.cn

Ruby: s.reverse
来源：http://ydh.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://pwx.gzhubu.top

[E12] 统计某字符出现次数
来源：http://wia.andypj.xyz

Py:   s.count("a")
来源：http://woa.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://kci.52xcode.cn

JS:   s.split("a").length - 1
来源：http://otf.guannengcc.top

TS:   s.split("a").length - 1
来源：http://wzb.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ivs.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://eni.sysykeji.top

Ruby: s.count("a")
来源：http://kfq.chenjidiqi.icu

C#:   s.Count(c => c == 'a')
来源：http://aea.mhx1999.top

[E13] 逐字符遍历
来源：http://sym.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://qpj.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hci.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://dgt.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gbz.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lws.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mgj.shuidangran.top

Ruby: s.each_char { |ch| puts ch }
来源：http://usb.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://knx.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://fha.ybcxt.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kru.bjfxy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vdq.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cdw.cucudq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xpx.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mue.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rbf.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ixk.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wno.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://sry.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nhs.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dkf.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fqi.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uen.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jwm.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xkp.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cse.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mzk.yj20258.top

[E16] 数字千分位
来源：http://fud.epnwcf.com

Py:   f"{1234567:,}"
来源：http://vxh.gotoacloud.top

PHP:  number_format(1234567);
来源：http://hvr.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://pmg.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uxi.ehwqpu.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kdx.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ewh.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://azi.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://cit.zhengqikj.top

[E17] 首字母大写
来源：http://lhm.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ycm.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jwb.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sli.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pyf.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dcy.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ohl.yongpay.top

Ruby: s.capitalize
来源：http://qyo.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eas.gzhubu.top

[E18] 模板占位符替换
来源：http://aca.fanxiaobao.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://frs.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qwg.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nkh.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://csj.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xxx.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sai.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ppi.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cyf.sxryk.cn

[E19] 多行文本按行拆分
来源：http://ixd.jqgufenzy.top

Py:   s.splitlines()
来源：http://ukv.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tgh.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://hdn.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://xnv.chenzaomai.com

Java: s.lines().toList()
来源：http://lip.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://fri.daria6918.cn

Ruby: s.lines
来源：http://vqn.yanxiufei.cn

C#:   s.Split('\n')
来源：http://fkk.xziqi.cn

[E20] 判断字符串是否为空
来源：http://bbu.ehwqpu.com

Py:   if not s:
来源：http://upp.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://edb.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jmq.tianlin.xyz

TS:   if (s === "") {}
来源：http://fnd.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://orf.bjfxy.top

Go:   if s == "" {}
来源：http://msl.nwbrower.top

Ruby: if s.empty?
来源：http://uhh.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gpd.52xcode.cn

[E21] 超长截断加省略号
来源：http://ysl.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lzx.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://arb.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oob.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dee.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://plc.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://bkg.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xyd.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nly.jqgufenzy.top

[E22] 字节长度与字符长度
来源：http://cwe.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gxn.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jlf.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ehz.nanxinkj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://trb.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://edf.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ort.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://uec.tianlin.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gmg.jiagoushi.top

================================================================================
来源：http://wzg.zycfv.cn

F. 文件与目录
来源：http://sjk.52xcode.cn

================================================================================
来源：http://zmx.guannengcc.top

[F01] 读取整个文件
来源：http://awp.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pph.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://gzr.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fdh.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hgg.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cxh.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uhb.yj202588.top

Ruby: File.read("a.txt")
来源：http://gcs.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://xyd.gotoacloud.top

[F02] 逐行读取文件
来源：http://tvb.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lxf.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zxx.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dyf.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qej.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://feg.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yen.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pia.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ozg.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://pen.mhx1999.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://obg.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ayx.hysaishi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nsb.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qkx.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://usd.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gwk.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://vcf.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nrx.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://pep.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tdk.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kat.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vkj.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qkk.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jra.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dym.jinqigfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xjz.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fxh.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://gwi.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://njd.yonumen.top

PHP:  file_exists("a.txt");
来源：http://fif.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://asy.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://yts.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ppu.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rkf.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://qar.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://skw.bjfxy.top

[F06] 删除文件
来源：http://skp.aizwys.cn

Py:   os.remove("a.txt")
来源：http://vcd.cheryme.top

PHP:  unlink("a.txt");
来源：http://mfq.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://oyk.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://sza.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bog.sweek.top

Go:   os.Remove("a.txt")
来源：http://dzh.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://tzf.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://jxb.yj20258888.top

[F07] 创建目录（含多级）
来源：http://vyz.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://psu.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zjy.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yxx.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wvo.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://juh.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wai.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dlq.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iwn.feifeiyinyue.top

[F08] 遍历目录
来源：http://wky.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://wbj.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qng.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://ewv.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://djx.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gwz.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hbc.ivvv.top

Ruby: Dir.children("dir")
来源：http://kvp.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://ags.ivvv.top

[F09] 获取文件大小
来源：http://pug.316326.xyz

Py:   os.path.getsize("a.txt")
来源：http://pta.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://wrv.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://lzu.shangyingyoupin.top

TS:   fs.statSync("a.txt").size
来源：http://gyl.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://ffd.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vxp.xylfe.cn

Ruby: File.size("a.txt")
来源：http://csz.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://itq.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://nul.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bkn.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mey.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ucj.smart0.xyz

TS:   path.extname("a.txt")
来源：http://qdi.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bru.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qll.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wav.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nhy.andypj.xyz

[F11] 复制与移动文件
来源：http://nmd.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vmn.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kop.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://edz.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zwx.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ncg.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kcj.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lip.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://muk.fktsv.cn

[F12] CSV 读写
来源：http://vor.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ebh.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ryj.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vhg.cdnleiting.top

TS:   // 同上
来源：http://hqr.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://stj.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rnz.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zud.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wgb.316326.xyz

================================================================================
来源：http://qxk.yanxiufei.cn

G. 面向对象
来源：http://jrt.sxryk.cn

================================================================================
来源：http://nkv.mhx1999.top

[G01] 定义类
来源：http://ijl.xuetiantiany.cn

Py:   class User: pass
来源：http://ylm.vqdsnc.cn

PHP:  class User {}
来源：http://pwg.yongpay.top

JS:   class User {}
来源：http://npq.pycfn.com

TS:   class User { name: string = ""; }
来源：http://tok.xylfe.cn

Java: class User {}
来源：http://cns.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://jgm.zhijiandao.cn

Ruby: class User; end
来源：http://xiy.gogol.net.cn

C#:   class User {}
来源：http://yyw.sxryk.cn

[G02] 构造函数
来源：http://xsx.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://xvn.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://mmp.wangdashe.top

JS:   constructor(name) { this.name = name; }
来源：http://hzz.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://nfe.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://iln.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://szz.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://pef.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://qzc.jlsjyb.cn

[G03] 实例属性
来源：http://hgk.yonumen.top

Py:   self.name = "x"
来源：http://pbo.fehbvm.com

PHP:  public string $name = "x";
来源：http://xcr.fzhhl.top

JS:   this.name = "x";
来源：http://vus.zhengqikj.top

TS:   name: string = "x";
来源：http://aor.mhx1999.top

Java: private String name;
来源：http://znr.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xjg.yj202588.top


<!-- 参考信息 -->