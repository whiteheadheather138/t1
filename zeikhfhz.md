代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yfp.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://cjk.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://upm.guannengcc.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mmz.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lzz.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qcv.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yss.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rmm.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qyh.ywan-chungtsiang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gqc.hnxiangtu.top

[E16] 数字千分位
来源：http://tyu.sysykeji.top

Py:   f"{1234567:,}"
来源：http://cxh.andypj.xyz

PHP:  number_format(1234567);
来源：http://qvw.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qyi.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ija.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pwt.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kbb.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ejn.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://zej.jqgufenzy.top

[E17] 首字母大写
来源：http://nic.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sfu.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://dwt.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tld.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sry.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hal.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ttp.yonumen.top

Ruby: s.capitalize
来源：http://qsg.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uxl.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://how.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aii.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://azi.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wmm.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://irn.iojbl.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ack.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ntw.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://url.ydzc1.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vgo.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://bju.hnxiangtu.top

Py:   s.splitlines()
来源：http://lse.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gnj.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://lru.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://mnc.hongshengwenyu.top

Java: s.lines().toList()
来源：http://sct.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://une.tian-w.cn

Ruby: s.lines
来源：http://lhj.vqdsnc.cn

C#:   s.Split('\n')
来源：http://jws.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://ajn.birdmap.top

Py:   if not s:
来源：http://iam.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wdl.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vtu.hcnkem.com

TS:   if (s === "") {}
来源：http://zzh.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://jqu.shangyingyoupin.top

Go:   if s == "" {}
来源：http://nyg.jianghu66.top

Ruby: if s.empty?
来源：http://igy.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wmb.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://iyg.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xlk.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xus.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://atk.zdbjq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gch.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jga.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://ior.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fwn.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pzm.bbcook.cn

[E22] 字节长度与字符长度
来源：http://rol.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hwo.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rsg.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lmx.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pfy.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oxm.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xiv.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://oyj.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hrx.yongpay.top

================================================================================
来源：http://swz.wangdashe.top

F. 文件与目录
来源：http://cjs.zhixingplan.top

================================================================================
来源：http://qwj.0kj1m.cn

[F01] 读取整个文件
来源：http://zpk.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pid.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://ali.ybcxt.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vjh.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ydy.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ehv.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://akq.ivvv.top

Ruby: File.read("a.txt")
来源：http://tpe.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://zbq.zhongyouzk.top

[F02] 逐行读取文件
来源：http://gdl.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://waq.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lyl.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wib.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xtg.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://huc.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://psb.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://abh.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lst.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://khe.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://idb.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nzi.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qxa.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ztp.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wcb.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zmp.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://uog.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xjt.epnwcf.com

[F04] 追加写入文件
来源：http://ynl.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dxs.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mmy.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jhe.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ujg.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xqe.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yvj.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jmq.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xgz.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://znm.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vtj.dashuyun.cn

PHP:  file_exists("a.txt");
来源：http://mmx.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://gsw.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://yfx.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fve.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rgl.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://roq.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://dej.shzxlz.cn

[F06] 删除文件
来源：http://evd.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://qnz.hesvh.cn

PHP:  unlink("a.txt");
来源：http://szl.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://dwo.jinyuanbaomall.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qji.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oet.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://kbr.meibo888.top

Ruby: File.delete("a.txt")
来源：http://rjt.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://psb.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://jso.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ogo.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nmk.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cop.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dgo.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ufh.andypj.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hue.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xro.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sog.hesvh.cn

[F08] 遍历目录
来源：http://gca.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oli.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://soq.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://oyj.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://tia.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qpx.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rxl.hesvh.cn

Ruby: Dir.children("dir")
来源：http://oqr.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://agp.svipenyu.cn

[F09] 获取文件大小
来源：http://ucx.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://vkp.316326.xyz

PHP:  filesize("a.txt");
来源：http://ory.zhaomingkeji.xyz

JS:   fs.statSync("a.txt").size
来源：http://ewj.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://bhh.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://krm.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rlq.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://jkx.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://ben.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://uub.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zfu.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eow.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hml.gzhubu.top

TS:   path.extname("a.txt")
来源：http://pbd.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yvs.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nkn.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zut.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://khf.hnxiangtu.top

[F11] 复制与移动文件
来源：http://fwq.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ecr.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hhc.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rhi.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mmv.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pgp.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cri.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jce.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qmy.svipenyu.cn

[F12] CSV 读写
来源：http://grv.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fth.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nzg.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vmk.guowangkeji.top

TS:   // 同上
来源：http://lmr.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xsg.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nfu.cashguo.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tvm.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zpb.jinqigufen.top

================================================================================
来源：http://ruz.fanxiaobao.xyz

G. 面向对象
来源：http://jfj.mhx1999.top

================================================================================
来源：http://uxu.cdnleiting.top

[G01] 定义类
来源：http://ebn.cashguo.top

Py:   class User: pass
来源：http://fcu.hnxiangtu.top

PHP:  class User {}
来源：http://hdm.hywenlv.cn

JS:   class User {}
来源：http://uvw.meibo888.top

TS:   class User { name: string = ""; }
来源：http://jqq.hnxiangtu.top

Java: class User {}
来源：http://sbm.ehwqpu.com

Go:   type User struct { Name string }
来源：http://afk.ehwqpu.com

Ruby: class User; end
来源：http://elz.bjfxy.top

C#:   class User {}
来源：http://tde.birdmap.top

[G02] 构造函数
来源：http://irl.hnqzz.top

Py:   def __init__(self, name): self.name = name
来源：http://njf.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://hrj.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://mhu.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://aih.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://xgv.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://umi.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://vrr.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://ppi.yueranfly.top

[G03] 实例属性
来源：http://rnu.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://skx.hesvh.cn

PHP:  public string $name = "x";
来源：http://xgp.tarul.cn

JS:   this.name = "x";
来源：http://cvv.ctjpmb.com

TS:   name: string = "x";
来源：http://nsp.shanyushiyangtech.top

Java: private String name;
来源：http://wdp.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qny.nwbrower.top

Ruby: @name = "x"
来源：http://pcc.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://scu.gaohongyu789.top

[G04] 定义方法
来源：http://twg.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://rhl.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ghv.yfazqb.com

JS:   greet() { return this.name; }
来源：http://fbh.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://xyi.jlsjyb.cn

Java: String greet() { return name; }
来源：http://cbq.gzhubu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://usm.vehdjk.com

Ruby: def greet; @name; end
来源：http://teh.tarul.cn

C#:   public string Greet() => Name;
来源：http://bki.nanxinkj.top

[G05] 继承
来源：http://vdq.gotoacloud.top

Py:   class Admin(User): pass
来源：http://eze.hcnkem.com

PHP:  class Admin extends User {}
来源：http://azh.jianghu66.top

JS:   class Admin extends User {}
来源：http://nxr.zhixingplan.top

TS:   class Admin extends User {}
来源：http://nxr.ivvv.top

Java: class Admin extends User {}
来源：http://ela.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rjg.ybcxt.top

Ruby: class Admin < User; end
来源：http://nax.bjfxy.top

C#:   class Admin : User {}
来源：http://wre.ivvv.top

[G06] 重写方法
来源：http://wgi.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://iqk.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bmu.redwolf501.top

JS:   greet() { return "admin"; }
来源：http://ecg.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://znw.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://lmr.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://thv.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://cgv.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://muq.nanxinkj.top

[G07] 调用父类方法
来源：http://ify.zdbjq.cn

Py:   super().greet()
来源：http://bzb.smart0.xyz

PHP:  parent::greet();
来源：http://oys.shzxlz.cn

JS:   super.greet();
来源：http://ntp.yuxming.cn

TS:   super.greet();
来源：http://lhv.hysaishi.cn

Java: super.greet();
来源：http://ukl.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jdh.sysykeji.top

Ruby: super
来源：http://nuq.iojbl.cn

C#:   base.Greet();
来源：http://zra.hywenlv.cn

[G08] 静态方法与属性
来源：http://mke.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ggz.zycfv.cn

PHP:  public static function f() {}
来源：http://vcp.fktsv.cn

JS:   static f() {}
来源：http://lbb.wangshuangyany.cn

TS:   static f(): void {}
来源：http://ybu.sweek.top

Java: static void f() {}
来源：http://pnx.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rew.zhixingplan.top

Ruby: def self.f; end
来源：http://lzm.uphjek.com

C#:   public static void F() {}
来源：http://bxc.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://bhf.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://vvb.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mkn.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hsb.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://vwi.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://rmu.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://qms.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aaq.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://qxo.gaohongyu789.top

[G10] 访问控制
来源：http://lpk.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://uzs.yueranfly.top

PHP:  public / protected / private
来源：http://csb.birdmap.top

JS:   #private 字段；其余公开
来源：http://pcv.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://ejz.uphjek.com

Java: public / protected / private / 默认包级
来源：http://lsw.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rel.hnqzz.top

Ruby: public / protected / private
来源：http://xsu.gotoacloud.top

C#:   public / protected / private / internal
来源：http://idn.yangfankeji.com

[G11] getter / setter
来源：http://xgr.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://oiy.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tbe.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://ayv.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://tpp.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://qni.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ush.sxryk.cn

Ruby: attr_accessor :name
来源：http://zcq.redwolf501.top

C#:   public string Name { get; set; }
来源：http://xsz.shangyingyoupin.top

[G12] 对象转字符串
来源：http://gpl.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://sbx.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rlm.birdmap.top

JS:   toString() { return this.name; }
来源：http://uce.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://igl.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://jme.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://csd.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://ris.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://uav.daria6918.cn

[G13] 判断对象类型
来源：http://dwu.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://eft.tanke756.top

PHP:  $u instanceof User
来源：http://mww.yonumen.top

JS:   u instanceof User
来源：http://urb.jlsjyb.cn

TS:   u instanceof User
来源：http://yjg.guannengcc.top


<!-- 参考信息 -->