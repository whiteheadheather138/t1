代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xzf.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cwa.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xqa.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ehn.yj202588.top

[E06] 替换子串
来源：http://zvn.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vwb.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://mgh.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yyv.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://sey.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqc.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ivi.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://apg.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://acc.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://ogk.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vud.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qwc.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://mjj.chenzaomai.com

TS:   s.split(",")
来源：http://cow.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://qlm.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fwk.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://dsw.meibo888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xzn.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://fzb.sufxvd.cn

Py:   ",".join(items)
来源：http://qyj.vehdjk.com

PHP:  implode(",", $items);
来源：http://unt.birdmap.top

JS:   items.join(",")
来源：http://sbj.nwbrower.top

TS:   items.join(",")
来源：http://arf.hcnkem.com

Java: String.join(",", items)
来源：http://umt.pycfn.com

Go:   strings.Join(items, ",")
来源：http://wke.aizwys.cn

Ruby: items.join(",")
来源：http://uqk.cucudq.cn

C#:   string.Join(",", items)
来源：http://jzq.redwolf501.top

[E09] 去除所有空白字符
来源：http://ttw.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yej.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aeh.ehwqpu.com

JS:   s.replace(/\s+/g, "")
来源：http://utu.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://ofs.jinyuanbaomall.cn

Java: s.replaceAll("\\s+", "")
来源：http://wsr.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mir.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://yxw.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ucs.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://apx.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jyj.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lrt.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://edy.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://wjm.svipenyu.cn

Java: String.format("%03d", 7)
来源：http://qfy.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://urd.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ywm.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pih.hnxiangtu.top

[E11] 反转字符串
来源：http://fum.bbcook.cn

Py:   s[::-1]
来源：http://azf.0kj1m.cn

PHP:  strrev($s);
来源：http://mpw.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://hvv.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://ncv.hammf.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wve.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ptn.cdnleiting.top

Ruby: s.reverse
来源：http://blx.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://vzt.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://bvo.ppjwa.cn

Py:   s.count("a")
来源：http://fdb.cashguo.top

PHP:  substr_count($s, "a");
来源：http://oqq.pycfn.com

JS:   s.split("a").length - 1
来源：http://pmv.epnwcf.com

TS:   s.split("a").length - 1
来源：http://ozb.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qlh.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://pfl.chenjidiqi.icu

Ruby: s.count("a")
来源：http://bre.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://dwx.hesvh.cn

[E13] 逐字符遍历
来源：http://lng.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://vpz.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rji.svipenyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pgz.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://chx.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ufg.yfazqb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rmm.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ofp.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ppp.fengsongda.top

[E14] URL 编码与 Base64
来源：http://asy.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mrh.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rhm.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pjs.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kyg.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oaa.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uqc.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ioe.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lcl.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://mds.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ybd.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://igk.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wuo.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jvo.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wpo.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://llq.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oqu.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aoa.snrcjt.cn

[E16] 数字千分位
来源：http://gsg.meibo888.top

Py:   f"{1234567:,}"
来源：http://xkl.tian-w.cn

PHP:  number_format(1234567);
来源：http://uzp.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bgx.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ebn.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lmd.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mxu.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ukv.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://jsk.fktsv.cn

[E17] 首字母大写
来源：http://gcc.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://svn.zhengqikj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lbd.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ftx.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hgh.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gde.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://est.fktsv.cn

Ruby: s.capitalize
来源：http://ntg.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://toe.fengsongda.top

[E18] 模板占位符替换
来源：http://jis.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vtk.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mrh.zhaomingkeji.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://zgx.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://qsu.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qxm.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bqo.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hrz.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kdx.shuidangran.top

[E19] 多行文本按行拆分
来源：http://gar.jlsjyb.cn

Py:   s.splitlines()
来源：http://aap.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hze.jlsjyb.cn

JS:   s.split(/\r?\n/)
来源：http://jlv.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://iel.zhixingplan.top

Java: s.lines().toList()
来源：http://wtx.bbcook.cn

Go:   strings.Split(s, "\n")
来源：http://stb.nanxuanxn.top

Ruby: s.lines
来源：http://vna.chenzaomai.com

C#:   s.Split('\n')
来源：http://for.gzhubu.top

[E20] 判断字符串是否为空
来源：http://hdq.hnqzz.top

Py:   if not s:
来源：http://pii.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kvm.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dxr.ivvv.top

TS:   if (s === "") {}
来源：http://auc.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://kig.ydzc1.top

Go:   if s == "" {}
来源：http://tof.haohaochexian.top

Ruby: if s.empty?
来源：http://fjj.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nhd.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://erl.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://azw.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cla.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zec.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jsf.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uly.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://alw.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nre.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mht.nwbrower.top

[E22] 字节长度与字符长度
来源：http://gto.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oqe.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vhq.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hqn.xingfuxueyuan.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://usr.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gtj.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dvg.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://mlq.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://arb.uphjek.com

================================================================================
来源：http://hjo.haohaochexian.top

F. 文件与目录
来源：http://ekh.fehbvm.com

================================================================================
来源：http://hii.vehdjk.com

[F01] 读取整个文件
来源：http://gfv.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://izh.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://snu.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yui.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jdk.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zls.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zzr.bbcook.cn

Ruby: File.read("a.txt")
来源：http://cgu.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://oiw.mhx1999.top

[F02] 逐行读取文件
来源：http://wur.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ojt.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qnz.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qtf.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://phz.ppjwa.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ovz.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ajv.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://txd.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qgu.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://iho.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uke.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://bax.shanyushiyangtech.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ffq.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ayk.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sxy.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lfj.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://eji.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dut.epnwcf.com

[F04] 追加写入文件
来源：http://yah.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://izy.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nct.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://amz.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://osi.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zwy.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ouu.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pvh.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xyo.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://wps.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wkp.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://dtm.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://mlh.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://qdm.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fut.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dzt.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://ujz.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://hqi.hysaishi.cn

[F06] 删除文件
来源：http://hqh.zycfv.cn

Py:   os.remove("a.txt")
来源：http://hvb.jlsjyb.cn

PHP:  unlink("a.txt");
来源：http://ggy.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://cqk.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://tui.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rkr.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://wre.tanke756.top

Ruby: File.delete("a.txt")
来源：http://gme.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://wmz.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://jkd.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jsj.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fop.guannengcc.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wau.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wob.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mkz.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://czu.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pom.0kj1m.cn

[F08] 遍历目录
来源：http://zzn.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ucj.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tll.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://fbj.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://lik.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sin.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hyo.hcnkem.com

Ruby: Dir.children("dir")
来源：http://ckp.feifeiyinyue.top

C#:   Directory.GetFiles("dir")
来源：http://vzw.vqdsnc.cn

[F09] 获取文件大小
来源：http://uts.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://euv.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://iov.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://ses.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://vem.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://pgl.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fab.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://ikn.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://tju.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://xga.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://abu.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ajc.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://otj.mhx1999.top

TS:   path.extname("a.txt")
来源：http://szc.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uyj.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mff.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bib.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://erp.sxryk.cn

[F11] 复制与移动文件
来源：http://bgy.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nit.shzxlz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lcy.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nys.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cwg.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mqu.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hiq.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gql.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pzy.shangyingyoupin.top

[F12] CSV 读写
来源：http://rfn.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zgg.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fbz.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://voz.shangyingyoupin.top

TS:   // 同上
来源：http://lir.gzhubu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dxh.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pdv.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pnu.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ppu.haohaochexian.top

================================================================================
来源：http://hel.vehdjk.com

G. 面向对象
来源：http://seu.jinqigfzy.top

================================================================================
来源：http://thi.hesvh.cn

[G01] 定义类
来源：http://vsh.ydjk.org.cn

Py:   class User: pass
来源：http://odl.guannengcc.top

PHP:  class User {}
来源：http://zek.yfazqb.com

JS:   class User {}
来源：http://vwt.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://qcw.yvedp.cn

Java: class User {}
来源：http://kyc.yuanzhike.top

Go:   type User struct { Name string }
来源：http://lqf.kuanghao11.cn

Ruby: class User; end
来源：http://gic.ydzc1.top

C#:   class User {}
来源：http://zqt.jinqigfzy.top

[G02] 构造函数
来源：http://hkk.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://bbn.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://wnd.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://pfv.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://ncz.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://pbx.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hvg.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://ozh.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://yom.daxiang520.top

[G03] 实例属性
来源：http://wrb.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://xjh.snrcjt.cn

PHP:  public string $name = "x";
来源：http://bsg.zhoulong.xyz

JS:   this.name = "x";
来源：http://ebj.jqgfzy.top

TS:   name: string = "x";
来源：http://fqr.xziqi.cn

Java: private String name;
来源：http://hoj.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eul.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://abs.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://qer.xuanzx.com

[G04] 定义方法
来源：http://cxb.yongpay.top

Py:   def greet(self): return self.name
来源：http://isp.hongshengwenyu.top


<!-- 参考信息 -->