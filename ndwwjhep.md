代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yel.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://beh.andypj.xyz

[E16] 数字千分位
来源：http://nyo.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://vxm.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://gnm.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://izd.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nax.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rnh.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uos.ppjwa.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ddt.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://dwy.tianlin.xyz

[E17] 首字母大写
来源：http://adb.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://los.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fbk.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yub.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sld.zhijiandao.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://igd.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ozz.yanxiufei.cn

Ruby: s.capitalize
来源：http://xrh.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iln.bjfxy.top

[E18] 模板占位符替换
来源：http://odv.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fol.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zts.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://vqh.gotoacloud.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lfz.yj20258.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vof.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fls.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cwh.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://udc.andypj.xyz

[E19] 多行文本按行拆分
来源：http://vxr.havefunace.top

Py:   s.splitlines()
来源：http://stx.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pjl.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://lit.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://jch.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://ybc.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://zmx.guannengcc.top

Ruby: s.lines
来源：http://jvg.52xcode.cn

C#:   s.Split('\n')
来源：http://cqu.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://oxy.jqgfzy.top

Py:   if not s:
来源：http://noc.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qrx.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rod.fktsv.cn

TS:   if (s === "") {}
来源：http://afy.316326.xyz

Java: if (s.isEmpty()) {}
来源：http://ctz.hnxiangtu.top

Go:   if s == "" {}
来源：http://srf.daxiang520.top

Ruby: if s.empty?
来源：http://ned.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pho.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://jpc.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lgh.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sto.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oko.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ngd.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://thh.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://ygt.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hmw.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qwg.yongpay.top

[E22] 字节长度与字符长度
来源：http://pfh.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ucd.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iaa.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fsf.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nda.xuetiantiany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vnd.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xgb.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://vim.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://opq.jlsjyb.cn

================================================================================
来源：http://lhd.xuetiantiany.cn

F. 文件与目录
来源：http://uie.zhaomingkeji.xyz

================================================================================
来源：http://bnd.sufxvd.cn

[F01] 读取整个文件
来源：http://xdw.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uza.yj20258.top

PHP:  file_get_contents("a.txt");
来源：http://fsw.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://axp.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ook.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nzu.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qat.yueranfly.top

Ruby: File.read("a.txt")
来源：http://qpk.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ufm.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://bdy.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gep.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sym.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vms.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zhm.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dlu.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ewr.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kjj.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dsh.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://lkx.bbcook.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oqc.ppjwa.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zcv.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yun.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xun.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://crn.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mrj.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://lhp.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uye.yuanzhike.top

[F04] 追加写入文件
来源：http://mva.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tbp.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uum.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://igl.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iuq.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yvl.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qqb.sysykeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bho.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://asq.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://npm.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mit.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://iqx.hysaishi.cn

JS:   fs.existsSync("a.txt")
来源：http://vwo.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://ndf.yvedp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://psk.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nwr.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://vrx.sweek.top

C#:   File.Exists("a.txt")
来源：http://wlg.yueranfly.top

[F06] 删除文件
来源：http://xpw.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://wcl.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://dbu.zhixingplan.top

JS:   fs.unlinkSync("a.txt")
来源：http://fwk.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lac.zhixingplan.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hgd.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://cym.hammf.cn

Ruby: File.delete("a.txt")
来源：http://nrc.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://xnq.c1oappe.top

[F07] 创建目录（含多级）
来源：http://imf.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfz.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://awz.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yuq.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wyx.aibaodan.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://brf.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://csy.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fqo.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bxy.aibaodan.cn

[F08] 遍历目录
来源：http://okw.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ekl.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ies.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://eem.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://stx.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xbh.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fzd.sufxvd.cn

Ruby: Dir.children("dir")
来源：http://iyz.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://abq.yanxiufei.cn

[F09] 获取文件大小
来源：http://dno.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://bwt.jiagoushi.top

PHP:  filesize("a.txt");
来源：http://zvi.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://siw.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://agp.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://vhb.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vac.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://spy.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://nyi.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://kud.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lrl.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vkw.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oft.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://ens.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uwh.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tit.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://koh.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ddz.cashguo.top

[F11] 复制与移动文件
来源：http://ksz.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://urb.yangfankeji.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jcq.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://awe.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yle.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tym.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wod.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bsx.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tcd.yonumen.top

[F12] CSV 读写
来源：http://ipx.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nyl.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gcd.jinqigufen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oph.sxryk.cn

TS:   // 同上
来源：http://jfd.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ifg.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xxq.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rid.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kir.tianlin.xyz

================================================================================
来源：http://hlq.jinqigufen.top

G. 面向对象
来源：http://gcu.andypj.xyz

================================================================================
来源：http://lnn.yueranfly.top

[G01] 定义类
来源：http://rte.redwolf501.top

Py:   class User: pass
来源：http://qdn.vehdjk.com

PHP:  class User {}
来源：http://yqh.jinyuanbaomall.cn

JS:   class User {}
来源：http://qqd.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://ahe.guannengcc.top

Java: class User {}
来源：http://ujd.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://chx.meibo888.top

Ruby: class User; end
来源：http://apd.tanke756.top

C#:   class User {}
来源：http://tuk.hywenlv.cn

[G02] 构造函数
来源：http://gvh.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://azb.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://fib.zhengqikj.top

JS:   constructor(name) { this.name = name; }
来源：http://imp.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://ght.xylfe.cn

Java: User(String name) { this.name = name; }
来源：http://uag.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wke.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://uew.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://woj.ydjk.org.cn

[G03] 实例属性
来源：http://cqo.sjlbkw.cn

Py:   self.name = "x"
来源：http://teb.zdqjudy.top

PHP:  public string $name = "x";
来源：http://sig.cashguo.top

JS:   this.name = "x";
来源：http://fcc.chenlongwang.top

TS:   name: string = "x";
来源：http://yky.xinyue.icu

Java: private String name;
来源：http://ild.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lru.fktsv.cn

Ruby: @name = "x"
来源：http://law.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://szl.yuanzhike.top

[G04] 定义方法
来源：http://sgy.yj20258.top

Py:   def greet(self): return self.name
来源：http://hxj.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://rdu.tian-w.cn

JS:   greet() { return this.name; }
来源：http://ogv.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://zeq.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://oag.xuetiantiany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://smb.pycfn.com

Ruby: def greet; @name; end
来源：http://ozw.fktsv.cn

C#:   public string Greet() => Name;
来源：http://xbw.zhijiandao.cn

[G05] 继承
来源：http://mgv.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://lmc.yfazqb.com

PHP:  class Admin extends User {}
来源：http://akz.birdmap.top

JS:   class Admin extends User {}
来源：http://mcp.andypj.xyz

TS:   class Admin extends User {}
来源：http://sow.pycfn.com

Java: class Admin extends User {}
来源：http://szw.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://atj.gzhubu.top

Ruby: class Admin < User; end
来源：http://nnj.hcnkem.com

C#:   class Admin : User {}
来源：http://yvd.iojbl.cn

[G06] 重写方法
来源：http://kne.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://bks.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://znx.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://cyz.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://gbg.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://exd.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pds.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://uuf.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://wyr.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://dyd.tian-w.cn

Py:   super().greet()
来源：http://lwz.mhx1999.top

PHP:  parent::greet();
来源：http://hnp.dianchejie.cn

JS:   super.greet();
来源：http://uml.shuidangran.top

TS:   super.greet();
来源：http://inf.hongshengwenyu.top

Java: super.greet();
来源：http://abt.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uep.gaohongyu789.top

Ruby: super
来源：http://kqa.jqgfzy.top

C#:   base.Greet();
来源：http://hic.ehwqpu.com

[G08] 静态方法与属性
来源：http://ftx.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pwy.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://fph.jinyuanbaomall.cn

JS:   static f() {}
来源：http://anc.jqgfzy.top

TS:   static f(): void {}
来源：http://mvb.nanxuanxn.top

Java: static void f() {}
来源：http://qqo.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cen.yvedp.cn

Ruby: def self.f; end
来源：http://otg.9152youxi.cn

C#:   public static void F() {}
来源：http://yih.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://aro.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://zov.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://umw.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jqi.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://hby.birdmap.top

Java: interface Shape { double area(); }
来源：http://ufj.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://uzq.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jfv.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://lze.quarkkingdee.top

[G10] 访问控制
来源：http://tcb.zhongyouzk.top

Py:   约定 _protected / __private（不强制）
来源：http://ali.hongshengwenyu.top

PHP:  public / protected / private
来源：http://dbg.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://drz.tian-w.cn

TS:   public / protected / private
来源：http://loq.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://xqa.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://msa.tian-w.cn

Ruby: public / protected / private
来源：http://fai.uphjek.com

C#:   public / protected / private / internal
来源：http://mbb.zhiwuduotai.top

[G11] getter / setter
来源：http://bvt.redwolf501.top

Py:   @property 与 @x.setter
来源：http://chy.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://bqc.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://ccw.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://euz.52xcode.cn

Java: public String getName() { return name; }
来源：http://lie.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bxs.aibaodan.cn

Ruby: attr_accessor :name
来源：http://yaq.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://xsc.snrcjt.cn

[G12] 对象转字符串
来源：http://squ.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://okv.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ksr.xziqi.cn

JS:   toString() { return this.name; }
来源：http://zkd.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://igo.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://kar.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qek.wangdashe.top

Ruby: def to_s; @name; end
来源：http://dkj.xinyue.icu

C#:   public override string ToString() => Name;
来源：http://dkz.0kj1m.cn

[G13] 判断对象类型
来源：http://xdw.jiagoushi.top

Py:   isinstance(u, User)
来源：http://utk.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://cbb.zycfv.cn

JS:   u instanceof User
来源：http://igk.gzhubu.top

TS:   u instanceof User
来源：http://mnj.daria6918.cn

Java: u instanceof User
来源：http://xqw.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zoe.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://tbt.daxiang520.top

C#:   u is User
来源：http://uwm.jqgufenzy.top

[G14] 数据类 / record
来源：http://eok.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jyw.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://pql.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://qgt.fanxiaobao.xyz


<!-- 参考信息 -->