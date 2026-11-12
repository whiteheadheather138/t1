代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yla.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bya.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bmx.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wtm.fehbvm.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cqd.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://pgm.vehdjk.com

Py:   html.escape(s);  html.unescape(s)
来源：http://uub.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gbi.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dis.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://img.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kxu.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://omk.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://crw.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bnh.jianghu66.top

[E16] 数字千分位
来源：http://fll.yj20258888.top

Py:   f"{1234567:,}"
来源：http://shj.sufxvd.cn

PHP:  number_format(1234567);
来源：http://jua.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zrd.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cyo.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pyr.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://adm.chenlongwang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ejm.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://bwi.gotoacloud.top

[E17] 首字母大写
来源：http://biw.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lim.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fms.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oss.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vxq.9152youxi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nev.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uwl.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://zhg.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ymw.hywenlv.cn

[E18] 模板占位符替换
来源：http://htn.vehdjk.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://joa.sweek.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hbv.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bhv.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://nfl.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iis.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rxm.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://egr.snrcjt.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kya.yvedp.cn

[E19] 多行文本按行拆分
来源：http://lit.gzhubu.top

Py:   s.splitlines()
来源：http://sfe.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fnf.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://mwp.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://hvb.tanke756.top

Java: s.lines().toList()
来源：http://kmr.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://eqc.zhongyouzk.top

Ruby: s.lines
来源：http://fvn.meibo888.top

C#:   s.Split('\n')
来源：http://xac.52xcode.cn

[E20] 判断字符串是否为空
来源：http://maf.smart0.xyz

Py:   if not s:
来源：http://ftb.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cdg.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vog.yj202588.top

TS:   if (s === "") {}
来源：http://ewu.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://ues.jyoumei.cn

Go:   if s == "" {}
来源：http://twu.daria6918.cn

Ruby: if s.empty?
来源：http://ptg.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://emn.nanxinkj.top

[E21] 超长截断加省略号
来源：http://afn.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dbp.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lyb.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vvd.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kpi.cdnleiting.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pvw.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://yjt.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qty.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zgt.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://dod.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ntd.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xrn.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aki.havefunace.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wgu.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uzr.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://obo.gaohongyu789.top

Ruby: s.bytesize;  s.length
来源：http://yus.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cie.ivvv.top

================================================================================
来源：http://gkh.yj202588.top

F. 文件与目录
来源：http://vrq.vehdjk.com

================================================================================
来源：http://rug.sysykeji.top

[F01] 读取整个文件
来源：http://okj.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fhf.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://tiv.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lwy.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cyw.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dmh.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ddy.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://zek.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://acu.hcnkem.com

[F02] 逐行读取文件
来源：http://msl.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rka.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cfn.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yah.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hxs.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fdl.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://usc.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jca.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ckq.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://xrj.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ciw.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rvo.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wie.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://orj.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oyf.zdqjudy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yxm.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://wxo.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hhl.yueranfly.top

[F04] 追加写入文件
来源：http://bam.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tyk.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hcv.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://boj.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ecf.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fwe.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gdh.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ofj.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iil.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://hcn.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gzr.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://lot.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://npd.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://fwf.yj202588.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uld.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zdd.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://jom.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://lyr.jinyuanbaomall.cn

[F06] 删除文件
来源：http://tvz.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://nza.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://jsb.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://mof.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://yld.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cuq.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://lbt.316326.xyz

Ruby: File.delete("a.txt")
来源：http://rpg.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://peo.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://krj.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rqd.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://exp.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pqi.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tcp.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hte.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qsq.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ypu.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nug.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://oyw.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pjt.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mby.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://rez.yueranfly.top

TS:   fs.readdirSync("dir")
来源：http://wgr.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://psl.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xiq.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://nbt.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://zen.tarul.cn

[F09] 获取文件大小
来源：http://gdx.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://for.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://fbu.jlsjyb.cn

JS:   fs.statSync("a.txt").size
来源：http://xzu.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://itm.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://jlh.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nmw.vehdjk.com

Ruby: File.size("a.txt")
来源：http://crr.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://sll.shzxlz.cn

[F10] 取文件扩展名 / 文件名
来源：http://mpv.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baw.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://epb.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tzo.shuidangran.top

TS:   path.extname("a.txt")
来源：http://heh.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://otp.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gvu.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fwy.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ify.aizwys.cn

[F11] 复制与移动文件
来源：http://hgj.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://slx.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sed.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bth.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lou.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sjp.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ocd.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ret.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qlt.9152youxi.cn

[F12] CSV 读写
来源：http://cpt.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zlh.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hlk.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pki.chenjidiqi.icu

TS:   // 同上
来源：http://ito.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qrd.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fiv.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pli.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kwx.bjfxy.top

================================================================================
来源：http://jih.ywan-chungtsiang.top

G. 面向对象
来源：http://xnr.iojbl.cn

================================================================================
来源：http://rgt.pycfn.com

[G01] 定义类
来源：http://khw.meibo888.top

Py:   class User: pass
来源：http://dtl.zhixingplan.top

PHP:  class User {}
来源：http://kwa.fanxiaobao.xyz

JS:   class User {}
来源：http://rvf.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://lzy.hywenlv.cn

Java: class User {}
来源：http://sku.pycfn.com

Go:   type User struct { Name string }
来源：http://ivn.zhoulong.xyz

Ruby: class User; end
来源：http://wzo.wangshuangyany.cn

C#:   class User {}
来源：http://hph.ctjpmb.com

[G02] 构造函数
来源：http://jkp.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://yis.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://qdf.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://myq.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://pry.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://ktl.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kix.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://srk.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://wzs.aibaodan.cn

[G03] 实例属性
来源：http://frb.sjlbkw.cn

Py:   self.name = "x"
来源：http://sgz.shzxlz.cn

PHP:  public string $name = "x";
来源：http://psu.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://cnt.ydzc1.top

TS:   name: string = "x";
来源：http://bfo.zhaomingkeji.xyz

Java: private String name;
来源：http://ndb.xingfuxueyuan.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gzq.zdbjq.cn

Ruby: @name = "x"
来源：http://aev.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://jie.uphjek.com

[G04] 定义方法
来源：http://wih.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://cfa.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uan.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://jqn.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://izr.hnxiangtu.top

Java: String greet() { return name; }
来源：http://rdj.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vpi.guannengcc.top

Ruby: def greet; @name; end
来源：http://bql.vehdjk.com

C#:   public string Greet() => Name;
来源：http://puh.hysaishi.cn

[G05] 继承
来源：http://pah.yj20258.top

Py:   class Admin(User): pass
来源：http://cyw.jinqigufen.top

PHP:  class Admin extends User {}
来源：http://spc.chenlongwang.top

JS:   class Admin extends User {}
来源：http://gbj.c1oappe.top

TS:   class Admin extends User {}
来源：http://glg.ctjpmb.com

Java: class Admin extends User {}
来源：http://axb.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pzv.yongpay.top

Ruby: class Admin < User; end
来源：http://nol.epnwcf.com

C#:   class Admin : User {}
来源：http://mst.chenlongwang.top

[G06] 重写方法
来源：http://cpk.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://snp.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://bcf.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://hha.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://puq.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://ppx.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://coe.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://wbh.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://ozv.smart0.xyz

[G07] 调用父类方法
来源：http://bcj.fzhhl.top

Py:   super().greet()
来源：http://idq.316326.xyz

PHP:  parent::greet();
来源：http://hme.wangdashe.top

JS:   super.greet();
来源：http://ydk.jiagoushi.top

TS:   super.greet();
来源：http://osp.tarul.cn

Java: super.greet();
来源：http://tif.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hdd.yj202588.top

Ruby: super
来源：http://iwc.zhoulong.xyz

C#:   base.Greet();
来源：http://ncu.zhoulong.xyz

[G08] 静态方法与属性
来源：http://ohc.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://usu.gotoacloud.top

PHP:  public static function f() {}
来源：http://mrm.pycfn.com

JS:   static f() {}
来源：http://rvd.pycfn.com

TS:   static f(): void {}
来源：http://wbb.jiagoushi.top

Java: static void f() {}
来源：http://xak.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://yql.cashguo.top

Ruby: def self.f; end
来源：http://fny.ivvv.top

C#:   public static void F() {}
来源：http://ohq.hnqzz.top

[G09] 接口 / 抽象类
来源：http://ghn.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://fum.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://egx.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://rwm.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://shn.shuidangran.top

Java: interface Shape { double area(); }
来源：http://lwu.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://wmc.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ghw.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://cvs.fzhhl.top

[G10] 访问控制
来源：http://dni.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://gcv.wangshuangyany.cn

PHP:  public / protected / private
来源：http://pcu.ivvv.top

JS:   #private 字段；其余公开
来源：http://khn.yangfankeji.com

TS:   public / protected / private
来源：http://tcs.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://plh.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zev.chenzaomai.com

Ruby: public / protected / private
来源：http://jxt.xinyue.icu

C#:   public / protected / private / internal
来源：http://aoz.svipenyu.cn

[G11] getter / setter
来源：http://req.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://rth.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dmk.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://gbh.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://dty.havefunace.top

Java: public String getName() { return name; }
来源：http://mlh.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vvz.yj20258.top

Ruby: attr_accessor :name
来源：http://oip.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://hpa.zhixingplan.top

[G12] 对象转字符串
来源：http://jei.yongpay.top

Py:   def __str__(self): return self.name
来源：http://dfw.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qok.bjfxy.top

JS:   toString() { return this.name; }
来源：http://yxf.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://hge.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://ptc.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ftz.316326.xyz

Ruby: def to_s; @name; end
来源：http://ags.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://yyl.316326.xyz

[G13] 判断对象类型
来源：http://cka.zhoulong.xyz


<!-- 参考信息 -->