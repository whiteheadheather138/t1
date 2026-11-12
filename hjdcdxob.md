代发 wailian999

Go:   strings.Join(items, ",")
来源：http://kes.cashguo.top

Ruby: items.join(",")
来源：http://ujf.ydzc1.top

C#:   string.Join(",", items)
来源：http://oqn.yueranfly.top

[E09] 去除所有空白字符
来源：http://pck.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mjw.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mch.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://stv.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://dhv.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://eoa.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lgl.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://aaw.smart0.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zgb.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://bks.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vdc.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://khg.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://dpu.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://iyi.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://uaa.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vfu.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vym.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wwa.hywenlv.cn

[E11] 反转字符串
来源：http://lph.pengpengdd.cyou

Py:   s[::-1]
来源：http://xes.yueranfly.top

PHP:  strrev($s);
来源：http://hmr.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://ksl.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://xzp.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yzh.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kok.xuanzx.com

Ruby: s.reverse
来源：http://ctm.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fmo.yongpay.top

[E12] 统计某字符出现次数
来源：http://vvu.gaohongyu789.top

Py:   s.count("a")
来源：http://hmo.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://yky.shuidangran.top

JS:   s.split("a").length - 1
来源：http://ssg.fanxiaobao.xyz

TS:   s.split("a").length - 1
来源：http://kmu.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ecx.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://erj.epnwcf.com

Ruby: s.count("a")
来源：http://dvc.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://bpi.fehbvm.com

[E13] 逐字符遍历
来源：http://pml.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://jmf.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://goo.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nrq.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pix.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zgk.xingfuxueyuan.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nqf.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://gta.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rzz.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://eva.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ctu.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kff.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mit.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://avt.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oqu.c1oappe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rks.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yim.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mvy.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://prs.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://dig.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tiu.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kzm.ppjwa.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oko.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://klo.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ieq.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bpv.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mbi.ybcxt.top

[E16] 数字千分位
来源：http://kct.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://rjp.jiagoushi.top

PHP:  number_format(1234567);
来源：http://ilt.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lpe.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ifk.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hjk.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gzu.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lqu.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://utw.cashguo.top

[E17] 首字母大写
来源：http://jfm.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://azx.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lry.gzhubu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lou.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zub.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eiv.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://amo.ctjpmb.com

Ruby: s.capitalize
来源：http://now.hongshengwenyu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lrk.yj20258888.top

[E18] 模板占位符替换
来源：http://znz.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ukf.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gvq.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://aja.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wbm.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vwh.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tkn.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wmo.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aiz.nwbrower.top

[E19] 多行文本按行拆分
来源：http://xws.epnwcf.com

Py:   s.splitlines()
来源：http://cty.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rfm.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://cps.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://vkn.yanxiufei.cn

Java: s.lines().toList()
来源：http://dyu.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://lmv.xinyue.icu

Ruby: s.lines
来源：http://dor.gogol.net.cn

C#:   s.Split('\n')
来源：http://pso.zycfv.cn

[E20] 判断字符串是否为空
来源：http://mxe.xinyue.icu

Py:   if not s:
来源：http://wst.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tzm.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aav.zhijiandao.cn

TS:   if (s === "") {}
来源：http://rci.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://fpn.yj20258888.top

Go:   if s == "" {}
来源：http://evy.zhengqikj.top

Ruby: if s.empty?
来源：http://mnk.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zqb.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://vuo.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://suh.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ech.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lqe.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mgf.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zns.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://szv.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jrb.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://abf.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://vlh.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://exy.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ztp.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blu.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hgh.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rna.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tme.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://qhv.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://viw.shanyushiyangtech.top

================================================================================
来源：http://nft.smart0.xyz

F. 文件与目录
来源：http://vbe.zhaomingkeji.xyz

================================================================================
来源：http://bii.yj20258888.top

[F01] 读取整个文件
来源：http://cdc.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pgv.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://myd.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://efu.cdnleiting.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rhj.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://uuu.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://avv.xziqi.cn

Ruby: File.read("a.txt")
来源：http://dca.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://mzy.tianlin.xyz

[F02] 逐行读取文件
来源：http://ipv.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zup.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pmr.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ghy.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zeq.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nhz.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xai.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xjn.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://asr.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://vom.feifeiyinyue.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ink.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://haw.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ghg.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lei.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ayi.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nve.daxiang520.top

Ruby: File.write("a.txt", "hi")
来源：http://had.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bvs.jlsjyb.cn

[F04] 追加写入文件
来源：http://llo.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://okd.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://min.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ztm.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyk.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://owo.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jqu.9152youxi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qqv.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wlp.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://wga.haohaochexian.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://omj.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://koq.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://ffd.cheryme.top

TS:   fs.existsSync("a.txt")
来源：http://yro.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://yci.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nnb.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://qdi.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://ewb.quarkkingdee.top

[F06] 删除文件
来源：http://cfk.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://qee.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://oms.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://sfy.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://zfj.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ovp.ybcxt.top

Go:   os.Remove("a.txt")
来源：http://afi.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://pqo.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://vkb.sweek.top

[F07] 创建目录（含多级）
来源：http://bcb.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wbe.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bcd.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uli.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gfh.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zws.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sid.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ntl.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://miv.guowangkeji.top

[F08] 遍历目录
来源：http://xwe.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://auh.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vor.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://cyn.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://ean.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rpm.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://cgz.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://npp.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://isa.zhiwuduotai.top

[F09] 获取文件大小
来源：http://fyk.yueranfly.top

Py:   os.path.getsize("a.txt")
来源：http://wzn.cashguo.top

PHP:  filesize("a.txt");
来源：http://hid.jlsjyb.cn

JS:   fs.statSync("a.txt").size
来源：http://nzs.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://ugj.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://zds.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ukk.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://gzb.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://oou.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://ige.xuanzx.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mwp.jinghuilouyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kif.hesvh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oxb.yongpay.top

TS:   path.extname("a.txt")
来源：http://igm.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lqi.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bxf.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dxn.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zwn.snrcjt.cn

[F11] 复制与移动文件
来源：http://mun.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fin.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ota.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lth.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xtx.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dtc.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ysw.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rss.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hps.birdmap.top

[F12] CSV 读写
来源：http://fea.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xcf.gaohongyu789.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uqu.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tmr.xuanzx.com

TS:   // 同上
来源：http://klf.yj20258888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wlm.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mky.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hvm.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bjc.hysaishi.cn

================================================================================
来源：http://iww.bbcook.cn

G. 面向对象
来源：http://xge.ppjwa.cn

================================================================================
来源：http://eqc.zycfv.cn

[G01] 定义类
来源：http://cve.zhaomingkeji.xyz

Py:   class User: pass
来源：http://nbd.mhx1999.top

PHP:  class User {}
来源：http://tqo.zhiwuduotai.top

JS:   class User {}
来源：http://ymj.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://jif.zhijiandao.cn

Java: class User {}
来源：http://bdi.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://qhx.zycfv.cn

Ruby: class User; end
来源：http://xcm.zhaomingkeji.xyz

C#:   class User {}
来源：http://xzj.jyoumei.cn

[G02] 构造函数
来源：http://kqi.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://uqz.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://snq.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://ucd.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://ofs.jianghu66.top

Java: User(String name) { this.name = name; }
来源：http://oqz.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vnx.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://svq.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://ifx.shuidangran.top

[G03] 实例属性
来源：http://jgk.chenlongwang.top

Py:   self.name = "x"
来源：http://lnv.kuanghao11.cn

PHP:  public string $name = "x";
来源：http://htc.redwolf501.top

JS:   this.name = "x";
来源：http://uek.chenzaomai.com

TS:   name: string = "x";
来源：http://cmx.snrcjt.cn

Java: private String name;
来源：http://vcq.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uyo.hnxiangtu.top

Ruby: @name = "x"
来源：http://ybs.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://wob.jinqigufen.top

[G04] 定义方法
来源：http://adl.ybcxt.top

Py:   def greet(self): return self.name
来源：http://psk.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://stt.shuidangran.top

JS:   greet() { return this.name; }
来源：http://bid.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://yfr.cqqwz.cn

Java: String greet() { return name; }
来源：http://yye.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zgh.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://tqj.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://vzu.smart0.xyz

[G05] 继承
来源：http://jai.bbcook.cn

Py:   class Admin(User): pass
来源：http://ntc.mhx1999.top

PHP:  class Admin extends User {}
来源：http://jjz.yj202588.top

JS:   class Admin extends User {}
来源：http://pbp.zdqjudy.top

TS:   class Admin extends User {}
来源：http://jxi.ydzc1.top

Java: class Admin extends User {}
来源：http://ais.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kqg.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://xrn.zycfv.cn

C#:   class Admin : User {}
来源：http://mfn.tianlin.xyz

[G06] 重写方法
来源：http://uap.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://mmq.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://old.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://hab.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://zjz.yuanzhike.top

Java: @Override String greet() { return "admin"; }
来源：http://dec.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://juz.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://cuw.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://pjj.yj20258.top

[G07] 调用父类方法
来源：http://vpm.tarul.cn

Py:   super().greet()
来源：http://imy.jinqigfzy.top

PHP:  parent::greet();
来源：http://dbn.xylfe.cn


<!-- 参考信息 -->