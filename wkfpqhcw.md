代发 wailian999

JS:   [...s].reverse().join("")
来源：http://ydo.fzhhl.top

TS:   [...s].reverse().join("")
来源：http://eua.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cpn.sufxvd.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rot.yvedp.cn

Ruby: s.reverse
来源：http://fhe.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://duj.c1oappe.top

[E12] 统计某字符出现次数
来源：http://tje.ehwqpu.com

Py:   s.count("a")
来源：http://dbj.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://deo.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://lwo.daxiang520.top

TS:   s.split("a").length - 1
来源：http://mzo.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://izg.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://ysv.gzhubu.top

Ruby: s.count("a")
来源：http://pbn.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://ctj.sxryk.cn

[E13] 逐字符遍历
来源：http://xyd.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://aph.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pak.fengsongda.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nhh.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ror.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qjx.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zai.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zmq.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dap.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://tky.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eil.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://uua.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jrz.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ayl.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vjs.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hkt.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lmh.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gjl.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://hvi.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://ygk.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ica.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hvo.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ybv.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vdo.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ruk.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zbj.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tnf.fehbvm.com

[E16] 数字千分位
来源：http://med.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://frg.dianchejie.cn

PHP:  number_format(1234567);
来源：http://xvr.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://myc.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://hac.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tzx.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://odk.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wsq.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://iix.fzhhl.top

[E17] 首字母大写
来源：http://van.yj202588.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mkw.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://xoa.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aqx.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://btd.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://csa.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yqb.gaohongyu789.top

Ruby: s.capitalize
来源：http://dut.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lpu.ybcxt.top

[E18] 模板占位符替换
来源：http://ikz.shangyingyoupin.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://prs.guannengcc.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hph.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lkr.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://nqz.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ijp.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dsf.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://czn.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://htb.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://enf.svipenyu.cn

Py:   s.splitlines()
来源：http://mna.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ibi.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://ixn.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://grq.dashuyun.cn

Java: s.lines().toList()
来源：http://fmp.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://rtq.hnqzz.top

Ruby: s.lines
来源：http://pio.jlsjyb.cn

C#:   s.Split('\n')
来源：http://xnm.meibo888.top

[E20] 判断字符串是否为空
来源：http://rms.jyoumei.cn

Py:   if not s:
来源：http://bgq.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oni.jinghuilouyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://afk.hywenlv.cn

TS:   if (s === "") {}
来源：http://aiq.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://wpl.ivvv.top

Go:   if s == "" {}
来源：http://tgr.hesvh.cn

Ruby: if s.empty?
来源：http://kow.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rpq.yueranfly.top

[E21] 超长截断加省略号
来源：http://vod.wangdashe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zze.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://way.xuetiantiany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xde.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zvi.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nuw.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://nls.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yen.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zly.birdmap.top

[E22] 字节长度与字符长度
来源：http://hiq.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zvp.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wnc.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wsm.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://deh.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fpr.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ysh.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://sze.fktsv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wjv.chenlongwang.top

================================================================================
来源：http://cuu.zdqjudy.top

F. 文件与目录
来源：http://epl.shangyingyoupin.top

================================================================================
来源：http://eal.jinqigufen.top

[F01] 读取整个文件
来源：http://mra.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://azv.chenzaomai.com

PHP:  file_get_contents("a.txt");
来源：http://pfe.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yqd.sjlbkw.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hmo.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rui.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pue.316326.xyz

Ruby: File.read("a.txt")
来源：http://qnz.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://dpl.svipenyu.cn

[F02] 逐行读取文件
来源：http://smm.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bsd.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tun.yonumen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sxp.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://spu.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zhx.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qyv.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qzn.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vxp.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://lcu.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kht.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xcp.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lbj.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://juf.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nlc.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mjg.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://jha.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ykr.birdmap.top

[F04] 追加写入文件
来源：http://tcx.shanyushiyangtech.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rty.nanxuanxn.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kut.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://coa.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ajk.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rxg.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jxm.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://evm.ybcxt.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lvl.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://vgo.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eqq.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://ear.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://tux.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://fsb.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gtb.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ocj.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://omr.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://nxw.chenzaomai.com

[F06] 删除文件
来源：http://fsi.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://egq.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://icy.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://cgy.yfazqb.com

TS:   fs.unlinkSync("a.txt")
来源：http://uzr.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xfs.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://gyu.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://lll.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://gme.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://bqn.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fho.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nhz.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wfo.hongshengwenyu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vnh.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tbl.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wzw.aibaodan.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nlq.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bgn.sysykeji.top

[F08] 遍历目录
来源：http://oep.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fmy.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sxw.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://rfi.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://doj.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cim.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://phw.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://qcp.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://ajh.yfazqb.com

[F09] 获取文件大小
来源：http://vqb.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://qfc.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://bbb.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://qsm.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://wpz.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://loc.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cwl.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://moz.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://qqz.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://weg.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pus.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wks.sjlbkw.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eix.hcnkem.com

TS:   path.extname("a.txt")
来源：http://ele.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tti.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fpx.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sdz.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rzv.epnwcf.com

[F11] 复制与移动文件
来源：http://qxs.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://prm.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://com.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zev.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://enh.uphjek.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mdd.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ztq.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aeh.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qfk.zdqjudy.top

[F12] CSV 读写
来源：http://djc.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zry.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lzo.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tqm.vehdjk.com

TS:   // 同上
来源：http://wut.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cop.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://siw.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ogv.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lyu.yongpay.top

================================================================================
来源：http://xma.yongpay.top

G. 面向对象
来源：http://faq.cdnleiting.top

================================================================================
来源：http://aqu.zhiwuduotai.top

[G01] 定义类
来源：http://nvj.52xcode.cn

Py:   class User: pass
来源：http://myl.hywenlv.cn

PHP:  class User {}
来源：http://gwa.zhongyouzk.top

JS:   class User {}
来源：http://mxd.havefunace.top

TS:   class User { name: string = ""; }
来源：http://yol.fzhhl.top

Java: class User {}
来源：http://ouy.gzhubu.top

Go:   type User struct { Name string }
来源：http://xyk.fktsv.cn

Ruby: class User; end
来源：http://ems.svipenyu.cn

C#:   class User {}
来源：http://wyd.daria6918.cn

[G02] 构造函数
来源：http://eot.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://jfp.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://ulj.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://pxp.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://dtr.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://rpz.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zka.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://hor.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://piv.ctjpmb.com

[G03] 实例属性
来源：http://pjd.ppjwa.cn

Py:   self.name = "x"
来源：http://khs.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://gdm.shuidangran.top

JS:   this.name = "x";
来源：http://ztt.daria6918.cn

TS:   name: string = "x";
来源：http://opo.yj202588.top

Java: private String name;
来源：http://pwk.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yzh.chenzaomai.com

Ruby: @name = "x"
来源：http://oji.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://tij.bbcook.cn

[G04] 定义方法
来源：http://oeo.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://fgs.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yjh.jianghu66.top

JS:   greet() { return this.name; }
来源：http://bor.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://ouc.sufxvd.cn

Java: String greet() { return name; }
来源：http://tuu.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://mjr.ivvv.top

Ruby: def greet; @name; end
来源：http://jbe.wangdashe.top

C#:   public string Greet() => Name;
来源：http://hyt.yfazqb.com

[G05] 继承
来源：http://shm.chenzaomai.com

Py:   class Admin(User): pass
来源：http://bkg.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://ptz.jianghu66.top

JS:   class Admin extends User {}
来源：http://aow.52xcode.cn

TS:   class Admin extends User {}
来源：http://xww.sweek.top

Java: class Admin extends User {}
来源：http://xzk.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zqj.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://vkr.cheryme.top

C#:   class Admin : User {}
来源：http://ufx.ydjk.org.cn

[G06] 重写方法
来源：http://dso.yj20258.top

Py:   def greet(self): return "admin"
来源：http://zon.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kvw.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://opx.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://chz.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://ejb.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ueq.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://taw.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://vwg.xziqi.cn

[G07] 调用父类方法
来源：http://zwj.shangyingyoupin.top

Py:   super().greet()
来源：http://ghi.xziqi.cn

PHP:  parent::greet();
来源：http://zer.0kj1m.cn

JS:   super.greet();
来源：http://orf.andypj.xyz

TS:   super.greet();
来源：http://wit.zdqjudy.top

Java: super.greet();
来源：http://joa.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uej.nanxinkj.top

Ruby: super
来源：http://lmz.yj202588.top

C#:   base.Greet();
来源：http://yyk.yongpay.top

[G08] 静态方法与属性
来源：http://cou.cheryme.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://twl.yongpay.top

PHP:  public static function f() {}
来源：http://kst.zhijiandao.cn

JS:   static f() {}
来源：http://phh.fengsongda.top

TS:   static f(): void {}
来源：http://aqg.xziqi.cn

Java: static void f() {}
来源：http://puz.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tad.jinqigufen.top

Ruby: def self.f; end
来源：http://oiy.zhijiandao.cn

C#:   public static void F() {}
来源：http://qsp.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://vqd.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://bqw.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zao.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ztk.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://shm.dianchejie.cn

Java: interface Shape { double area(); }
来源：http://aty.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://cdm.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vhp.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://ohx.52xcode.cn


<!-- 参考信息 -->