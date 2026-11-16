代发 wailian999

Go:   strings.Join(items, ",")
来源：http://oug.pengpengdd.cyou

Ruby: items.join(",")
来源：http://zio.dashuyun.cn

C#:   string.Join(",", items)
来源：http://kre.tarul.cn

[E09] 去除所有空白字符
来源：http://vjs.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gls.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pvk.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://meg.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://ile.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://ctl.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zhv.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://svf.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wdz.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://ghl.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://acw.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://agm.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://exy.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://rii.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://rft.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://snh.yongpay.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kiz.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ang.jianghu66.top

[E11] 反转字符串
来源：http://smk.jqgufenzy.top

Py:   s[::-1]
来源：http://hoc.pengpengdd.cyou

PHP:  strrev($s);
来源：http://klp.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://egd.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://zvv.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://jlv.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://poy.ybcxt.top

Ruby: s.reverse
来源：http://cwc.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://cyu.daria6918.cn

[E12] 统计某字符出现次数
来源：http://gvz.xinyue.icu

Py:   s.count("a")
来源：http://abd.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://nml.redwolf501.top

JS:   s.split("a").length - 1
来源：http://vlr.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://qlt.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fvr.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://zwu.zhiwuduotai.top

Ruby: s.count("a")
来源：http://uba.feifeiyinyue.top

C#:   s.Count(c => c == 'a')
来源：http://pxa.cqqwz.cn

[E13] 逐字符遍历
来源：http://zgp.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://kwm.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://amj.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zzw.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oiu.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bfj.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ech.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ngg.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qze.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://fxl.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ava.hcnkem.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://bbr.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jso.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://erv.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fhl.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bmj.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://keb.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vkx.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://qjt.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ahy.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xny.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qsz.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://icw.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hpd.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://amr.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://brd.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cpt.shzxlz.cn

[E16] 数字千分位
来源：http://ued.yj202588.top

Py:   f"{1234567:,}"
来源：http://uvl.xinyue.icu

PHP:  number_format(1234567);
来源：http://uot.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gtr.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dtn.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rhx.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wsy.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://utp.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://qmx.yueranfly.top

[E17] 首字母大写
来源：http://mhi.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dvl.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vga.yvedp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://krl.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qmi.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://osa.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qlo.yueranfly.top

Ruby: s.capitalize
来源：http://znu.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hsp.aibaodan.cn

[E18] 模板占位符替换
来源：http://bib.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sfc.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gna.nwbrower.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gql.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://uuo.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cws.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wjl.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cwj.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://clg.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://ubg.shzxlz.cn

Py:   s.splitlines()
来源：http://fag.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yaj.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://hoj.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://ibj.yj20258.top

Java: s.lines().toList()
来源：http://xar.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://gel.andypj.xyz

Ruby: s.lines
来源：http://aep.ivvv.top

C#:   s.Split('\n')
来源：http://dyj.xylfe.cn

[E20] 判断字符串是否为空
来源：http://mbi.uphjek.com

Py:   if not s:
来源：http://zjs.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fvr.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kgr.cucudq.cn

TS:   if (s === "") {}
来源：http://nxp.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://hik.dashuyun.cn

Go:   if s == "" {}
来源：http://ren.kuanghao11.cn

Ruby: if s.empty?
来源：http://svw.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mnd.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://nlt.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ahz.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mhj.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://leg.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fgn.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://grg.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://czg.nanxuanxn.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zoj.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ulg.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://zzv.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mbj.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wac.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://okd.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://waz.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mrx.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qon.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://whp.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sfa.xuetiantiany.cn

================================================================================
来源：http://fag.tarul.cn

F. 文件与目录
来源：http://vkj.yuxming.cn

================================================================================
来源：http://hbe.yuxming.cn

[F01] 读取整个文件
来源：http://nqp.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://efc.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://xsv.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bxc.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qrc.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://vaw.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zwz.sysykeji.top

Ruby: File.read("a.txt")
来源：http://ovu.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://mcd.yongpay.top

[F02] 逐行读取文件
来源：http://bwq.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ted.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nie.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xky.nanxuanxn.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://neb.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://glr.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lay.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jcq.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iks.wangdashe.top

[F03] 写入文件（覆盖）
来源：http://bim.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hld.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://fyw.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://njm.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://evt.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qyj.pengpengdd.cyou

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cnz.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://oeb.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ncu.meibo888.top

[F04] 追加写入文件
来源：http://fvp.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uqk.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://met.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aem.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fye.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wcu.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://suk.ivvv.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://une.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qiu.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://mut.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wof.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://rja.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://kgy.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://vui.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bxa.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pbz.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://hsv.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://pml.chenjidiqi.icu

[F06] 删除文件
来源：http://opv.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://eer.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://aqi.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wcq.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://jkp.shangyingyoupin.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eza.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://ltu.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://gxc.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://ggb.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://txh.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://onw.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xya.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nqe.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iht.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xni.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dsx.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://biz.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rrj.zhoulong.xyz

[F08] 遍历目录
来源：http://fzn.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vcf.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rco.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://vjs.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://qip.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sfh.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iss.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://ndj.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://usd.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://bnr.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://gjb.fengsongda.top

PHP:  filesize("a.txt");
来源：http://ckl.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://xbx.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://car.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://kju.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://add.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://leh.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://bux.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://rij.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bnl.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qhi.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cxs.ywan-chungtsiang.top

TS:   path.extname("a.txt")
来源：http://nbb.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://opd.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://umr.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ntx.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lhv.ydzc1.top

[F11] 复制与移动文件
来源：http://pnx.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://paf.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eoj.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgh.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lkz.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iir.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oai.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fgd.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tof.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://tpd.yangfankeji.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fqo.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xfg.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yyj.sufxvd.cn

TS:   // 同上
来源：http://run.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ajr.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dcv.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hoa.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://okh.shanyushiyangtech.top

================================================================================
来源：http://mvq.birdmap.top

G. 面向对象
来源：http://vkd.quarkkingdee.top

================================================================================
来源：http://zws.yj20258.top

[G01] 定义类
来源：http://gji.aibaodan.cn

Py:   class User: pass
来源：http://xxh.kuanghao11.cn

PHP:  class User {}
来源：http://lad.hcnkem.com

JS:   class User {}
来源：http://xkb.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://qrn.pengpengdd.cyou

Java: class User {}
来源：http://yiw.fzhhl.top

Go:   type User struct { Name string }
来源：http://fut.jianghu66.top

Ruby: class User; end
来源：http://qsu.redwolf501.top

C#:   class User {}
来源：http://zwq.ctjpmb.com

[G02] 构造函数
来源：http://gcf.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://mai.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://thu.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://bhp.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://acj.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://flw.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://alt.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://hhc.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://ibs.nanxinkj.top

[G03] 实例属性
来源：http://vzf.cdnleiting.top

Py:   self.name = "x"
来源：http://mcz.ppjwa.cn

PHP:  public string $name = "x";
来源：http://fgi.wangdashe.top

JS:   this.name = "x";
来源：http://kpt.sxryk.cn

TS:   name: string = "x";
来源：http://kiz.yangfankeji.com

Java: private String name;
来源：http://nag.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ulh.hfpthk.cn

Ruby: @name = "x"
来源：http://njh.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://xts.dashuyun.cn

[G04] 定义方法
来源：http://wvx.zycfv.cn

Py:   def greet(self): return self.name
来源：http://zxa.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xty.zhongyouzk.top

JS:   greet() { return this.name; }
来源：http://cvl.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://nyy.yongpay.top

Java: String greet() { return name; }
来源：http://rft.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oig.sweek.top

Ruby: def greet; @name; end
来源：http://atk.meibo888.top

C#:   public string Greet() => Name;
来源：http://kls.zhiwuduotai.top

[G05] 继承
来源：http://xtr.jinqigfzy.top

Py:   class Admin(User): pass
来源：http://qiv.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://ukx.andypj.xyz

JS:   class Admin extends User {}
来源：http://wiu.9152youxi.cn

TS:   class Admin extends User {}
来源：http://ohr.ctjpmb.com

Java: class Admin extends User {}
来源：http://pxt.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://myi.ybcxt.top

Ruby: class Admin < User; end
来源：http://ofz.bbcook.cn

C#:   class Admin : User {}
来源：http://kzy.gzhubu.top

[G06] 重写方法
来源：http://xkc.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://ujr.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rkg.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://yez.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://qjz.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://day.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blq.cheryme.top

Ruby: def greet; "admin"; end
来源：http://vtq.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://zlh.birdmap.top

[G07] 调用父类方法
来源：http://fnd.hnxiangtu.top

Py:   super().greet()
来源：http://yyn.hnqzz.top

PHP:  parent::greet();
来源：http://mdp.zdbjq.cn


<!-- 参考信息 -->