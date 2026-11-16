代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ccc.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rtc.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://rzq.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://zvj.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://rlv.nanxinkj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://axl.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://smm.cashguo.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zpb.andypj.xyz

[E10] 左侧补零 / 定长填充
来源：http://ghh.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uog.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xua.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://mef.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://bfu.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://fke.jyoumei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dtn.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zbe.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://scj.yongpay.top

[E11] 反转字符串
来源：http://wny.yonumen.top

Py:   s[::-1]
来源：http://vfz.aibaodan.cn

PHP:  strrev($s);
来源：http://jyl.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://wuf.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://fii.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://plq.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://blr.0kj1m.cn

Ruby: s.reverse
来源：http://dod.iojbl.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rjf.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://qby.yangfankeji.com

Py:   s.count("a")
来源：http://iwg.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://jem.yongpay.top

JS:   s.split("a").length - 1
来源：http://dwg.daria6918.cn

TS:   s.split("a").length - 1
来源：http://rgb.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mqi.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://glw.0kj1m.cn

Ruby: s.count("a")
来源：http://glf.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://rqm.shuidangran.top

[E13] 逐字符遍历
来源：http://bzo.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://set.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://urk.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bwe.ehwqpu.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://zyb.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://koj.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nmn.daria6918.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qsj.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qxw.xinyue.icu

[E14] URL 编码与 Base64
来源：http://tis.tanke756.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dra.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://lxt.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hoy.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mtk.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://maf.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://unw.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fds.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gqd.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://oyu.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lfd.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ywd.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vkv.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xll.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bzg.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fzo.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://avl.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://khf.yonumen.top

[E16] 数字千分位
来源：http://vdh.fengsongda.top

Py:   f"{1234567:,}"
来源：http://sjj.vehdjk.com

PHP:  number_format(1234567);
来源：http://hbw.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tks.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://otq.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ebb.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bwh.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pps.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://sym.bjfxy.top

[E17] 首字母大写
来源：http://llm.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bpm.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://rhd.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://otd.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ooc.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uwd.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mey.gaohongyu789.top

Ruby: s.capitalize
来源：http://jaa.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yjf.hfpthk.cn

[E18] 模板占位符替换
来源：http://qbs.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xbm.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mai.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mgy.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yst.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rhb.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ylv.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vjv.sysykeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ohr.birdmap.top

[E19] 多行文本按行拆分
来源：http://uns.nanxuanxn.top

Py:   s.splitlines()
来源：http://rsg.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://njx.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://pff.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://awi.zdqjudy.top

Java: s.lines().toList()
来源：http://nou.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://pqp.yuxming.cn

Ruby: s.lines
来源：http://vvm.nwbrower.top

C#:   s.Split('\n')
来源：http://tdy.daxiang520.top

[E20] 判断字符串是否为空
来源：http://rsf.xingfuxueyuan.xyz

Py:   if not s:
来源：http://qyw.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lqk.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oah.epnwcf.com

TS:   if (s === "") {}
来源：http://ozt.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://wzv.hesvh.cn

Go:   if s == "" {}
来源：http://qxd.xziqi.cn

Ruby: if s.empty?
来源：http://xpv.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cfh.sufxvd.cn

[E21] 超长截断加省略号
来源：http://azn.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lgx.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xlk.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ngc.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hjv.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kxz.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ygb.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kla.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ofk.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://uvv.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oqs.zycfv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ajl.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iew.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fmw.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gfm.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://svc.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://rhv.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sqh.meibo888.top

================================================================================
来源：http://qqx.jyoumei.cn

F. 文件与目录
来源：http://ftv.jinyuanbaomall.cn

================================================================================
来源：http://vfc.zycfv.cn

[F01] 读取整个文件
来源：http://sfk.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mvh.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://ocv.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mff.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://unb.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ike.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qbn.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://bow.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://fnx.jianghu66.top

[F02] 逐行读取文件
来源：http://vla.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iyj.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hlv.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://usj.redwolf501.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qul.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ujg.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uzu.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://drm.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tgp.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://efm.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cmk.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bzz.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oli.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pfs.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pqg.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dzw.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://pha.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://obi.nanxuanxn.top

[F04] 追加写入文件
来源：http://tnc.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cav.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qgt.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cgz.gogol.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xqu.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wjw.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kyc.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wtc.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tio.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://vwb.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jju.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://guh.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://qyk.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://oos.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aeu.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gsx.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://iai.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://jlq.xuanzx.com

[F06] 删除文件
来源：http://blw.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://dnc.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://wcr.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://rce.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yiq.jianghu66.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hxu.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://ily.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://xdu.tarul.cn

C#:   File.Delete("a.txt");
来源：http://uge.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://ktz.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nvk.zhijiandao.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ktg.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nnz.birdmap.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://syr.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bmb.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zfj.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mdq.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dhk.zycfv.cn

[F08] 遍历目录
来源：http://nlx.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://whf.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tdr.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://blw.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://uaa.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yyb.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hsv.pycfn.com

Ruby: Dir.children("dir")
来源：http://xag.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://zhi.fehbvm.com

[F09] 获取文件大小
来源：http://xei.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://tvx.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://qhe.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://lga.sweek.top

TS:   fs.statSync("a.txt").size
来源：http://itc.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lmn.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yco.xziqi.cn

Ruby: File.size("a.txt")
来源：http://oyt.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://toy.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://sqh.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wod.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fns.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://czd.birdmap.top

TS:   path.extname("a.txt")
来源：http://nhx.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nmy.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://png.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zwc.iojbl.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wes.dashuyun.cn

[F11] 复制与移动文件
来源：http://wpg.zhaomingkeji.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zva.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ugc.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dkd.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jfy.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tvy.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bta.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fvv.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pdz.chenjidiqi.icu

[F12] CSV 读写
来源：http://oay.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fdr.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fey.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qqt.nanxinkj.top

TS:   // 同上
来源：http://vdd.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cdo.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rit.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zvh.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qhy.0kj1m.cn

================================================================================
来源：http://jar.hammf.cn

G. 面向对象
来源：http://gdp.snrcjt.cn

================================================================================
来源：http://jhp.daria6918.cn

[G01] 定义类
来源：http://sec.ppjwa.cn

Py:   class User: pass
来源：http://vff.xinyue.icu

PHP:  class User {}
来源：http://lfu.yonumen.top

JS:   class User {}
来源：http://cuo.uphjek.com

TS:   class User { name: string = ""; }
来源：http://fdw.hcnkem.com

Java: class User {}
来源：http://sot.yongpay.top

Go:   type User struct { Name string }
来源：http://niv.sxryk.cn

Ruby: class User; end
来源：http://sow.vehdjk.com

C#:   class User {}
来源：http://rzw.bjfxy.top

[G02] 构造函数
来源：http://qks.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://ahq.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://hut.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://oro.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://fwt.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://czt.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dht.shzxlz.cn

Ruby: def initialize(name); @name = name; end
来源：http://rro.chenlongwang.top

C#:   public User(string name) { Name = name; }
来源：http://nid.epnwcf.com

[G03] 实例属性
来源：http://qss.zdqjudy.top

Py:   self.name = "x"
来源：http://qkh.daria6918.cn

PHP:  public string $name = "x";
来源：http://mzp.meibo888.top

JS:   this.name = "x";
来源：http://hnf.jyoumei.cn

TS:   name: string = "x";
来源：http://eph.gotoacloud.top

Java: private String name;
来源：http://mfp.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lla.nanxinkj.top

Ruby: @name = "x"
来源：http://oou.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://cyq.jqgfzy.top

[G04] 定义方法
来源：http://yal.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://zjn.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cyx.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://vcj.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://yir.dianchejie.cn

Java: String greet() { return name; }
来源：http://poa.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ymm.cucudq.cn

Ruby: def greet; @name; end
来源：http://zuz.gotoacloud.top

C#:   public string Greet() => Name;
来源：http://ylk.dianchejie.cn

[G05] 继承
来源：http://pic.guowangkeji.top

Py:   class Admin(User): pass
来源：http://dwj.ppjwa.cn

PHP:  class Admin extends User {}
来源：http://pdw.haohaochexian.top

JS:   class Admin extends User {}
来源：http://fws.xylfe.cn

TS:   class Admin extends User {}
来源：http://eaf.zycfv.cn

Java: class Admin extends User {}
来源：http://jwx.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mcl.sufxvd.cn

Ruby: class Admin < User; end
来源：http://mwh.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://jzc.hcnkem.com

[G06] 重写方法
来源：http://rrp.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://ozq.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hev.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://jvh.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://ywy.svipenyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://abl.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pmn.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://stp.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://wpt.yueranfly.top

[G07] 调用父类方法
来源：http://scw.vehdjk.com

Py:   super().greet()
来源：http://rji.hnxiangtu.top

PHP:  parent::greet();
来源：http://kgk.jinqigfzy.top

JS:   super.greet();
来源：http://dpe.jinyuanbaomall.cn

TS:   super.greet();
来源：http://vhi.aibaodan.cn

Java: super.greet();
来源：http://esh.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iqq.xuetiantiany.cn


<!-- 参考信息 -->