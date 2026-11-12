代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lpa.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yfc.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mhv.yonumen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xus.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jcq.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://set.zycfv.cn

[E16] 数字千分位
来源：http://jpw.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://vkb.sufxvd.cn

PHP:  number_format(1234567);
来源：http://xzi.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qod.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mke.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tal.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oak.cqqwz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tgx.ivvv.top

C#:   1234567.ToString("N0")
来源：http://hti.ivvv.top

[E17] 首字母大写
来源：http://hpp.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://crb.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ubf.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://now.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uzr.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://exu.gogol.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uri.pengpengdd.cyou

Ruby: s.capitalize
来源：http://lpw.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kdf.mhx1999.top

[E18] 模板占位符替换
来源：http://qmj.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ein.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nmn.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://gwe.yuanzhike.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hqe.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zty.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ezq.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wwd.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cfi.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://sha.bjfxy.top

Py:   s.splitlines()
来源：http://zxt.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bpg.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://fdd.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://gou.jianghu66.top

Java: s.lines().toList()
来源：http://ndp.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://ddz.zhiwuduotai.top

Ruby: s.lines
来源：http://lni.ctjpmb.com

C#:   s.Split('\n')
来源：http://nxx.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://shw.gaohongyu789.top

Py:   if not s:
来源：http://qmz.zdbjq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xqb.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lhv.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://zug.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://gck.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://qbj.jianghu66.top

Ruby: if s.empty?
来源：http://kxi.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uhj.tanke756.top

[E21] 超长截断加省略号
来源：http://yns.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://owf.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ium.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ohl.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rxo.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ddl.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://vcl.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rrh.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tpz.daxiang520.top

[E22] 字节长度与字符长度
来源：http://rcn.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zfo.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xvz.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://slw.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mkx.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rye.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vdw.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://kmm.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zao.chenlongwang.top

================================================================================
来源：http://yao.epnwcf.com

F. 文件与目录
来源：http://qlt.jlsjyb.cn

================================================================================
来源：http://cyh.xuetiantiany.cn

[F01] 读取整个文件
来源：http://xwt.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ifh.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://qlp.zhaomingkeji.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qlb.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://swx.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oru.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://siv.ivvv.top

Ruby: File.read("a.txt")
来源：http://dwt.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://jbe.guannengcc.top

[F02] 逐行读取文件
来源：http://ayh.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uwg.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uqi.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lqg.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zhf.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://haa.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vub.zycfv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bdu.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iuk.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://xhq.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oen.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rfw.shanyushiyangtech.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://asd.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wfd.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gxi.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tgn.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://env.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vft.dashuyun.cn

[F04] 追加写入文件
来源：http://qbw.yongpay.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ueb.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hdw.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://owq.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xyd.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wps.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xns.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://age.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yqv.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://jkp.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cov.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://gvf.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://dav.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://fic.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dqf.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wnx.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://vvy.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://llt.jinqigfzy.top

[F06] 删除文件
来源：http://qsu.cashguo.top

Py:   os.remove("a.txt")
来源：http://swu.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://mnk.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://sdw.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xqn.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lah.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://iib.pycfn.com

Ruby: File.delete("a.txt")
来源：http://sqm.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://adj.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://wqz.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iyb.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xxh.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ioc.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://szq.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gzi.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ccc.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dio.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kub.316326.xyz

[F08] 遍历目录
来源：http://osf.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://cyv.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jxv.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://tdv.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://fsa.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ned.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://xac.meibo888.top

Ruby: Dir.children("dir")
来源：http://rqq.chenjidiqi.icu

C#:   Directory.GetFiles("dir")
来源：http://sss.hywenlv.cn

[F09] 获取文件大小
来源：http://scr.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://pji.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://bnv.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://bud.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://ooj.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jqf.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dxz.yuxming.cn

Ruby: File.size("a.txt")
来源：http://lec.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://avf.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://htz.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rgy.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cen.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eth.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://aji.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://byb.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tci.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ogn.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lbd.dashuyun.cn

[F11] 复制与移动文件
来源：http://kxd.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uka.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tef.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xel.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://big.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kiw.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nyf.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://svg.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pbo.tianlin.xyz

[F12] CSV 读写
来源：http://ulu.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://acn.ydjk.org.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zmo.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ecv.havefunace.top

TS:   // 同上
来源：http://unw.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eiv.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ciz.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://stf.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oif.xuanzx.com

================================================================================
来源：http://nih.zhongyouzk.top

G. 面向对象
来源：http://rfl.ydjk.org.cn

================================================================================
来源：http://fet.ehwqpu.com

[G01] 定义类
来源：http://ffn.hcnkem.com

Py:   class User: pass
来源：http://rzr.sxryk.cn

PHP:  class User {}
来源：http://vht.vqdsnc.cn

JS:   class User {}
来源：http://weu.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://oym.yj202588.top

Java: class User {}
来源：http://vkr.epnwcf.com

Go:   type User struct { Name string }
来源：http://ifu.ydjk.org.cn

Ruby: class User; end
来源：http://lwt.bbcook.cn

C#:   class User {}
来源：http://lfr.iojbl.cn

[G02] 构造函数
来源：http://pdg.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://cbg.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ijh.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://jcj.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://hho.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://wvk.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zqj.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://abl.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://ype.vehdjk.com

[G03] 实例属性
来源：http://cfv.shanyushiyangtech.top

Py:   self.name = "x"
来源：http://psw.havefunace.top

PHP:  public string $name = "x";
来源：http://jvp.gotoacloud.top

JS:   this.name = "x";
来源：http://hjz.ydjk.org.cn

TS:   name: string = "x";
来源：http://zjg.zdqjudy.top

Java: private String name;
来源：http://zwj.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jvt.ctjpmb.com

Ruby: @name = "x"
来源：http://fxg.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://kpq.yonumen.top

[G04] 定义方法
来源：http://khe.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://xvq.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xno.pycfn.com

JS:   greet() { return this.name; }
来源：http://sxl.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://cgo.quarkkingdee.top

Java: String greet() { return name; }
来源：http://ehm.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bxr.daxiang520.top

Ruby: def greet; @name; end
来源：http://qsi.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://gik.yonumen.top

[G05] 继承
来源：http://lcw.bjfxy.top

Py:   class Admin(User): pass
来源：http://nrk.bjfxy.top

PHP:  class Admin extends User {}
来源：http://lih.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://tpu.jianghu66.top

TS:   class Admin extends User {}
来源：http://njq.gotoacloud.top

Java: class Admin extends User {}
来源：http://afv.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rra.316326.xyz

Ruby: class Admin < User; end
来源：http://kgx.yanxiufei.cn

C#:   class Admin : User {}
来源：http://ovt.cqqwz.cn

[G06] 重写方法
来源：http://vfr.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://ryb.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yir.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://dtn.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://lue.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://nzt.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tls.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://xmq.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://rvj.shuidangran.top

[G07] 调用父类方法
来源：http://seg.quarkkingdee.top

Py:   super().greet()
来源：http://zgy.hammf.cn

PHP:  parent::greet();
来源：http://xck.gzhubu.top

JS:   super.greet();
来源：http://vgl.zhoulong.xyz

TS:   super.greet();
来源：http://gqs.jinqigfzy.top

Java: super.greet();
来源：http://xxl.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qgk.aibaodan.cn

Ruby: super
来源：http://apb.sysykeji.top

C#:   base.Greet();
来源：http://nzs.yonumen.top

[G08] 静态方法与属性
来源：http://qof.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vyr.wangdashe.top

PHP:  public static function f() {}
来源：http://hwt.yfazqb.com

JS:   static f() {}
来源：http://rng.hysaishi.cn

TS:   static f(): void {}
来源：http://bxk.zhongyouzk.top

Java: static void f() {}
来源：http://axo.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ssq.xziqi.cn

Ruby: def self.f; end
来源：http://pmr.hammf.cn

C#:   public static void F() {}
来源：http://ldw.havefunace.top

[G09] 接口 / 抽象类
来源：http://vpi.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://hwn.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qdq.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vyh.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://quy.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://kkv.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://qky.hammf.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tco.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://qpn.ctjpmb.com

[G10] 访问控制
来源：http://ise.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://atj.hammf.cn

PHP:  public / protected / private
来源：http://tht.yueranfly.top

JS:   #private 字段；其余公开
来源：http://nsm.xinyue.icu

TS:   public / protected / private
来源：http://gea.havefunace.top

Java: public / protected / private / 默认包级
来源：http://czz.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sqa.316326.xyz

Ruby: public / protected / private
来源：http://bkf.yonumen.top

C#:   public / protected / private / internal
来源：http://ywm.snrcjt.cn

[G11] getter / setter
来源：http://ske.yuxming.cn

Py:   @property 与 @x.setter
来源：http://mxq.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ajf.daxiang520.top

JS:   get name() { return this._name; }
来源：http://oxs.jyoumei.cn

TS:   get name(): string { return this._name; }
来源：http://zli.tanke756.top

Java: public String getName() { return name; }
来源：http://jtc.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ojf.c1oappe.top

Ruby: attr_accessor :name
来源：http://zem.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://pri.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://yqn.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://thz.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bcj.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://ejf.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://fxf.sweek.top

Java: @Override public String toString() { return name; }
来源：http://hox.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://ovf.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://jdc.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://smu.yonumen.top

[G13] 判断对象类型
来源：http://kca.fktsv.cn

Py:   isinstance(u, User)
来源：http://dor.yanxiufei.cn

PHP:  $u instanceof User
来源：http://ucd.daria6918.cn

JS:   u instanceof User
来源：http://yzr.bjfxy.top

TS:   u instanceof User
来源：http://nmw.sjlbkw.cn

Java: u instanceof User
来源：http://mmz.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ahu.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://dpm.yfazqb.com

C#:   u is User
来源：http://ace.tian-w.cn


<!-- 参考信息 -->