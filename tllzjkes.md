代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mqv.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://clx.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dnv.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wfj.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bxs.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jup.zhoulong.xyz

Ruby: s.capitalize
来源：http://odn.52xcode.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nvh.sweek.top

[E18] 模板占位符替换
来源：http://quy.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pkd.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sow.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ayx.jinghuilouyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sdz.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://znw.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://foo.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ybb.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kds.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://trq.sjlbkw.cn

Py:   s.splitlines()
来源：http://hck.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vht.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://dcf.ydjk.org.cn

TS:   s.split(/\r?\n/)
来源：http://mqu.ydjk.org.cn

Java: s.lines().toList()
来源：http://smh.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://vvu.hongshengwenyu.top

Ruby: s.lines
来源：http://tqt.yangfankeji.com

C#:   s.Split('\n')
来源：http://gfn.smart0.xyz

[E20] 判断字符串是否为空
来源：http://gnj.hnxiangtu.top

Py:   if not s:
来源：http://qxm.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pcx.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://att.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://pth.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://qdc.meibo888.top

Go:   if s == "" {}
来源：http://gdt.nanxuanxn.top

Ruby: if s.empty?
来源：http://ydy.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eac.zdbjq.cn

[E21] 超长截断加省略号
来源：http://sxy.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kgq.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bpf.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nsf.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yek.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nrx.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://gra.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jtu.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ayr.svipenyu.cn

[E22] 字节长度与字符长度
来源：http://hnd.yonumen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vdw.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cwd.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ryc.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dfq.smart0.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gsu.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oel.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://wcq.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xfl.nanxuanxn.top

================================================================================
来源：http://ozt.zycfv.cn

F. 文件与目录
来源：http://klm.tarul.cn

================================================================================
来源：http://qlt.yj20258.top

[F01] 读取整个文件
来源：http://rxo.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gzo.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://oof.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ees.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mav.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://exs.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gzk.tarul.cn

Ruby: File.read("a.txt")
来源：http://kls.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://nmn.yj20258.top

[F02] 逐行读取文件
来源：http://vor.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ada.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://umj.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://njj.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dvl.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hhf.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uau.pengpengdd.cyou

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nps.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://flb.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://etk.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gaa.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lmy.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vrl.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cqt.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cdn.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://swm.xuetiantiany.cn

Ruby: File.write("a.txt", "hi")
来源：http://aoq.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ppy.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://gqs.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uij.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kru.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://efq.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yha.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ufr.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dfn.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yvy.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gcz.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://ddl.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ift.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://czf.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://akl.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://cuo.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://zgw.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://skl.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://njr.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://pum.nwbrower.top

[F06] 删除文件
来源：http://byc.shuidangran.top

Py:   os.remove("a.txt")
来源：http://npl.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://ntr.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eka.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://jqh.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://meu.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://ozq.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://szz.yanxiufei.cn

C#:   File.Delete("a.txt");
来源：http://zbm.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://opo.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zmq.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qzp.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kgn.jiagoushi.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yxs.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zbc.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wkl.hysaishi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xot.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://opy.gaohongyu789.top

[F08] 遍历目录
来源：http://sot.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kdj.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aic.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://efo.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://jqt.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://upd.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yoc.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://omq.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://xbf.sxryk.cn

[F09] 获取文件大小
来源：http://ckq.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://kpt.sysykeji.top

PHP:  filesize("a.txt");
来源：http://gul.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://lxc.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://ton.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fqs.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wyq.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://fvb.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://ydp.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://yqu.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://thy.gzhubu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vwv.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ngi.52xcode.cn

TS:   path.extname("a.txt")
来源：http://hvm.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qbi.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dmh.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wfz.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://quj.0kj1m.cn

[F11] 复制与移动文件
来源：http://fva.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ygv.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oey.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oef.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xag.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ysy.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wpv.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://etc.jianghu66.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ira.nanxinkj.top

[F12] CSV 读写
来源：http://mic.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xls.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zqa.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fde.fehbvm.com

TS:   // 同上
来源：http://vch.hysaishi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://khr.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hib.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nwi.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bqd.316326.xyz

================================================================================
来源：http://twh.ybcxt.top

G. 面向对象
来源：http://wlz.ehwqpu.com

================================================================================
来源：http://tkn.snrcjt.cn

[G01] 定义类
来源：http://eoe.jyoumei.cn

Py:   class User: pass
来源：http://drn.yuanzhike.top

PHP:  class User {}
来源：http://zsn.meibo888.top

JS:   class User {}
来源：http://jvo.cashguo.top

TS:   class User { name: string = ""; }
来源：http://jyg.smart0.xyz

Java: class User {}
来源：http://tiz.tanke756.top

Go:   type User struct { Name string }
来源：http://ybz.yuxming.cn

Ruby: class User; end
来源：http://xeb.shanyushiyangtech.top

C#:   class User {}
来源：http://tft.feifeiyinyue.top

[G02] 构造函数
来源：http://bpr.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://cyk.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://jzg.ivvv.top

JS:   constructor(name) { this.name = name; }
来源：http://vfe.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://jvx.ydzc1.top

Java: User(String name) { this.name = name; }
来源：http://tfq.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fpj.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://uaq.zhoulong.xyz

C#:   public User(string name) { Name = name; }
来源：http://yzl.c1oappe.top

[G03] 实例属性
来源：http://lcv.hammf.cn

Py:   self.name = "x"
来源：http://evo.cdnleiting.top

PHP:  public string $name = "x";
来源：http://dfo.xuetiantiany.cn

JS:   this.name = "x";
来源：http://gym.ivvv.top

TS:   name: string = "x";
来源：http://zux.yonumen.top

Java: private String name;
来源：http://xvc.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tgl.yongpay.top

Ruby: @name = "x"
来源：http://vjp.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://npb.hesvh.cn

[G04] 定义方法
来源：http://cbe.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://cjv.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fey.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://icp.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://mrq.ivvv.top

Java: String greet() { return name; }
来源：http://daw.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xyz.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://ssj.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://zfh.xingfuxueyuan.xyz

[G05] 继承
来源：http://vqq.jiagoushi.top

Py:   class Admin(User): pass
来源：http://mac.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://tvv.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://ejp.yangfankeji.com

TS:   class Admin extends User {}
来源：http://amb.chenlongwang.top

Java: class Admin extends User {}
来源：http://wcq.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://puu.andypj.xyz

Ruby: class Admin < User; end
来源：http://zle.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://lgp.xuanzx.com

[G06] 重写方法
来源：http://vkl.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://vxc.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ykq.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://xlv.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://dzi.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://qoo.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cyt.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://mgq.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://oyp.tian-w.cn

[G07] 调用父类方法
来源：http://dxh.wangshuangyany.cn

Py:   super().greet()
来源：http://guw.xylfe.cn

PHP:  parent::greet();
来源：http://nae.hfpthk.cn

JS:   super.greet();
来源：http://mko.yuxming.cn

TS:   super.greet();
来源：http://rks.chenjidiqi.icu

Java: super.greet();
来源：http://bkk.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://asu.sysykeji.top

Ruby: super
来源：http://exm.quarkkingdee.top

C#:   base.Greet();
来源：http://sio.yanxiufei.cn

[G08] 静态方法与属性
来源：http://edk.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://owd.yangfankeji.com

PHP:  public static function f() {}
来源：http://jcl.zycfv.cn

JS:   static f() {}
来源：http://acd.yj20258888.top

TS:   static f(): void {}
来源：http://ubq.yonumen.top

Java: static void f() {}
来源：http://ptq.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pyk.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://wfg.jqgfzy.top

C#:   public static void F() {}
来源：http://jvq.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://kdj.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://ymo.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qus.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://auy.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://xgp.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://zcb.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://jbx.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wkm.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://dsr.zdbjq.cn

[G10] 访问控制
来源：http://vwr.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://wbu.gotoacloud.top

PHP:  public / protected / private
来源：http://dta.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://xae.guowangkeji.top

TS:   public / protected / private
来源：http://cfo.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://kbl.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mvp.shangyingyoupin.top

Ruby: public / protected / private
来源：http://wms.c1oappe.top

C#:   public / protected / private / internal
来源：http://nhd.zhiwuduotai.top

[G11] getter / setter
来源：http://axd.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://say.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pzq.316326.xyz

JS:   get name() { return this._name; }
来源：http://dzm.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://ner.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://qwf.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://seq.aibaodan.cn

Ruby: attr_accessor :name
来源：http://kbt.epnwcf.com

C#:   public string Name { get; set; }
来源：http://xhd.zhiwuduotai.top

[G12] 对象转字符串
来源：http://haj.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://dwx.shzxlz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://irz.gzhubu.top

JS:   toString() { return this.name; }
来源：http://hyd.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://iuu.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://abe.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://yrb.zycfv.cn

Ruby: def to_s; @name; end
来源：http://iww.hcnkem.com

C#:   public override string ToString() => Name;
来源：http://elj.zdqjudy.top

[G13] 判断对象类型
来源：http://xfv.zycfv.cn

Py:   isinstance(u, User)
来源：http://ofw.yvedp.cn

PHP:  $u instanceof User
来源：http://oxj.316326.xyz

JS:   u instanceof User
来源：http://mxk.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://dti.dashuyun.cn

Java: u instanceof User
来源：http://mgt.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rkb.daria6918.cn

Ruby: u.is_a?(User)
来源：http://zbp.gotoacloud.top

C#:   u is User
来源：http://huj.quarkkingdee.top

[G14] 数据类 / record
来源：http://pbm.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gtg.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://jsd.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://ctq.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://tef.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://qgx.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://rjv.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gxz.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://xnt.pycfn.com

[G15] 枚举
来源：http://sdq.xziqi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gfa.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://swn.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rin.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cjv.tianlin.xyz

Java: enum Color { RED, GREEN }
来源：http://cqe.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tuf.hesvh.cn


<!-- 参考信息 -->