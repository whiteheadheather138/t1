代发 wailian999

Go:   strings.Join(items, ",")
来源：http://qnp.nwbrower.top

Ruby: items.join(",")
来源：http://myq.316326.xyz

C#:   string.Join(",", items)
来源：http://yta.birdmap.top

[E09] 去除所有空白字符
来源：http://lss.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iag.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fgw.yfazqb.com

JS:   s.replace(/\s+/g, "")
来源：http://irx.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://ovq.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://mqq.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zka.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://isj.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://krf.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://uzg.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ptc.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vhp.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://lqs.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://pnq.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://zmr.yueranfly.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bzc.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hve.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cma.redwolf501.top

[E11] 反转字符串
来源：http://kua.sxryk.cn

Py:   s[::-1]
来源：http://kdt.ybcxt.top

PHP:  strrev($s);
来源：http://vkr.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://aia.hnxiangtu.top

TS:   [...s].reverse().join("")
来源：http://nse.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uez.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qfk.xuetiantiany.cn

Ruby: s.reverse
来源：http://edb.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jxl.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://abq.feifeiyinyue.top

Py:   s.count("a")
来源：http://vlz.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://ogf.zhongyouzk.top

JS:   s.split("a").length - 1
来源：http://vfe.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://rcq.birdmap.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://egf.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://hit.shangyingyoupin.top

Ruby: s.count("a")
来源：http://bdz.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://vqf.jyoumei.cn

[E13] 逐字符遍历
来源：http://ick.daxiang520.top

Py:   for ch in s: print(ch)
来源：http://rtb.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gts.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://vas.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xcv.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zyb.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wue.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sxg.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gkp.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://gwl.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rfz.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://spm.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nvh.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qlp.ywan-chungtsiang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://epp.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fhq.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://voc.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xkz.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://csv.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tws.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://onq.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vid.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vtv.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rki.cqqwz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://etm.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wxz.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fmt.shanyushiyangkeji.top

[E16] 数字千分位
来源：http://stq.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://doq.hnqzz.top

PHP:  number_format(1234567);
来源：http://fra.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fwt.gotoacloud.top

TS:   (1234567).toLocaleString("en-US")
来源：http://uyz.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wkr.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rzi.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zom.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://jme.316326.xyz

[E17] 首字母大写
来源：http://lnw.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lxe.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://kvk.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cue.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fyj.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cad.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rhx.gzhubu.top

Ruby: s.capitalize
来源：http://oix.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uvc.nanxinkj.top

[E18] 模板占位符替换
来源：http://ezd.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gcv.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ijs.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://khp.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jlg.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hpo.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nsf.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cof.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ulv.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://tcw.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://xxz.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kof.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://pot.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://urp.xuetiantiany.cn

Java: s.lines().toList()
来源：http://cbo.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://spv.zhijiandao.cn

Ruby: s.lines
来源：http://gcw.jqgfzy.top

C#:   s.Split('\n')
来源：http://tye.xuanzx.com

[E20] 判断字符串是否为空
来源：http://qtf.ydjk.org.cn

Py:   if not s:
来源：http://ode.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cjr.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://slb.9152youxi.cn

TS:   if (s === "") {}
来源：http://kbw.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://tpb.yfazqb.com

Go:   if s == "" {}
来源：http://ppv.cqqwz.cn

Ruby: if s.empty?
来源：http://fsd.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ejr.gogol.net.cn

[E21] 超长截断加省略号
来源：http://qjw.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kpc.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nlf.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bgc.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cdt.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://syi.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://mss.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://trl.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qhn.ydzc1.top

[E22] 字节长度与字符长度
来源：http://sea.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yuu.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fdz.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rmv.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ynr.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bfr.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://czc.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://igv.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wyi.xingfuxueyuan.xyz

================================================================================
来源：http://hom.fzhhl.top

F. 文件与目录
来源：http://ydf.tanke756.top

================================================================================
来源：http://qvx.hnqzz.top

[F01] 读取整个文件
来源：http://vzg.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vbm.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://ixp.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://byt.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jev.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://epa.ybcxt.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cgn.meibo888.top

Ruby: File.read("a.txt")
来源：http://dae.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://vbp.sufxvd.cn

[F02] 逐行读取文件
来源：http://sdj.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zkd.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://frn.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ibl.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ndv.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fwc.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wfn.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dhf.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kjv.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://ple.ydjk.org.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://toq.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://huo.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ugu.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tyx.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nxj.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://duf.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://ceb.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://twn.gotoacloud.top

[F04] 追加写入文件
来源：http://cke.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yxd.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vcc.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xfg.jinghuilouyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://arl.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hxy.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fbh.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kmy.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://usk.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://kct.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fdt.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://xxk.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://tmg.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://lpz.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://msu.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ozd.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://viy.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://pxd.zhaomingkeji.xyz

[F06] 删除文件
来源：http://vms.sweek.top

Py:   os.remove("a.txt")
来源：http://ojh.yongpay.top

PHP:  unlink("a.txt");
来源：http://qch.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tot.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://hyf.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://roi.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://xui.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://bae.cheryme.top

C#:   File.Delete("a.txt");
来源：http://iae.hnqzz.top

[F07] 创建目录（含多级）
来源：http://hzy.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://odr.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ecd.ybcxt.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fjx.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mri.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gkf.ehwqpu.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hed.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bgb.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sil.fzhhl.top

[F08] 遍历目录
来源：http://kki.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://coi.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uyd.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://mxv.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://lgy.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rcb.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bng.52xcode.cn

Ruby: Dir.children("dir")
来源：http://xzq.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://wsb.hywenlv.cn

[F09] 获取文件大小
来源：http://xqr.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://eqw.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://pcr.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://vbs.cashguo.top

TS:   fs.statSync("a.txt").size
来源：http://xvr.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://oka.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nbd.pycfn.com

Ruby: File.size("a.txt")
来源：http://qbe.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://smz.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://agl.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lop.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bzk.yonumen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ara.mhx1999.top

TS:   path.extname("a.txt")
来源：http://igc.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mdp.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dqk.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://psu.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mxc.meibo888.top

[F11] 复制与移动文件
来源：http://kwu.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cyn.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sce.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ofl.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://knv.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ign.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oza.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://syw.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://abo.xuanzx.com

[F12] CSV 读写
来源：http://oix.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vil.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zju.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sxl.zhixingplan.top

TS:   // 同上
来源：http://kzv.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nxh.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ulj.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sxj.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://azc.sysykeji.top

================================================================================
来源：http://wdb.yj202588.top

G. 面向对象
来源：http://rrq.snrcjt.cn

================================================================================
来源：http://pau.smart0.xyz

[G01] 定义类
来源：http://hty.aibaodan.cn

Py:   class User: pass
来源：http://pmu.tian-w.cn

PHP:  class User {}
来源：http://jio.shanyushiyangkeji.top

JS:   class User {}
来源：http://ucq.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://gfd.jinghuilouyu.cn

Java: class User {}
来源：http://kte.aibaodan.cn

Go:   type User struct { Name string }
来源：http://use.gotoacloud.top

Ruby: class User; end
来源：http://vgx.chenlongwang.top

C#:   class User {}
来源：http://alk.ppjwa.cn

[G02] 构造函数
来源：http://xbd.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://iln.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://uzy.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://hok.meibo888.top

TS:   constructor(public name: string) {}
来源：http://wbz.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://iut.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hvm.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://ydk.fengsongda.top

C#:   public User(string name) { Name = name; }
来源：http://fta.sufxvd.cn

[G03] 实例属性
来源：http://qeq.smart0.xyz

Py:   self.name = "x"
来源：http://vfz.0kj1m.cn

PHP:  public string $name = "x";
来源：http://ifs.bjfxy.top

JS:   this.name = "x";
来源：http://nxj.yj20258888.top

TS:   name: string = "x";
来源：http://qar.meibo888.top

Java: private String name;
来源：http://ank.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jyu.svipenyu.cn

Ruby: @name = "x"
来源：http://jam.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://lhe.wangdashe.top

[G04] 定义方法
来源：http://sbs.cheryme.top

Py:   def greet(self): return self.name
来源：http://llm.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://avx.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://wrp.haohaochexian.top

TS:   greet(): string { return this.name; }
来源：http://wai.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://tpr.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oyg.cqqwz.cn

Ruby: def greet; @name; end
来源：http://nvz.daria6918.cn

C#:   public string Greet() => Name;
来源：http://hru.zycfv.cn

[G05] 继承
来源：http://pne.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://mnm.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://jti.tian-w.cn

JS:   class Admin extends User {}
来源：http://icp.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://xey.yuanzhike.top

Java: class Admin extends User {}
来源：http://qfh.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ohg.mhx1999.top

Ruby: class Admin < User; end
来源：http://hoh.0kj1m.cn

C#:   class Admin : User {}
来源：http://fao.sjlbkw.cn

[G06] 重写方法
来源：http://fwr.iojbl.cn

Py:   def greet(self): return "admin"
来源：http://qjr.dianchejie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ath.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://buq.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://nkq.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://rtl.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cuu.cdnleiting.top

Ruby: def greet; "admin"; end
来源：http://ttz.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://ujt.hfpthk.cn

[G07] 调用父类方法
来源：http://rkk.shanyushiyangtech.top

Py:   super().greet()
来源：http://dss.yongpay.top

PHP:  parent::greet();
来源：http://jdi.meibo888.top


<!-- 参考信息 -->