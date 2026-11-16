代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ckr.yongpay.top

[E11] 反转字符串
来源：http://smq.zdbjq.cn

Py:   s[::-1]
来源：http://qay.nanxuanxn.top

PHP:  strrev($s);
来源：http://cur.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://sej.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://afx.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zcl.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xaa.cucudq.cn

Ruby: s.reverse
来源：http://olx.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nvc.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://wfv.jqgufenzy.top

Py:   s.count("a")
来源：http://igl.wangshuangyany.cn

PHP:  substr_count($s, "a");
来源：http://ajt.meibo888.top

JS:   s.split("a").length - 1
来源：http://lnv.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://cje.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xae.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://jvp.sufxvd.cn

Ruby: s.count("a")
来源：http://dhz.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://jci.yfazqb.com

[E13] 逐字符遍历
来源：http://yth.yj20258.top

Py:   for ch in s: print(ch)
来源：http://mxh.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yuc.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cpu.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://wyf.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kpe.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nkc.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hty.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rkj.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://tgd.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dwq.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tlw.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gnc.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://plp.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dbr.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sai.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://chn.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sxc.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://ldi.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qsa.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://djq.zycfv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iup.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vpt.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hvi.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xjp.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tom.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://phs.birdmap.top

[E16] 数字千分位
来源：http://imk.xinyue.icu

Py:   f"{1234567:,}"
来源：http://gzb.tianlin.xyz

PHP:  number_format(1234567);
来源：http://fpa.nwbrower.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vab.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hip.birdmap.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wxg.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oxa.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gok.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://mxf.fanxiaobao.xyz

[E17] 首字母大写
来源：http://gvq.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zwy.snrcjt.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zvo.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hmw.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bte.quarkkingdee.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vgn.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ccu.gogol.net.cn

Ruby: s.capitalize
来源：http://qqe.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uly.chenzaomai.com

[E18] 模板占位符替换
来源：http://gxe.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mzk.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nok.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uso.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qlg.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wzt.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nnz.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dor.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hss.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://wtk.dianchejie.cn

Py:   s.splitlines()
来源：http://rzr.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nus.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://oxe.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://vzu.wangdashe.top

Java: s.lines().toList()
来源：http://dch.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://nsp.tianlin.xyz

Ruby: s.lines
来源：http://cuj.gogol.net.cn

C#:   s.Split('\n')
来源：http://mlu.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://wms.bbcook.cn

Py:   if not s:
来源：http://rwl.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ejz.shuidangran.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hnj.jinqigfzy.top

TS:   if (s === "") {}
来源：http://uyu.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://wrb.ydzc1.top

Go:   if s == "" {}
来源：http://aow.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://amt.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://liq.hywenlv.cn

[E21] 超长截断加省略号
来源：http://xzj.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pyo.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ste.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqm.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://heb.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tks.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://bzm.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://syx.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ltl.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://ebq.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rmf.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wxb.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vvo.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zha.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jqb.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qbi.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://kpj.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hoc.cdnleiting.top

================================================================================
来源：http://vqf.mhx1999.top

F. 文件与目录
来源：http://rwz.quarkkingdee.top

================================================================================
来源：http://adw.hongshengwenyu.top

[F01] 读取整个文件
来源：http://wol.svipenyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ekq.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://kyc.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://keo.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lly.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hue.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://psb.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://yvp.tanke756.top

C#:   File.ReadAllText("a.txt");
来源：http://pws.yueranfly.top

[F02] 逐行读取文件
来源：http://pjs.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ohv.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pdu.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lse.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tyb.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://voz.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mlv.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zti.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jvx.yj202588.top

[F03] 写入文件（覆盖）
来源：http://jrm.hnxiangtu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lrx.yonumen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zez.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nrx.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://azo.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pnk.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kbh.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://aja.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mhq.jiagoushi.top

[F04] 追加写入文件
来源：http://dwg.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zcl.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gxx.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lqp.chenjidiqi.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hdp.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fbd.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ged.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wwv.fengsongda.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xwc.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://xnj.bjfxy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://imk.cheryme.top

PHP:  file_exists("a.txt");
来源：http://hsu.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://ktk.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://dgl.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://grd.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oeg.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://ukr.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://syf.nanxuanxn.top

[F06] 删除文件
来源：http://ksv.bjfxy.top

Py:   os.remove("a.txt")
来源：http://kyu.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://znm.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://hyi.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://zza.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lmm.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://wlu.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://oxm.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://ooq.bjfxy.top

[F07] 创建目录（含多级）
来源：http://rlc.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pgs.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ntp.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kii.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mmx.dashuyun.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aka.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qqb.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hhd.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lnt.9152youxi.cn

[F08] 遍历目录
来源：http://zqd.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mbo.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eua.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://mur.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://ugz.gotoacloud.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rdd.hesvh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sqf.sweek.top

Ruby: Dir.children("dir")
来源：http://eds.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://nji.nanxuanxn.top

[F09] 获取文件大小
来源：http://qki.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://lui.fktsv.cn

PHP:  filesize("a.txt");
来源：http://wnq.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://xbn.meibo888.top

TS:   fs.statSync("a.txt").size
来源：http://eex.316326.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://nxx.daxiang520.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mfn.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://fdu.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://yqm.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://hex.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zmk.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hzq.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wjz.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://iqg.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xam.hesvh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wlh.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ajq.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vbu.daxiang520.top

[F11] 复制与移动文件
来源：http://tyk.shangyingyoupin.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gkr.snrcjt.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mqq.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xmo.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dhl.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://asb.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qbq.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://khe.jianghu66.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cku.bbcook.cn

[F12] CSV 读写
来源：http://wio.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hmy.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iwt.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://npo.shangyingyoupin.top

TS:   // 同上
来源：http://fuy.yj202588.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oqo.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yly.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zai.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xxf.feifeiyinyue.top

================================================================================
来源：http://vqi.ctjpmb.com

G. 面向对象
来源：http://xfs.vehdjk.com

================================================================================
来源：http://pje.daria6918.cn

[G01] 定义类
来源：http://xqf.wangdashe.top

Py:   class User: pass
来源：http://ljh.zdbjq.cn

PHP:  class User {}
来源：http://wll.zhongyouzk.top

JS:   class User {}
来源：http://fvg.tarul.cn

TS:   class User { name: string = ""; }
来源：http://eys.fanxiaobao.xyz

Java: class User {}
来源：http://btb.nwbrower.top

Go:   type User struct { Name string }
来源：http://nzo.chenlongwang.top

Ruby: class User; end
来源：http://rju.kuanghao11.cn

C#:   class User {}
来源：http://hlu.jinqigufen.top

[G02] 构造函数
来源：http://gow.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://blr.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://vzo.birdmap.top

JS:   constructor(name) { this.name = name; }
来源：http://gtv.tanke756.top

TS:   constructor(public name: string) {}
来源：http://pwk.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://ucc.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://npi.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://ukw.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://mqc.hnxiangtu.top

[G03] 实例属性
来源：http://xhy.daria6918.cn

Py:   self.name = "x"
来源：http://byf.sweek.top

PHP:  public string $name = "x";
来源：http://nub.yangfankeji.com

JS:   this.name = "x";
来源：http://efv.0kj1m.cn

TS:   name: string = "x";
来源：http://bjg.hywenlv.cn

Java: private String name;
来源：http://nvj.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xub.yj20258888.top

Ruby: @name = "x"
来源：http://uxd.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://uri.tianlin.xyz

[G04] 定义方法
来源：http://gha.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://efp.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://ohs.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://yag.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://nyi.zhengqikj.top

Java: String greet() { return name; }
来源：http://rqb.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mbo.xylfe.cn

Ruby: def greet; @name; end
来源：http://ppn.epnwcf.com

C#:   public string Greet() => Name;
来源：http://wpo.zdqjudy.top

[G05] 继承
来源：http://jfp.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://pmw.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://ntl.zhixingplan.top

JS:   class Admin extends User {}
来源：http://uci.tianlin.xyz

TS:   class Admin extends User {}
来源：http://qim.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://ftk.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hjz.tanke756.top

Ruby: class Admin < User; end
来源：http://mhm.sweek.top

C#:   class Admin : User {}
来源：http://tst.nanxinkj.top

[G06] 重写方法
来源：http://xtg.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://gmx.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://clg.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://vxo.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://ddq.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://jeu.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lpe.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://kot.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://jkq.jqgfzy.top

[G07] 调用父类方法
来源：http://vmq.gzhubu.top

Py:   super().greet()
来源：http://xrq.fehbvm.com

PHP:  parent::greet();
来源：http://jej.haohaochexian.top

JS:   super.greet();
来源：http://qfr.yanxiufei.cn

TS:   super.greet();
来源：http://svo.svipenyu.cn

Java: super.greet();
来源：http://fxj.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ycp.zhixingplan.top

Ruby: super
来源：http://ljm.bbcook.cn

C#:   base.Greet();
来源：http://vxu.yj20258888.top

[G08] 静态方法与属性
来源：http://inp.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pfl.yanxiufei.cn

PHP:  public static function f() {}
来源：http://xxl.chenjidiqi.icu

JS:   static f() {}
来源：http://jsq.chenzaomai.com

TS:   static f(): void {}
来源：http://gzt.zdqjudy.top

Java: static void f() {}
来源：http://lbe.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nwc.ppjwa.cn

Ruby: def self.f; end
来源：http://cra.yueranfly.top

C#:   public static void F() {}
来源：http://fkk.shuidangran.top

[G09] 接口 / 抽象类
来源：http://kzd.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://uox.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ppb.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hbm.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://ydf.ydzc1.top


<!-- 参考信息 -->