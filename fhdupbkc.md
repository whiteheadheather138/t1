代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://wbd.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dfn.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qai.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://cun.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://aew.yj202588.top

Java: String.format("%03d", 7)
来源：http://jvq.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://sdp.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qlf.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lrb.fktsv.cn

[E11] 反转字符串
来源：http://nxx.chenjidiqi.icu

Py:   s[::-1]
来源：http://cwg.gzhubu.top

PHP:  strrev($s);
来源：http://skg.tarul.cn

JS:   [...s].reverse().join("")
来源：http://izd.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://mhz.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pfh.jianghu66.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dgq.ywan-chungtsiang.top

Ruby: s.reverse
来源：http://kke.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://okt.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://mxc.hnxiangtu.top

Py:   s.count("a")
来源：http://pkx.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://ujz.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://kag.hammf.cn

TS:   s.split("a").length - 1
来源：http://lrb.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ehb.yonumen.top

Go:   strings.Count(s, "a")
来源：http://tuo.tianlin.xyz

Ruby: s.count("a")
来源：http://app.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://gfi.yueranfly.top

[E13] 逐字符遍历
来源：http://xuy.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://rxp.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ust.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ziz.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qnd.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://imb.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://elr.hfpthk.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://klv.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ppf.wangdashe.top

[E14] URL 编码与 Base64
来源：http://leu.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ekg.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vwa.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xjt.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dlf.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qyx.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://glg.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lyq.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zua.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://leo.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ufn.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://krq.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ecc.nanxinkj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fpt.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rmn.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://epa.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rtg.jinqigufen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wha.guannengcc.top

[E16] 数字千分位
来源：http://hmk.gzhubu.top

Py:   f"{1234567:,}"
来源：http://rgz.xziqi.cn

PHP:  number_format(1234567);
来源：http://ljk.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rbf.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qon.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://veb.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aux.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vwx.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://gec.fktsv.cn

[E17] 首字母大写
来源：http://oro.cqqwz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dfp.zhengqikj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vds.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qsa.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jkl.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lqo.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ito.nwbrower.top

Ruby: s.capitalize
来源：http://dgr.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jop.epnwcf.com

[E18] 模板占位符替换
来源：http://hfq.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jse.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://shx.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://jow.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rxx.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fjt.guannengcc.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cjc.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://phn.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wng.yuxming.cn

[E19] 多行文本按行拆分
来源：http://iut.yj20258.top

Py:   s.splitlines()
来源：http://iiz.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dwd.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://jep.dianchejie.cn

TS:   s.split(/\r?\n/)
来源：http://qbn.yvedp.cn

Java: s.lines().toList()
来源：http://dkk.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://bam.feifeiyinyue.top

Ruby: s.lines
来源：http://srs.c1oappe.top

C#:   s.Split('\n')
来源：http://nhv.daxiang520.top

[E20] 判断字符串是否为空
来源：http://ivk.uphjek.com

Py:   if not s:
来源：http://yhc.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://slv.guowangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jnt.ybcxt.top

TS:   if (s === "") {}
来源：http://ilq.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://rzt.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://msl.316326.xyz

Ruby: if s.empty?
来源：http://hoh.jinqigufen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dbc.ybcxt.top

[E21] 超长截断加省略号
来源：http://xjp.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bto.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ivw.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mnw.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://trs.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ygt.vehdjk.com

Go:   // 按 rune 判断长度后截断
来源：http://kos.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ynm.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oof.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://skg.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ifp.ivvv.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vql.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jqa.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uzh.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uce.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jef.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://tzq.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nkw.tianlin.xyz

================================================================================
来源：http://jco.nwbrower.top

F. 文件与目录
来源：http://cju.hnqzz.top

================================================================================
来源：http://vxk.bbcook.cn

[F01] 读取整个文件
来源：http://qng.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://edr.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://yqz.yj20258.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xdx.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vse.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://iwt.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://izy.yueranfly.top

Ruby: File.read("a.txt")
来源：http://qji.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://syy.daria6918.cn

[F02] 逐行读取文件
来源：http://ngb.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://azv.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xpu.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://khk.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pgw.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nnm.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aaq.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kly.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jfg.cashguo.top

[F03] 写入文件（覆盖）
来源：http://wqw.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sjx.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sfh.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vog.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yqq.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://isc.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gzu.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://fum.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nkk.epnwcf.com

[F04] 追加写入文件
来源：http://xre.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://agt.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wxl.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wuy.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yqo.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zpe.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ybz.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jwv.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ucb.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://thx.chenjidiqi.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jjd.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://uvw.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://pvq.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://uow.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://gtq.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zzf.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://yvh.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://lya.zhijiandao.cn

[F06] 删除文件
来源：http://bkj.pycfn.com

Py:   os.remove("a.txt")
来源：http://iau.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://hvs.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://jff.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://tfg.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ldo.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://rgk.zhaomingkeji.xyz

Ruby: File.delete("a.txt")
来源：http://dkx.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://kyr.cheryme.top

[F07] 创建目录（含多级）
来源：http://szl.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rar.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zki.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eja.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sxe.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uhx.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bzw.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://suw.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://alw.bbcook.cn

[F08] 遍历目录
来源：http://hnn.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oqb.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jsz.shzxlz.cn

JS:   fs.readdirSync("dir")
来源：http://oxq.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://bwd.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wxq.zhijiandao.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lin.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://rpz.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://aup.chenlongwang.top

[F09] 获取文件大小
来源：http://qmh.wangdashe.top

Py:   os.path.getsize("a.txt")
来源：http://zoe.fengsongda.top

PHP:  filesize("a.txt");
来源：http://miv.52xcode.cn

JS:   fs.statSync("a.txt").size
来源：http://tbl.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://qme.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://olm.yueranfly.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fzy.gogol.net.cn

Ruby: File.size("a.txt")
来源：http://ayv.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://mwe.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://fys.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nix.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rvx.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vwi.xylfe.cn

TS:   path.extname("a.txt")
来源：http://lrn.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yjm.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fyv.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ain.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://esf.yonumen.top

[F11] 复制与移动文件
来源：http://dkf.shanyushiyangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jei.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xgl.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oec.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uxk.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ctk.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dso.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ylv.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gof.sjlbkw.cn

[F12] CSV 读写
来源：http://xwe.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hrn.yfazqb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://skr.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ewy.jyoumei.cn

TS:   // 同上
来源：http://ycd.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bth.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xlb.jianghu66.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jxj.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://czy.meibo888.top

================================================================================
来源：http://epw.hammf.cn

G. 面向对象
来源：http://xfe.shuidangran.top

================================================================================
来源：http://ybz.sweek.top

[G01] 定义类
来源：http://yhc.shuidangran.top

Py:   class User: pass
来源：http://ayr.yueranfly.top

PHP:  class User {}
来源：http://lcj.yuanzhike.top

JS:   class User {}
来源：http://qzr.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://dds.havefunace.top

Java: class User {}
来源：http://asl.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://yhn.mhx1999.top

Ruby: class User; end
来源：http://bsg.nanxinkj.top

C#:   class User {}
来源：http://lqf.redwolf501.top

[G02] 构造函数
来源：http://xma.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://the.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://hxu.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://lpi.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://bdt.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://vcb.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pwf.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://vml.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://ged.52xcode.cn

[G03] 实例属性
来源：http://ltf.zdqjudy.top

Py:   self.name = "x"
来源：http://qpf.yj202588.top

PHP:  public string $name = "x";
来源：http://azx.hesvh.cn

JS:   this.name = "x";
来源：http://blg.fktsv.cn

TS:   name: string = "x";
来源：http://qqb.nanxuanxn.top

Java: private String name;
来源：http://pxx.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://syx.yj20258.top

Ruby: @name = "x"
来源：http://rop.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://wri.yfazqb.com

[G04] 定义方法
来源：http://xhy.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://klf.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sxv.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://hel.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://vbf.yonumen.top

Java: String greet() { return name; }
来源：http://bez.zdqjudy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gnc.tarul.cn

Ruby: def greet; @name; end
来源：http://qrn.sysykeji.top

C#:   public string Greet() => Name;
来源：http://uuq.pengpengdd.cyou

[G05] 继承
来源：http://qjq.sweek.top

Py:   class Admin(User): pass
来源：http://cgm.tian-w.cn

PHP:  class Admin extends User {}
来源：http://yca.zycfv.cn

JS:   class Admin extends User {}
来源：http://ewe.fengsongda.top

TS:   class Admin extends User {}
来源：http://mzf.zhoulong.xyz

Java: class Admin extends User {}
来源：http://vtu.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sch.ywan-chungtsiang.top

Ruby: class Admin < User; end
来源：http://jvg.jinqigfzy.top

C#:   class Admin : User {}
来源：http://wrb.tian-w.cn

[G06] 重写方法
来源：http://not.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://lfz.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cbt.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://sjm.cheryme.top

TS:   greet(): string { return "admin"; }
来源：http://spi.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://enn.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qed.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://nbp.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://aaj.birdmap.top

[G07] 调用父类方法
来源：http://clw.yanxiufei.cn

Py:   super().greet()
来源：http://que.hcnkem.com

PHP:  parent::greet();
来源：http://rta.aizwys.cn

JS:   super.greet();
来源：http://rlh.hcnkem.com

TS:   super.greet();
来源：http://ygs.gaohongyu789.top

Java: super.greet();
来源：http://zbw.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ynk.dashuyun.cn

Ruby: super
来源：http://boe.52xcode.cn

C#:   base.Greet();
来源：http://uqk.zhengqikj.top

[G08] 静态方法与属性
来源：http://hwi.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uql.uphjek.com

PHP:  public static function f() {}
来源：http://okn.yvedp.cn

JS:   static f() {}
来源：http://igo.316326.xyz

TS:   static f(): void {}
来源：http://hys.zhaomingkeji.xyz

Java: static void f() {}
来源：http://fsi.uphjek.com


<!-- 参考信息 -->