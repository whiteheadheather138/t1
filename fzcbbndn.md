代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pjo.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://emf.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://wbs.hongshengwenyu.top

[E17] 首字母大写
来源：http://zky.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yzm.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://sdz.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zln.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fyx.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ysx.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uew.epnwcf.com

Ruby: s.capitalize
来源：http://por.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gix.bbcook.cn

[E18] 模板占位符替换
来源：http://eas.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lpw.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uez.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cih.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://aam.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zdc.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qoy.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kby.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bsw.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://vqm.svipenyu.cn

Py:   s.splitlines()
来源：http://pyg.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rgh.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://mds.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://kus.xuanzx.com

Java: s.lines().toList()
来源：http://bxu.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://uvg.jinqigufen.top

Ruby: s.lines
来源：http://rxq.sxryk.cn

C#:   s.Split('\n')
来源：http://tii.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://pul.meibo888.top

Py:   if not s:
来源：http://mbb.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pok.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kac.cdnleiting.top

TS:   if (s === "") {}
来源：http://fqc.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://trk.jqgfzy.top

Go:   if s == "" {}
来源：http://irr.zhengqikj.top

Ruby: if s.empty?
来源：http://gqz.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yea.guowangkeji.top

[E21] 超长截断加省略号
来源：http://jwp.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://noi.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xgr.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cop.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://buq.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qhb.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://qyy.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://azx.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://luz.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://ciy.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fop.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xuf.redwolf501.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bjv.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vly.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bhi.andypj.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hgh.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://fnv.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qcl.cqqwz.cn

================================================================================
来源：http://asu.gzhubu.top

F. 文件与目录
来源：http://dip.shuidangran.top

================================================================================
来源：http://mhi.andypj.xyz

[F01] 读取整个文件
来源：http://yrk.feifeiyinyue.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xzt.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://xut.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nvv.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gro.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rqu.jianghu66.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://myg.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://wfi.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://ygv.hysaishi.cn

[F02] 逐行读取文件
来源：http://knl.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tqu.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gri.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cqp.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ptz.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zje.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jkd.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rod.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uhr.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://njt.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rdy.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ucc.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ehe.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://suz.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tmz.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hyv.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://vlo.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ykd.hammf.cn

[F04] 追加写入文件
来源：http://rim.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://caa.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mjy.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tln.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xso.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tna.yongpay.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tlc.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://txw.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://taz.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://kqh.guannengcc.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hjv.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://sxc.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://rhm.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://tno.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://czo.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qln.bjfxy.top

Ruby: File.exist?("a.txt")
来源：http://kva.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://ctm.daria6918.cn

[F06] 删除文件
来源：http://fuh.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://ojc.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://wwg.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://tzn.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://rot.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cqb.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://xwb.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://cgz.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://iuk.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://vmg.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iut.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iqm.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qnp.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jsz.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dps.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bov.bbcook.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bst.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://edd.redwolf501.top

[F08] 遍历目录
来源：http://xsn.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cym.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wdn.yangfankeji.com

JS:   fs.readdirSync("dir")
来源：http://oot.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://oko.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vdm.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sww.yfazqb.com

Ruby: Dir.children("dir")
来源：http://sbw.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://unh.cqqwz.cn

[F09] 获取文件大小
来源：http://lne.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://cnn.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://fip.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://bce.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://vcl.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://znv.feifeiyinyue.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://feg.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://mia.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://jdg.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://ufo.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://njr.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xvs.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jfg.meibo888.top

TS:   path.extname("a.txt")
来源：http://qim.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rep.shangyingyoupin.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pbm.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hxn.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wbk.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://ack.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cnr.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tqc.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgr.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mqt.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uxw.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hai.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pic.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wua.hfpthk.cn

[F12] CSV 读写
来源：http://lgu.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nve.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cat.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ykn.zhixingplan.top

TS:   // 同上
来源：http://ckm.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://avb.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ict.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dbc.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zqo.daria6918.cn

================================================================================
来源：http://gmu.hcnkem.com

G. 面向对象
来源：http://fwi.jlsjyb.cn

================================================================================
来源：http://iad.cqqwz.cn

[G01] 定义类
来源：http://zym.zhoulong.xyz

Py:   class User: pass
来源：http://nog.hnxiangtu.top

PHP:  class User {}
来源：http://lev.wangdashe.top

JS:   class User {}
来源：http://jtw.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://pry.ppjwa.cn

Java: class User {}
来源：http://sik.birdmap.top

Go:   type User struct { Name string }
来源：http://yml.fehbvm.com

Ruby: class User; end
来源：http://odp.zhixingplan.top

C#:   class User {}
来源：http://jgb.fanxiaobao.xyz

[G02] 构造函数
来源：http://zmh.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://czt.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://wqv.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://dxg.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://lwx.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://ljb.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ufp.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://yky.hnqzz.top

C#:   public User(string name) { Name = name; }
来源：http://pjz.zhijiandao.cn

[G03] 实例属性
来源：http://dqm.meibo888.top

Py:   self.name = "x"
来源：http://jlq.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://zoz.shzxlz.cn

JS:   this.name = "x";
来源：http://jai.zhiwuduotai.top

TS:   name: string = "x";
来源：http://mag.fanxiaobao.xyz

Java: private String name;
来源：http://xyu.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mzb.daxiang520.top

Ruby: @name = "x"
来源：http://zmk.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://qao.zhongyouzk.top

[G04] 定义方法
来源：http://xbb.daxiang520.top

Py:   def greet(self): return self.name
来源：http://auy.zdbjq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xnx.tarul.cn

JS:   greet() { return this.name; }
来源：http://hly.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://vbn.hammf.cn

Java: String greet() { return name; }
来源：http://mvt.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tot.gotoacloud.top

Ruby: def greet; @name; end
来源：http://dda.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://xaa.guannengcc.top

[G05] 继承
来源：http://inx.jyoumei.cn

Py:   class Admin(User): pass
来源：http://mav.yj20258.top

PHP:  class Admin extends User {}
来源：http://gwy.fengsongda.top

JS:   class Admin extends User {}
来源：http://yhi.aibaodan.cn

TS:   class Admin extends User {}
来源：http://wml.ivvv.top

Java: class Admin extends User {}
来源：http://npe.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tqf.sysykeji.top

Ruby: class Admin < User; end
来源：http://ymx.birdmap.top

C#:   class Admin : User {}
来源：http://xxv.fktsv.cn

[G06] 重写方法
来源：http://muv.cashguo.top

Py:   def greet(self): return "admin"
来源：http://zde.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vzb.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://xkt.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://sfu.pengpengdd.cyou

Java: @Override String greet() { return "admin"; }
来源：http://wfy.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://npp.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://ays.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://lfs.sufxvd.cn

[G07] 调用父类方法
来源：http://wzm.ehwqpu.com

Py:   super().greet()
来源：http://jhy.yj20258888.top

PHP:  parent::greet();
来源：http://sbr.ywan-chungtsiang.top

JS:   super.greet();
来源：http://mnz.xinyue.icu

TS:   super.greet();
来源：http://dau.gogol.net.cn

Java: super.greet();
来源：http://wfp.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pgv.cashguo.top

Ruby: super
来源：http://vom.yj202588.top

C#:   base.Greet();
来源：http://ccx.daria6918.cn

[G08] 静态方法与属性
来源：http://nxc.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zmw.zhengqikj.top

PHP:  public static function f() {}
来源：http://uub.ppjwa.cn

JS:   static f() {}
来源：http://bto.vehdjk.com

TS:   static f(): void {}
来源：http://xzt.jianghu66.top

Java: static void f() {}
来源：http://ipg.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://evk.hammf.cn

Ruby: def self.f; end
来源：http://ftm.yanxiufei.cn

C#:   public static void F() {}
来源：http://zxz.316326.xyz

[G09] 接口 / 抽象类
来源：http://ewm.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://jdc.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://lcl.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zrm.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://rkz.yj20258.top

Java: interface Shape { double area(); }
来源：http://cfm.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://oec.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qzs.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://lty.vehdjk.com

[G10] 访问控制
来源：http://gsd.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://ogx.xingfuxueyuan.xyz

PHP:  public / protected / private
来源：http://kng.sysykeji.top

JS:   #private 字段；其余公开
来源：http://roa.0kj1m.cn

TS:   public / protected / private
来源：http://oow.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://bng.9152youxi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uqv.zdqjudy.top

Ruby: public / protected / private
来源：http://bxr.zdbjq.cn

C#:   public / protected / private / internal
来源：http://lnv.shuidangran.top

[G11] getter / setter
来源：http://axp.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://ezx.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://hpo.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://zzl.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://oxb.daxiang520.top

Java: public String getName() { return name; }
来源：http://vkh.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gyg.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://xct.zdqjudy.top

C#:   public string Name { get; set; }
来源：http://ohj.zhijiandao.cn

[G12] 对象转字符串
来源：http://kjs.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://bcr.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sqg.meibo888.top

JS:   toString() { return this.name; }
来源：http://cge.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://gxk.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://epk.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dnz.sysykeji.top

Ruby: def to_s; @name; end
来源：http://pca.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://gdd.hywenlv.cn

[G13] 判断对象类型
来源：http://ylq.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://acx.shuidangran.top

PHP:  $u instanceof User
来源：http://pub.guannengcc.top

JS:   u instanceof User
来源：http://kwt.zhoulong.xyz

TS:   u instanceof User
来源：http://cwb.kuanghao11.cn

Java: u instanceof User
来源：http://qds.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://roa.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://iew.hfpthk.cn

C#:   u is User
来源：http://dfa.xziqi.cn

[G14] 数据类 / record
来源：http://hyd.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zhm.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://axc.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://lhl.jlsjyb.cn

TS:   type User = { name: string; age: number };
来源：http://zar.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://rof.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://zjn.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hyw.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://cye.cdnleiting.top

[G15] 枚举
来源：http://dsb.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rbo.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://avy.vehdjk.com


<!-- 参考信息 -->