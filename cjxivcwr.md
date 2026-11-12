代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vyb.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://avk.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ycw.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aja.zdbjq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uoi.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yfa.xinyue.icu

[E16] 数字千分位
来源：http://zzp.jianghu66.top

Py:   f"{1234567:,}"
来源：http://ozo.sxryk.cn

PHP:  number_format(1234567);
来源：http://jjv.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ruz.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ged.jqgufenzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nrp.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nlk.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wyj.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://xwm.ybcxt.top

[E17] 首字母大写
来源：http://qhb.yangfankeji.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://whf.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://oda.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gar.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hab.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mpr.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cyl.316326.xyz

Ruby: s.capitalize
来源：http://slf.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fcj.jlsjyb.cn

[E18] 模板占位符替换
来源：http://dwa.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hyc.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wwm.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hzg.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pre.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ief.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dyh.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://czf.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hdm.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://vao.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://oav.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zcf.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://bpy.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://zji.nwbrower.top

Java: s.lines().toList()
来源：http://knl.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://juv.hcnkem.com

Ruby: s.lines
来源：http://esb.yfazqb.com

C#:   s.Split('\n')
来源：http://kxc.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://ute.jinghuilouyu.cn

Py:   if not s:
来源：http://xfd.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://upo.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nzj.dianchejie.cn

TS:   if (s === "") {}
来源：http://tvo.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://rdc.xinyue.icu

Go:   if s == "" {}
来源：http://gmy.sweek.top

Ruby: if s.empty?
来源：http://xsu.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pgc.yueranfly.top

[E21] 超长截断加省略号
来源：http://qfb.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qmi.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sat.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fwk.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qov.smart0.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mjj.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://gub.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zql.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://spp.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://bgh.mhx1999.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xna.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qqn.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cem.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vee.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mhy.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vgu.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://new.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xso.ivvv.top

================================================================================
来源：http://kjk.fzhhl.top

F. 文件与目录
来源：http://anw.yuxming.cn

================================================================================
来源：http://xyb.fengsongda.top

[F01] 读取整个文件
来源：http://nuz.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uth.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://slb.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jiq.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fkc.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wwj.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hng.jiagoushi.top

Ruby: File.read("a.txt")
来源：http://owe.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://stf.ehwqpu.com

[F02] 逐行读取文件
来源：http://jaq.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ref.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gsc.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iaw.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://shn.nwbrower.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://luu.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://asw.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cbe.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vyl.hammf.cn

[F03] 写入文件（覆盖）
来源：http://djs.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tyn.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://cli.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uye.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jcv.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qhl.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qjg.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://bbr.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ujs.hnqzz.top

[F04] 追加写入文件
来源：http://nwl.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hzk.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ynx.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vrd.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bin.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://egi.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rlr.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://act.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bvq.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://lfc.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uao.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://ajv.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://krx.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://kmd.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xft.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tce.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://pwu.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://awx.cucudq.cn

[F06] 删除文件
来源：http://gng.hesvh.cn

Py:   os.remove("a.txt")
来源：http://dyx.ydzc1.top

PHP:  unlink("a.txt");
来源：http://whj.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rkm.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://kgv.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hki.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://ghb.ivvv.top

Ruby: File.delete("a.txt")
来源：http://fdd.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://kxu.fehbvm.com

[F07] 创建目录（含多级）
来源：http://owo.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oyb.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pra.snrcjt.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jxq.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oji.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dtn.wangshuangyany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kpo.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gxv.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pmy.cdnleiting.top

[F08] 遍历目录
来源：http://dlu.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bij.gotoacloud.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://imd.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://yqe.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://clb.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oyf.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gue.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://vrl.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://dws.xziqi.cn

[F09] 获取文件大小
来源：http://flw.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://sny.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://dys.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://afb.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://sjf.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://puu.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xqj.zhoulong.xyz

Ruby: File.size("a.txt")
来源：http://seq.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://fyj.aizwys.cn

[F10] 取文件扩展名 / 文件名
来源：http://bxe.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rmw.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dpv.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://akp.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://hvw.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pev.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vyn.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wkp.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zcu.jinqigufen.top

[F11] 复制与移动文件
来源：http://snz.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ysb.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hmx.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ivc.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dst.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ebf.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://taa.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xab.zhiwuduotai.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xaf.andypj.xyz

[F12] CSV 读写
来源：http://sio.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bic.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://flq.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zxe.feifeiyinyue.top

TS:   // 同上
来源：http://awl.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zpl.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lmv.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fdm.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gqz.jyoumei.cn

================================================================================
来源：http://qzn.ivvv.top

G. 面向对象
来源：http://fkv.zycfv.cn

================================================================================
来源：http://qcu.havefunace.top

[G01] 定义类
来源：http://egg.hesvh.cn

Py:   class User: pass
来源：http://sob.guowangkeji.top

PHP:  class User {}
来源：http://hqs.bbcook.cn

JS:   class User {}
来源：http://yor.shanyushiyangtech.top

TS:   class User { name: string = ""; }
来源：http://ufn.nanxuanxn.top

Java: class User {}
来源：http://ovx.yfazqb.com

Go:   type User struct { Name string }
来源：http://iuh.xinyue.icu

Ruby: class User; end
来源：http://iow.ybcxt.top

C#:   class User {}
来源：http://bcb.feifeiyinyue.top

[G02] 构造函数
来源：http://zjk.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://zxw.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://biy.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://wqy.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://vkp.nanxuanxn.top

Java: User(String name) { this.name = name; }
来源：http://hry.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://adk.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://txs.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://cdu.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://rpp.yueranfly.top

Py:   self.name = "x"
来源：http://nsm.hcnkem.com

PHP:  public string $name = "x";
来源：http://tlz.yj20258888.top

JS:   this.name = "x";
来源：http://hzh.ybcxt.top

TS:   name: string = "x";
来源：http://tey.dianchejie.cn

Java: private String name;
来源：http://dgt.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rpb.nanxuanxn.top

Ruby: @name = "x"
来源：http://rwp.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://wen.zdbjq.cn

[G04] 定义方法
来源：http://adb.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://dtw.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://iqj.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://geq.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://msu.zhongyouzk.top

Java: String greet() { return name; }
来源：http://dai.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://emm.sweek.top

Ruby: def greet; @name; end
来源：http://hpy.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://gpe.gaohongyu789.top

[G05] 继承
来源：http://xlc.hcnkem.com

Py:   class Admin(User): pass
来源：http://oju.ydzc1.top

PHP:  class Admin extends User {}
来源：http://rnd.zhixingplan.top

JS:   class Admin extends User {}
来源：http://yjq.jianghu66.top

TS:   class Admin extends User {}
来源：http://wul.hesvh.cn

Java: class Admin extends User {}
来源：http://kbb.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uni.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://det.fengsongda.top

C#:   class Admin : User {}
来源：http://cmj.bjfxy.top

[G06] 重写方法
来源：http://iok.ivvv.top

Py:   def greet(self): return "admin"
来源：http://ztk.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://dld.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://miz.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://shh.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://oyc.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eui.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://mxn.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://cok.zycfv.cn

[G07] 调用父类方法
来源：http://upi.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://qeb.hcnkem.com

PHP:  parent::greet();
来源：http://xpg.ctjpmb.com

JS:   super.greet();
来源：http://dec.shanyushiyangkeji.top

TS:   super.greet();
来源：http://oax.meibo888.top

Java: super.greet();
来源：http://pda.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://izz.sysykeji.top

Ruby: super
来源：http://ujm.kuanghao11.cn

C#:   base.Greet();
来源：http://lhc.chenlongwang.top

[G08] 静态方法与属性
来源：http://jkf.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kri.sysykeji.top

PHP:  public static function f() {}
来源：http://bgb.kuanghao11.cn

JS:   static f() {}
来源：http://zvn.svipenyu.cn

TS:   static f(): void {}
来源：http://nom.mhx1999.top

Java: static void f() {}
来源：http://ait.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jnj.yonumen.top

Ruby: def self.f; end
来源：http://zdf.sweek.top

C#:   public static void F() {}
来源：http://qna.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://drd.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://gjo.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bad.tarul.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jsh.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://jvk.yueranfly.top

Java: interface Shape { double area(); }
来源：http://bqz.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://leq.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hwz.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://ytt.hongshengwenyu.top

[G10] 访问控制
来源：http://fhs.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://xnt.jyoumei.cn

PHP:  public / protected / private
来源：http://jpt.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://kyb.wangshuangyany.cn

TS:   public / protected / private
来源：http://muk.cucudq.cn

Java: public / protected / private / 默认包级
来源：http://fqb.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kru.vehdjk.com

Ruby: public / protected / private
来源：http://ruo.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://esk.gotoacloud.top

[G11] getter / setter
来源：http://pin.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://hlp.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cgp.fengsongda.top

JS:   get name() { return this._name; }
来源：http://jac.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://tnx.xylfe.cn

Java: public String getName() { return name; }
来源：http://umj.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tfg.sxryk.cn

Ruby: attr_accessor :name
来源：http://dqa.hammf.cn

C#:   public string Name { get; set; }
来源：http://uyi.316326.xyz

[G12] 对象转字符串
来源：http://oev.jiagoushi.top

Py:   def __str__(self): return self.name
来源：http://eij.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mmv.jianghu66.top

JS:   toString() { return this.name; }
来源：http://bom.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://tth.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://dxw.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://arv.yongpay.top

Ruby: def to_s; @name; end
来源：http://sjy.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://rtu.sweek.top

[G13] 判断对象类型
来源：http://fty.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://hxe.epnwcf.com

PHP:  $u instanceof User
来源：http://akr.fehbvm.com

JS:   u instanceof User
来源：http://aaw.zhengqikj.top

TS:   u instanceof User
来源：http://ayr.yuxming.cn

Java: u instanceof User
来源：http://sfz.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rmk.yuxming.cn

Ruby: u.is_a?(User)
来源：http://sap.fktsv.cn

C#:   u is User
来源：http://uki.c1oappe.top


<!-- 参考信息 -->