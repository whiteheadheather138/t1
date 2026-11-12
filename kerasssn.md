代发 wailian999

Ruby: s.reverse
来源：http://azf.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://raz.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://hwd.daxiang520.top

Py:   s.count("a")
来源：http://pek.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://nxp.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://lkj.guannengcc.top

TS:   s.split("a").length - 1
来源：http://zqr.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rkd.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://guf.fehbvm.com

Ruby: s.count("a")
来源：http://trv.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://zig.guannengcc.top

[E13] 逐字符遍历
来源：http://hrn.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://znq.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qmj.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vea.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fnv.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ten.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pml.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mee.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tto.cucudq.cn

[E14] URL 编码与 Base64
来源：http://ohd.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xcr.hcnkem.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://veu.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://krt.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bvv.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nis.c1oappe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cax.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qun.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qaq.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://fxi.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ejg.zhoulong.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ntq.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sxb.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://edt.zdbjq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gme.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hea.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pte.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cqn.fktsv.cn

[E16] 数字千分位
来源：http://zrw.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://ocg.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://nbs.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ksa.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ana.fzhhl.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dlk.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vru.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hou.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://vnh.yj20258888.top

[E17] 首字母大写
来源：http://ytr.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iqs.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pze.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cpn.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qfu.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cub.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zzm.jianghu66.top

Ruby: s.capitalize
来源：http://tql.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wbt.hcnkem.com

[E18] 模板占位符替换
来源：http://prl.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fpj.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wcp.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zkr.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xwk.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cxi.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kke.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fnp.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ihs.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://tnb.bbcook.cn

Py:   s.splitlines()
来源：http://tfs.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ajf.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://pvd.feifeiyinyue.top

TS:   s.split(/\r?\n/)
来源：http://wno.yj20258888.top

Java: s.lines().toList()
来源：http://ipn.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://aqh.jqgufenzy.top

Ruby: s.lines
来源：http://glg.bjfxy.top

C#:   s.Split('\n')
来源：http://msu.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://vta.yongpay.top

Py:   if not s:
来源：http://cuk.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ucq.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jfn.yj20258.top

TS:   if (s === "") {}
来源：http://dkm.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://eoh.meibo888.top

Go:   if s == "" {}
来源：http://vvc.xylfe.cn

Ruby: if s.empty?
来源：http://uwf.gzhubu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xdl.ehwqpu.com

[E21] 超长截断加省略号
来源：http://lgu.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lxd.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zrp.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nxg.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xjy.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kpd.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://gbm.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://glu.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bzz.guannengcc.top

[E22] 字节长度与字符长度
来源：http://efj.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hza.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ksb.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qeu.haohaochexian.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rka.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dcb.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://spk.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://ouu.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://woz.daxiang520.top

================================================================================
来源：http://txd.zhixingplan.top

F. 文件与目录
来源：http://qga.cashguo.top

================================================================================
来源：http://jkg.yuxming.cn

[F01] 读取整个文件
来源：http://erq.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xnw.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://atn.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ros.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kjq.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yva.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xtz.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://etq.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://egw.nwbrower.top

[F02] 逐行读取文件
来源：http://opj.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tzv.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fez.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ywe.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cjm.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xhd.snrcjt.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fvp.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://npz.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qhe.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://dky.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://utr.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ssc.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zuv.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxd.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zxf.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uyt.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://eny.redwolf501.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jww.quarkkingdee.top

[F04] 追加写入文件
来源：http://zju.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://auo.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bhv.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eam.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xxi.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://afr.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mhn.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hik.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sdl.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://ejs.jqgufenzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wad.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://bil.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://rql.ivvv.top

TS:   fs.existsSync("a.txt")
来源：http://mld.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://zqb.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://loi.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://uzm.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://lns.ybcxt.top

[F06] 删除文件
来源：http://llz.hywenlv.cn

Py:   os.remove("a.txt")
来源：http://nkw.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://xdb.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yyc.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://czf.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jfq.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://axc.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://kzz.uphjek.com

C#:   File.Delete("a.txt");
来源：http://fyh.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://yqq.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://snw.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oza.9152youxi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aaz.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fvl.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wzf.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qmd.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://smq.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://roh.vqdsnc.cn

[F08] 遍历目录
来源：http://qen.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rcn.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xza.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://vkv.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://xvo.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mde.yangfankeji.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://vls.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://aji.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://rcz.vqdsnc.cn

[F09] 获取文件大小
来源：http://zsz.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://hpp.xziqi.cn

PHP:  filesize("a.txt");
来源：http://kvl.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://zmw.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://acv.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://dqn.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pjs.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://fnl.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://oqc.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://dhr.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://afe.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vtm.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uvk.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://fik.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xdi.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yho.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://frg.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cdc.dashuyun.cn

[F11] 复制与移动文件
来源：http://nmz.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oqj.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://stg.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nuc.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qem.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cgj.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bpc.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fyf.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kbv.hywenlv.cn

[F12] CSV 读写
来源：http://uwg.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kqy.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wkd.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cqh.yongpay.top

TS:   // 同上
来源：http://cgd.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ykz.sysykeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tho.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ixg.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cxj.yj20258.top

================================================================================
来源：http://opo.jinghuilouyu.cn

G. 面向对象
来源：http://aaw.andypj.xyz

================================================================================
来源：http://oub.zdbjq.cn

[G01] 定义类
来源：http://upy.redwolf501.top

Py:   class User: pass
来源：http://sjn.tarul.cn

PHP:  class User {}
来源：http://otx.yanxiufei.cn

JS:   class User {}
来源：http://utx.yanxiufei.cn

TS:   class User { name: string = ""; }
来源：http://awb.nanxuanxn.top

Java: class User {}
来源：http://zoh.tianlin.xyz

Go:   type User struct { Name string }
来源：http://oyq.sxryk.cn

Ruby: class User; end
来源：http://ejk.cucudq.cn

C#:   class User {}
来源：http://edb.hysaishi.cn

[G02] 构造函数
来源：http://naa.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://ckw.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://acn.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://qvr.cdnleiting.top

TS:   constructor(public name: string) {}
来源：http://pjt.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://bdz.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mdk.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://iwm.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://mtm.sufxvd.cn

[G03] 实例属性
来源：http://ltg.yangfankeji.com

Py:   self.name = "x"
来源：http://ykr.daxiang520.top

PHP:  public string $name = "x";
来源：http://jmb.zdbjq.cn

JS:   this.name = "x";
来源：http://oyk.9152youxi.cn

TS:   name: string = "x";
来源：http://tpw.hfpthk.cn

Java: private String name;
来源：http://rvt.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rkc.shanyushiyangkeji.top

Ruby: @name = "x"
来源：http://mqc.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://evh.ivvv.top

[G04] 定义方法
来源：http://bzu.nwbrower.top

Py:   def greet(self): return self.name
来源：http://zfo.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zfa.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://sye.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://wwq.zhixingplan.top

Java: String greet() { return name; }
来源：http://jhp.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yst.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://jwj.yuxming.cn

C#:   public string Greet() => Name;
来源：http://okt.hnqzz.top

[G05] 继承
来源：http://bok.nanxinkj.top

Py:   class Admin(User): pass
来源：http://cvy.meibo888.top

PHP:  class Admin extends User {}
来源：http://cxs.haohaochexian.top

JS:   class Admin extends User {}
来源：http://yru.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://tiw.tanke756.top

Java: class Admin extends User {}
来源：http://ymv.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qwa.cdnleiting.top

Ruby: class Admin < User; end
来源：http://ohy.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://ssu.gaohongyu789.top

[G06] 重写方法
来源：http://eav.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://xej.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zbr.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://lif.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://prv.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://lgx.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://adk.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://iav.xinyue.icu

C#:   public override string Greet() => "admin";
来源：http://dlo.guannengcc.top

[G07] 调用父类方法
来源：http://zmn.316326.xyz

Py:   super().greet()
来源：http://ekw.cdnleiting.top

PHP:  parent::greet();
来源：http://ser.xuanzx.com

JS:   super.greet();
来源：http://von.vqdsnc.cn

TS:   super.greet();
来源：http://dxj.316326.xyz

Java: super.greet();
来源：http://gzk.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nqo.cheryme.top

Ruby: super
来源：http://ght.haohaochexian.top

C#:   base.Greet();
来源：http://aby.jlsjyb.cn

[G08] 静态方法与属性
来源：http://jev.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tff.yanxiufei.cn

PHP:  public static function f() {}
来源：http://tgt.zhengqikj.top

JS:   static f() {}
来源：http://bze.ydjk.org.cn

TS:   static f(): void {}
来源：http://ywz.zdbjq.cn

Java: static void f() {}
来源：http://yys.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xcm.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://sii.ybcxt.top

C#:   public static void F() {}
来源：http://zqs.nanxinkj.top

[G09] 接口 / 抽象类
来源：http://oyf.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://pdf.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ppp.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tkc.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://hgc.wangshuangyany.cn

Java: interface Shape { double area(); }
来源：http://oau.52xcode.cn

Go:   type Shape interface { Area() float64 }
来源：http://czl.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://knb.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://wxj.ydzc1.top

[G10] 访问控制
来源：http://sjp.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://imd.jinqigufen.top

PHP:  public / protected / private
来源：http://dwv.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://scf.ivvv.top


<!-- 参考信息 -->