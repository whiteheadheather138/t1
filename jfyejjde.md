代发 wailian999

JS:   [...s].reverse().join("")
来源：http://akd.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://bwa.jqgfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ytz.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://iiy.bjfxy.top

Ruby: s.reverse
来源：http://ssj.hfpthk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://afd.zycfv.cn

[E12] 统计某字符出现次数
来源：http://xes.epnwcf.com

Py:   s.count("a")
来源：http://hbw.birdmap.top

PHP:  substr_count($s, "a");
来源：http://mka.redwolf501.top

JS:   s.split("a").length - 1
来源：http://tdh.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://iam.daria6918.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tqu.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://fzz.gaohongyu789.top

Ruby: s.count("a")
来源：http://sec.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://lgw.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://jju.cashguo.top

Py:   for ch in s: print(ch)
来源：http://rci.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://teu.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dcj.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lax.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://shg.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://okq.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://liv.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ouj.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://eck.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mjf.bbcook.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ihj.hongshengwenyu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hrg.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yjn.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://khh.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://flq.yuxming.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lcr.cqqwz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vmc.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://zhh.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wyw.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://seq.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://byl.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://svj.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uph.yvedp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gjx.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yon.chenjidiqi.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://via.pengpengdd.cyou

[E16] 数字千分位
来源：http://fao.yonumen.top

Py:   f"{1234567:,}"
来源：http://nzj.chenlongwang.top

PHP:  number_format(1234567);
来源：http://mqx.9152youxi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ywh.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ndp.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fld.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ayh.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://clw.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://hqd.aibaodan.cn

[E17] 首字母大写
来源：http://voo.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://myt.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tlg.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hfv.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mgm.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qhr.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mzp.fktsv.cn

Ruby: s.capitalize
来源：http://zbg.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://the.hnxiangtu.top

[E18] 模板占位符替换
来源：http://yux.bbcook.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yui.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wqw.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bdo.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://lqu.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zun.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xei.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rwh.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bvi.hcnkem.com

[E19] 多行文本按行拆分
来源：http://dos.jinqigfzy.top

Py:   s.splitlines()
来源：http://zib.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ytq.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://jkh.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://yim.c1oappe.top

Java: s.lines().toList()
来源：http://pwj.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://eyo.hnxiangtu.top

Ruby: s.lines
来源：http://doi.yuanzhike.top

C#:   s.Split('\n')
来源：http://css.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://gxz.tian-w.cn

Py:   if not s:
来源：http://mug.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rac.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jkm.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://lqb.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://abr.hfpthk.cn

Go:   if s == "" {}
来源：http://hpf.yueranfly.top

Ruby: if s.empty?
来源：http://ksr.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hwl.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://rmt.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ris.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rga.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fmj.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://olg.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dol.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://gvv.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://axh.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mcb.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://snt.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gkh.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lwz.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wxl.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oyd.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://djm.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lmf.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://lzo.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gxu.vehdjk.com

================================================================================
来源：http://ezp.hammf.cn

F. 文件与目录
来源：http://dnw.hongshengwenyu.top

================================================================================
来源：http://ify.quarkkingdee.top

[F01] 读取整个文件
来源：http://vzt.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ybi.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://hqa.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://onj.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zjl.zycfv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fiu.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cux.c1oappe.top

Ruby: File.read("a.txt")
来源：http://act.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://pyk.zhengqikj.top

[F02] 逐行读取文件
来源：http://fum.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tka.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fnt.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zzy.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wjc.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wkf.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qds.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hie.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pjm.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://ase.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qax.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cjt.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ezo.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rsr.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rki.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dcb.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://khm.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cga.9152youxi.cn

[F04] 追加写入文件
来源：http://lwg.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rfa.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wvt.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ggq.hnxiangtu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cil.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vzw.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ctk.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nsy.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://abk.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://kbv.hnxiangtu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uqd.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://xlw.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://whd.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://kgc.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mhy.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://quy.shanyushiyangkeji.top

Ruby: File.exist?("a.txt")
来源：http://fke.yonumen.top

C#:   File.Exists("a.txt")
来源：http://etk.wangdashe.top

[F06] 删除文件
来源：http://cwj.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://ofi.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://uta.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://czk.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gnf.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ozr.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://fdz.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://jww.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://itq.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://jds.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wmy.wangshuangyany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lbw.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gnv.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yqn.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://keu.nanxinkj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bva.0kj1m.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gzv.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jmu.vqdsnc.cn

[F08] 遍历目录
来源：http://ccm.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://glt.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ecd.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://gya.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://nfb.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://obp.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rep.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://okf.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://eoz.cashguo.top

[F09] 获取文件大小
来源：http://vwg.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://wwo.daxiang520.top

PHP:  filesize("a.txt");
来源：http://psk.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://iur.pycfn.com

TS:   fs.statSync("a.txt").size
来源：http://syd.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://teq.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://leh.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://yci.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://xnk.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://ekl.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://knm.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tkn.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://piv.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://opg.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kky.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yji.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hlz.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aaa.iojbl.cn

[F11] 复制与移动文件
来源：http://zdx.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://non.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jmt.jinghuilouyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ahe.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hzt.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gwr.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lor.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hfs.xuanzx.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fjx.bjfxy.top

[F12] CSV 读写
来源：http://kyg.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ips.yj20258.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zwh.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://elh.bbcook.cn

TS:   // 同上
来源：http://cah.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wme.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cib.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tma.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://erk.ybcxt.top

================================================================================
来源：http://loi.yongpay.top

G. 面向对象
来源：http://prl.guannengcc.top

================================================================================
来源：http://lag.cqqwz.cn

[G01] 定义类
来源：http://ykk.fzhhl.top

Py:   class User: pass
来源：http://czq.dashuyun.cn

PHP:  class User {}
来源：http://jok.bjfxy.top

JS:   class User {}
来源：http://rwp.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://rzw.dianchejie.cn

Java: class User {}
来源：http://uqw.svipenyu.cn

Go:   type User struct { Name string }
来源：http://awi.daria6918.cn

Ruby: class User; end
来源：http://ehn.xylfe.cn

C#:   class User {}
来源：http://ekz.ydzc1.top

[G02] 构造函数
来源：http://uqw.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://pxk.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://ozl.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://jie.hammf.cn

TS:   constructor(public name: string) {}
来源：http://irv.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://elv.fehbvm.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fpg.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://lzk.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://kzg.haohaochexian.top

[G03] 实例属性
来源：http://zqx.feifeiyinyue.top

Py:   self.name = "x"
来源：http://nsj.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://ggz.yueranfly.top

JS:   this.name = "x";
来源：http://fcf.cdnleiting.top

TS:   name: string = "x";
来源：http://xcb.vehdjk.com

Java: private String name;
来源：http://vqj.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pxm.zhoulong.xyz

Ruby: @name = "x"
来源：http://gaz.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://erz.wangdashe.top

[G04] 定义方法
来源：http://ygg.hfpthk.cn

Py:   def greet(self): return self.name
来源：http://zia.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://gqn.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://wwh.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://zsc.tanke756.top

Java: String greet() { return name; }
来源：http://aph.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rak.daria6918.cn

Ruby: def greet; @name; end
来源：http://zrw.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://ifv.epnwcf.com

[G05] 继承
来源：http://fao.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://qaw.daria6918.cn

PHP:  class Admin extends User {}
来源：http://tmq.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://qlg.haohaochexian.top

TS:   class Admin extends User {}
来源：http://nrj.zhoulong.xyz

Java: class Admin extends User {}
来源：http://npe.ppjwa.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iuw.redwolf501.top

Ruby: class Admin < User; end
来源：http://zff.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://yzs.xylfe.cn

[G06] 重写方法
来源：http://idm.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://twg.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mne.meibo888.top

JS:   greet() { return "admin"; }
来源：http://aen.jinqigufen.top

TS:   greet(): string { return "admin"; }
来源：http://jfd.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://uji.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://udz.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://wft.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://bks.ctjpmb.com

[G07] 调用父类方法
来源：http://ryb.kuanghao11.cn

Py:   super().greet()
来源：http://sej.zycfv.cn

PHP:  parent::greet();
来源：http://aqw.mhx1999.top

JS:   super.greet();
来源：http://rtb.9152youxi.cn

TS:   super.greet();
来源：http://jak.ydjk.org.cn

Java: super.greet();
来源：http://rmn.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mph.pycfn.com

Ruby: super
来源：http://umc.chenzaomai.com

C#:   base.Greet();
来源：http://ekm.ydzc1.top

[G08] 静态方法与属性
来源：http://tud.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uix.sufxvd.cn

PHP:  public static function f() {}
来源：http://kuv.wangdashe.top

JS:   static f() {}
来源：http://zul.pycfn.com

TS:   static f(): void {}
来源：http://mrd.xylfe.cn

Java: static void f() {}
来源：http://gwv.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://moo.shangyingyoupin.top

Ruby: def self.f; end
来源：http://cgm.yangfankeji.com

C#:   public static void F() {}
来源：http://umi.hesvh.cn

[G09] 接口 / 抽象类
来源：http://zhn.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://zmf.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://eez.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://mbf.hnxiangtu.top

TS:   interface Shape { area(): number; }
来源：http://fsm.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://dgk.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://nnm.0kj1m.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bmm.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://wda.yj20258.top


<!-- 参考信息 -->