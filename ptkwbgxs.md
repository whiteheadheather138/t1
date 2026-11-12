代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aqt.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://vhn.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nvs.chenjidiqi.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://buy.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cnn.hammf.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xwl.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://htf.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://san.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://les.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://svs.shanyushiyangtech.top

[E16] 数字千分位
来源：http://whe.bjfxy.top

Py:   f"{1234567:,}"
来源：http://gch.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://xby.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://iyz.yj202588.top

TS:   (1234567).toLocaleString("en-US")
来源：http://obd.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pex.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://amn.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tmr.sufxvd.cn

C#:   1234567.ToString("N0")
来源：http://qrz.xingfuxueyuan.xyz

[E17] 首字母大写
来源：http://sva.cqqwz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oks.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ccz.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://otb.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wsw.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ddz.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://esd.c1oappe.top

Ruby: s.capitalize
来源：http://nwg.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dce.jlsjyb.cn

[E18] 模板占位符替换
来源：http://jgh.bjfxy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nfz.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qpa.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nzn.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yhu.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fdi.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tpk.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ncq.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vnj.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://tie.yuanzhike.top

Py:   s.splitlines()
来源：http://ado.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jwz.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://mzg.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://sce.cashguo.top

Java: s.lines().toList()
来源：http://gtm.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://zse.cashguo.top

Ruby: s.lines
来源：http://zoi.epnwcf.com

C#:   s.Split('\n')
来源：http://sow.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://pzu.52xcode.cn

Py:   if not s:
来源：http://uhp.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vwm.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pnq.bjfxy.top

TS:   if (s === "") {}
来源：http://qnc.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://ugd.haohaochexian.top

Go:   if s == "" {}
来源：http://yoe.bjfxy.top

Ruby: if s.empty?
来源：http://pux.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cah.ydzc1.top

[E21] 超长截断加省略号
来源：http://uer.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vlj.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tjd.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hox.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ssz.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iwe.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://xjc.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ipf.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uuj.zycfv.cn

[E22] 字节长度与字符长度
来源：http://bxy.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ibk.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://flh.svipenyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dej.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vep.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ruo.sysykeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zbt.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://uov.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hnc.shuidangran.top

================================================================================
来源：http://wuk.ydjk.org.cn

F. 文件与目录
来源：http://swd.redwolf501.top

================================================================================
来源：http://gcz.gaohongyu789.top

[F01] 读取整个文件
来源：http://drm.cdnleiting.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://duq.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://bhn.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://phz.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jbu.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hom.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dev.fehbvm.com

Ruby: File.read("a.txt")
来源：http://bzt.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://fzo.yongpay.top

[F02] 逐行读取文件
来源：http://zee.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jhz.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://muz.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bze.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iwq.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cgw.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://abd.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://amn.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gaw.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://oeg.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mwm.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dmg.zhijiandao.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://acp.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lgo.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xhr.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nsl.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qbp.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ser.chenzaomai.com

[F04] 追加写入文件
来源：http://qje.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://agm.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wpw.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jzk.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ikp.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ihf.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ilr.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tyv.sxryk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wln.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://baz.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://weq.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://epm.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://rcg.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://bmj.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zns.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ccd.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://ohf.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://grh.yj20258888.top

[F06] 删除文件
来源：http://ijy.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://yef.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://jpz.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://psc.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qgd.yangfankeji.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ndy.tanke756.top

Go:   os.Remove("a.txt")
来源：http://fmp.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://vav.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://kbh.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://erd.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xbl.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bkk.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fhu.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pfz.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lkw.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://smi.ctjpmb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wkf.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://imc.sysykeji.top

[F08] 遍历目录
来源：http://onc.jinqigufen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ebu.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jbz.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://zfh.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://dsk.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uxn.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zzj.meibo888.top

Ruby: Dir.children("dir")
来源：http://fxr.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://epi.dianchejie.cn

[F09] 获取文件大小
来源：http://qxv.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://bhv.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://etc.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://ncw.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://qzg.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://gqv.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zdf.wangshuangyany.cn

Ruby: File.size("a.txt")
来源：http://hqv.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://tct.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://yhz.316326.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://usu.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ssv.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yro.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://xpo.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://znp.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jkp.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qjj.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ngo.jinqigfzy.top

[F11] 复制与移动文件
来源：http://ilm.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fjy.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://emi.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://skd.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iaj.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dsp.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kpq.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dns.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://afw.xuetiantiany.cn

[F12] CSV 读写
来源：http://dxj.zhoulong.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eum.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cas.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nlm.shzxlz.cn

TS:   // 同上
来源：http://hyz.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vuv.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wnd.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zga.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ozf.yvedp.cn

================================================================================
来源：http://upo.tarul.cn

G. 面向对象
来源：http://kjk.chenlongwang.top

================================================================================
来源：http://kqm.kuanghao11.cn

[G01] 定义类
来源：http://huh.havefunace.top

Py:   class User: pass
来源：http://mbh.9152youxi.cn

PHP:  class User {}
来源：http://nrx.gaohongyu789.top

JS:   class User {}
来源：http://dtj.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://niq.ybcxt.top

Java: class User {}
来源：http://mlx.jqgfzy.top

Go:   type User struct { Name string }
来源：http://gez.smart0.xyz

Ruby: class User; end
来源：http://vpl.dianchejie.cn

C#:   class User {}
来源：http://vop.yuxming.cn

[G02] 构造函数
来源：http://jto.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://zya.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://wzp.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://miz.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://qtk.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://nnc.gotoacloud.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wwg.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://gka.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://fnn.hesvh.cn

[G03] 实例属性
来源：http://tiw.epnwcf.com

Py:   self.name = "x"
来源：http://yef.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://zff.zhiwuduotai.top

JS:   this.name = "x";
来源：http://lpw.yfazqb.com

TS:   name: string = "x";
来源：http://ged.yongpay.top

Java: private String name;
来源：http://rcu.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jyh.chenjidiqi.icu

Ruby: @name = "x"
来源：http://ivd.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://cuh.dashuyun.cn

[G04] 定义方法
来源：http://aix.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://sbq.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://fsz.ydzc1.top

JS:   greet() { return this.name; }
来源：http://blk.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://gps.hnqzz.top

Java: String greet() { return name; }
来源：http://kyp.zhoulong.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://xnm.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://iff.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://tly.guowangkeji.top

[G05] 继承
来源：http://clp.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://cmg.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://mss.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://wjm.hfpthk.cn

TS:   class Admin extends User {}
来源：http://wbr.sufxvd.cn

Java: class Admin extends User {}
来源：http://trf.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kyy.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://lip.xinyue.icu

C#:   class Admin : User {}
来源：http://afw.chenlongwang.top

[G06] 重写方法
来源：http://izc.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://spw.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://iwu.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://zqt.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://yiw.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://rjk.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://esi.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://nms.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://uor.yonumen.top

[G07] 调用父类方法
来源：http://hgx.zhengqikj.top

Py:   super().greet()
来源：http://kzg.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://mqi.52xcode.cn

JS:   super.greet();
来源：http://bef.jianghu66.top

TS:   super.greet();
来源：http://uiv.yanxiufei.cn

Java: super.greet();
来源：http://bks.birdmap.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://elz.ywan-chungtsiang.top

Ruby: super
来源：http://rtn.tian-w.cn

C#:   base.Greet();
来源：http://wea.yfazqb.com

[G08] 静态方法与属性
来源：http://kgs.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uye.xingfuxueyuan.xyz

PHP:  public static function f() {}
来源：http://krf.ywan-chungtsiang.top

JS:   static f() {}
来源：http://tpy.gzhubu.top

TS:   static f(): void {}
来源：http://iez.sysykeji.top

Java: static void f() {}
来源：http://wgb.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://yqx.epnwcf.com

Ruby: def self.f; end
来源：http://wfp.fengsongda.top

C#:   public static void F() {}
来源：http://qye.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://edi.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://bul.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://ued.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://kkb.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://mqq.hammf.cn

Java: interface Shape { double area(); }
来源：http://uth.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://wfn.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wka.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://jdt.sxryk.cn

[G10] 访问控制
来源：http://hqm.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://duc.bbcook.cn

PHP:  public / protected / private
来源：http://mbv.cashguo.top

JS:   #private 字段；其余公开
来源：http://ugw.jqgfzy.top

TS:   public / protected / private
来源：http://yzr.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://ffr.sufxvd.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wht.sxryk.cn

Ruby: public / protected / private
来源：http://mly.aizwys.cn

C#:   public / protected / private / internal
来源：http://glh.ydjk.org.cn

[G11] getter / setter
来源：http://yro.jqgufenzy.top

Py:   @property 与 @x.setter
来源：http://vzo.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qlw.tian-w.cn

JS:   get name() { return this._name; }
来源：http://wpq.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://zxq.vehdjk.com

Java: public String getName() { return name; }
来源：http://vvq.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wja.aibaodan.cn

Ruby: attr_accessor :name
来源：http://dsi.havefunace.top

C#:   public string Name { get; set; }
来源：http://kwx.jyoumei.cn

[G12] 对象转字符串
来源：http://dxi.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://aul.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ptp.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://spy.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://hwb.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://rev.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://nrd.zycfv.cn

Ruby: def to_s; @name; end
来源：http://nyk.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://bkb.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://gfv.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://hyr.quarkkingdee.top

PHP:  $u instanceof User
来源：http://hnx.hnqzz.top

JS:   u instanceof User
来源：http://zji.pengpengdd.cyou

TS:   u instanceof User
来源：http://sal.hfpthk.cn


<!-- 参考信息 -->