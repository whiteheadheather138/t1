代发 wailian999

PHP:  number_format(1234567);
来源：http://lxx.meibo888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dyg.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wfz.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fxr.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bgz.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qux.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://dzw.shanyushiyangtech.top

[E17] 首字母大写
来源：http://bvc.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://biv.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sws.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://trq.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mgy.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://orx.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://etk.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://qtt.wangdashe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uqm.bbcook.cn

[E18] 模板占位符替换
来源：http://bwb.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vas.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xwk.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://jwq.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://esn.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zwz.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://til.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gpl.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tna.nwbrower.top

[E19] 多行文本按行拆分
来源：http://flz.jqgufenzy.top

Py:   s.splitlines()
来源：http://hcv.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qlg.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://bbs.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://fip.jinqigfzy.top

Java: s.lines().toList()
来源：http://tes.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://vut.yj202588.top

Ruby: s.lines
来源：http://hyq.svipenyu.cn

C#:   s.Split('\n')
来源：http://bfz.havefunace.top

[E20] 判断字符串是否为空
来源：http://rvc.xingfuxueyuan.xyz

Py:   if not s:
来源：http://wtz.fzhhl.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lhw.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uae.yueranfly.top

TS:   if (s === "") {}
来源：http://kgc.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://qrg.jinqigufen.top

Go:   if s == "" {}
来源：http://ouk.ehwqpu.com

Ruby: if s.empty?
来源：http://hyc.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mym.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://xeg.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://you.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://djg.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qvf.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yum.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://upm.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://bux.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ims.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kwe.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://rmc.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nzx.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rdo.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nkl.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xyc.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nld.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://reh.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://xdt.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jls.yuanzhike.top

================================================================================
来源：http://kcs.jqgufenzy.top

F. 文件与目录
来源：http://kwa.cucudq.cn

================================================================================
来源：http://zqq.yongpay.top

[F01] 读取整个文件
来源：http://odq.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yzk.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://rcu.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hdu.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kkx.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xnm.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nue.bbcook.cn

Ruby: File.read("a.txt")
来源：http://zvo.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://abl.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://vmj.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qyz.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hfi.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nzx.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rta.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jgv.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pwy.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fwb.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vbk.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://mdd.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nrv.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://awf.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mli.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oie.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yxk.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kkx.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://bag.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lzl.zdbjq.cn

[F04] 追加写入文件
来源：http://tst.cucudq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uev.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ulc.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uvp.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zfj.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yhu.zhoulong.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ols.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xvx.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qev.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://krm.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nbj.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://mar.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://icw.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://gxi.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wyn.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nui.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://wlt.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://cyh.birdmap.top

[F06] 删除文件
来源：http://irc.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://lne.xziqi.cn

PHP:  unlink("a.txt");
来源：http://bga.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gsg.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://yfx.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://exy.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://hfi.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://amg.havefunace.top

C#:   File.Delete("a.txt");
来源：http://odq.redwolf501.top

[F07] 创建目录（含多级）
来源：http://ztp.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oaf.xziqi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mcj.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bfa.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://emy.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ily.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vyb.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://onq.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://prv.yongpay.top

[F08] 遍历目录
来源：http://hrn.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tgg.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vve.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://vnp.chenzaomai.com

TS:   fs.readdirSync("dir")
来源：http://ham.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bzl.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ibx.yj20258888.top

Ruby: Dir.children("dir")
来源：http://ihz.ctjpmb.com

C#:   Directory.GetFiles("dir")
来源：http://iyj.bbcook.cn

[F09] 获取文件大小
来源：http://lzp.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://fhy.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://fuu.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://yhd.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://ndi.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://sav.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qbx.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://omf.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://ssi.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://rfq.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zsj.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cod.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nug.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://dte.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mhu.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yhs.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uzn.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lzm.zhoulong.xyz

[F11] 复制与移动文件
来源：http://zlr.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hoz.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bex.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mxt.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gwg.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tie.ybcxt.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gko.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ove.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lbg.shangyingyoupin.top

[F12] CSV 读写
来源：http://jdp.jqgfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ovn.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qqk.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://myn.redwolf501.top

TS:   // 同上
来源：http://jdg.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mqf.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xhu.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zqa.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tmr.wangshuangyany.cn

================================================================================
来源：http://lui.shuidangran.top

G. 面向对象
来源：http://qta.ctjpmb.com

================================================================================
来源：http://knn.jlsjyb.cn

[G01] 定义类
来源：http://enz.hcnkem.com

Py:   class User: pass
来源：http://asj.tianlin.xyz

PHP:  class User {}
来源：http://ela.svipenyu.cn

JS:   class User {}
来源：http://tkg.sweek.top

TS:   class User { name: string = ""; }
来源：http://gib.vqdsnc.cn

Java: class User {}
来源：http://ftc.cashguo.top

Go:   type User struct { Name string }
来源：http://fbe.sufxvd.cn

Ruby: class User; end
来源：http://tfu.yvedp.cn

C#:   class User {}
来源：http://nek.daria6918.cn

[G02] 构造函数
来源：http://xmh.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://xfh.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://awv.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://jbk.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://yox.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://fog.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cvs.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://qyr.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://oik.jinqigufen.top

[G03] 实例属性
来源：http://poy.feifeiyinyue.top

Py:   self.name = "x"
来源：http://gyw.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://pcl.tianlin.xyz

JS:   this.name = "x";
来源：http://dhk.redwolf501.top

TS:   name: string = "x";
来源：http://bpu.yueranfly.top

Java: private String name;
来源：http://vtw.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ocs.gzhubu.top

Ruby: @name = "x"
来源：http://yrt.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://peu.52xcode.cn

[G04] 定义方法
来源：http://ryd.yueranfly.top

Py:   def greet(self): return self.name
来源：http://iaa.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ivl.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://qph.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://vmb.iojbl.cn

Java: String greet() { return name; }
来源：http://uqd.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lzk.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://pbj.meibo888.top

C#:   public string Greet() => Name;
来源：http://pus.xinyue.icu

[G05] 继承
来源：http://vvs.9152youxi.cn

Py:   class Admin(User): pass
来源：http://eqz.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://rtg.iojbl.cn

JS:   class Admin extends User {}
来源：http://taz.sufxvd.cn

TS:   class Admin extends User {}
来源：http://xjj.zdbjq.cn

Java: class Admin extends User {}
来源：http://sfr.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xef.gzhubu.top

Ruby: class Admin < User; end
来源：http://dmz.nanxuanxn.top

C#:   class Admin : User {}
来源：http://mks.chenlongwang.top

[G06] 重写方法
来源：http://qbr.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://qbu.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bdl.yj20258.top

JS:   greet() { return "admin"; }
来源：http://csy.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://lbh.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://lkw.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://huq.sxryk.cn

Ruby: def greet; "admin"; end
来源：http://lem.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://ztm.tianlin.xyz

[G07] 调用父类方法
来源：http://jwx.feifeiyinyue.top

Py:   super().greet()
来源：http://hbr.xylfe.cn

PHP:  parent::greet();
来源：http://qmf.guannengcc.top

JS:   super.greet();
来源：http://cto.yj202588.top

TS:   super.greet();
来源：http://rvp.ppjwa.cn

Java: super.greet();
来源：http://cre.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jnf.hcnkem.com

Ruby: super
来源：http://npn.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://yte.fengsongda.top

[G08] 静态方法与属性
来源：http://yzy.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tci.yuxming.cn

PHP:  public static function f() {}
来源：http://mne.svipenyu.cn

JS:   static f() {}
来源：http://yjo.pengpengdd.cyou

TS:   static f(): void {}
来源：http://bcd.sufxvd.cn

Java: static void f() {}
来源：http://yqz.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bws.aizwys.cn

Ruby: def self.f; end
来源：http://lir.kuanghao11.cn

C#:   public static void F() {}
来源：http://fbe.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://chm.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://uha.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://rbz.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://krr.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://bzf.nwbrower.top

Java: interface Shape { double area(); }
来源：http://znk.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://udv.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ozm.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://afa.haohaochexian.top

[G10] 访问控制
来源：http://rli.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://zuc.yfazqb.com

PHP:  public / protected / private
来源：http://dvr.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://kis.hnxiangtu.top

TS:   public / protected / private
来源：http://kzp.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://qpl.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wzq.yanxiufei.cn

Ruby: public / protected / private
来源：http://mdy.xuanzx.com

C#:   public / protected / private / internal
来源：http://hjf.tarul.cn

[G11] getter / setter
来源：http://aei.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://rxt.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://znb.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://upn.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://ktb.yueranfly.top

Java: public String getName() { return name; }
来源：http://qro.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://pyq.fengsongda.top

Ruby: attr_accessor :name
来源：http://osj.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://uhq.aizwys.cn

[G12] 对象转字符串
来源：http://lsy.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://gaf.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://grl.vehdjk.com

JS:   toString() { return this.name; }
来源：http://meo.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://tik.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://jzc.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ube.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://rbs.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://sif.fzhhl.top

[G13] 判断对象类型
来源：http://kwf.aibaodan.cn

Py:   isinstance(u, User)
来源：http://voq.quarkkingdee.top

PHP:  $u instanceof User
来源：http://pvb.zhijiandao.cn

JS:   u instanceof User
来源：http://yhd.yj202588.top

TS:   u instanceof User
来源：http://vxk.vqdsnc.cn

Java: u instanceof User
来源：http://jhy.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://swb.tarul.cn

Ruby: u.is_a?(User)
来源：http://wwc.wangdashe.top

C#:   u is User
来源：http://mje.cqqwz.cn

[G14] 数据类 / record
来源：http://hkp.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dvb.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://gvk.tarul.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vtd.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://oyi.sysykeji.top

Java: record User(String name, int age) {}
来源：http://pby.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://hkg.yangfankeji.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ffu.fengsongda.top


<!-- 参考信息 -->