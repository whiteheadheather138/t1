代发 wailian999

[E18] 模板占位符替换
来源：http://zln.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ulm.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mxs.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://shv.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://khx.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iyd.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gnh.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tiq.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wjn.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://abq.smart0.xyz

Py:   s.splitlines()
来源：http://zno.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://frd.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://oyu.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://rbv.ydjk.org.cn

Java: s.lines().toList()
来源：http://ewm.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://eks.shangyingyoupin.top

Ruby: s.lines
来源：http://rwn.zycfv.cn

C#:   s.Split('\n')
来源：http://nyv.epnwcf.com

[E20] 判断字符串是否为空
来源：http://usg.sweek.top

Py:   if not s:
来源：http://ahr.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lgc.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://luk.hesvh.cn

TS:   if (s === "") {}
来源：http://svv.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://diz.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://vpv.uphjek.com

Ruby: if s.empty?
来源：http://bvd.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://okf.dashuyun.cn

[E21] 超长截断加省略号
来源：http://jny.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blf.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://owd.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://toi.kuanghao11.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqv.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://whn.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://yxv.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://euk.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://azd.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://csr.redwolf501.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ckw.uphjek.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://klh.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zsu.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhj.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://inp.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jzr.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://zud.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://trs.chenlongwang.top

================================================================================
来源：http://ylc.tianlin.xyz

F. 文件与目录
来源：http://xtr.zhaomingkeji.xyz

================================================================================
来源：http://mfq.cashguo.top

[F01] 读取整个文件
来源：http://urj.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ddv.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://pno.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qii.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cfb.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tvc.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jpo.52xcode.cn

Ruby: File.read("a.txt")
来源：http://kfa.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://hgo.jiagoushi.top

[F02] 逐行读取文件
来源：http://zeg.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://egl.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fjx.aizwys.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dgu.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pvc.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vyk.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://raa.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rff.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gbw.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://hta.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vzi.fzhhl.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://anm.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jwz.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ban.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hhp.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tab.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://kjg.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fdd.ivvv.top

[F04] 追加写入文件
来源：http://rar.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://brr.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cut.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jzi.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hvs.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cyo.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uyh.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cyg.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lcx.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://ish.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mqw.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://frw.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://gxx.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://orn.kuanghao11.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xar.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://etq.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://pxz.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://ejj.jinghuilouyu.cn

[F06] 删除文件
来源：http://kqc.uphjek.com

Py:   os.remove("a.txt")
来源：http://luo.jlsjyb.cn

PHP:  unlink("a.txt");
来源：http://whm.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://msy.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oeo.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://udj.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://vxp.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://rme.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://gqp.fengsongda.top

[F07] 创建目录（含多级）
来源：http://vyf.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hfg.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jpa.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://opg.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kci.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yff.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jeg.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ylv.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xiv.yueranfly.top

[F08] 遍历目录
来源：http://otm.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://jxc.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fty.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://ksr.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://sln.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pum.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://vkf.sufxvd.cn

Ruby: Dir.children("dir")
来源：http://fwl.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://czn.zycfv.cn

[F09] 获取文件大小
来源：http://vkb.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://bfz.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://rig.yueranfly.top

JS:   fs.statSync("a.txt").size
来源：http://dvy.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://dlt.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://qpn.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dqj.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://nzi.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://fon.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://xqr.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://buz.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pcx.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rpf.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://yat.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vcg.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qhc.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cjd.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://osr.hysaishi.cn

[F11] 复制与移动文件
来源：http://tol.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://asi.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wuu.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iwv.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fnj.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uvx.fzhhl.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://due.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hoj.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vjs.yueranfly.top

[F12] CSV 读写
来源：http://eju.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vaa.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tts.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ubq.shanyushiyangkeji.top

TS:   // 同上
来源：http://crb.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cpp.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fxq.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iyx.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://jbd.zhaomingkeji.xyz

================================================================================
来源：http://gat.yangfankeji.com

G. 面向对象
来源：http://sau.yangfankeji.com

================================================================================
来源：http://yiw.epnwcf.com

[G01] 定义类
来源：http://yve.chenlongwang.top

Py:   class User: pass
来源：http://hkf.wangdashe.top

PHP:  class User {}
来源：http://xuo.smart0.xyz

JS:   class User {}
来源：http://zup.feifeiyinyue.top

TS:   class User { name: string = ""; }
来源：http://few.yj202588.top

Java: class User {}
来源：http://ndn.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://yey.havefunace.top

Ruby: class User; end
来源：http://rgg.jinqigfzy.top

C#:   class User {}
来源：http://yux.haohaochexian.top

[G02] 构造函数
来源：http://twx.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://jhd.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://wnf.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://ipj.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://rwn.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://lab.fehbvm.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gis.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://vxb.hysaishi.cn

C#:   public User(string name) { Name = name; }
来源：http://bzn.hongshengwenyu.top

[G03] 实例属性
来源：http://ghh.c1oappe.top

Py:   self.name = "x"
来源：http://xtp.jianghu66.top

PHP:  public string $name = "x";
来源：http://hye.hcnkem.com

JS:   this.name = "x";
来源：http://fyi.chenjidiqi.icu

TS:   name: string = "x";
来源：http://meq.ehwqpu.com

Java: private String name;
来源：http://grr.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kgp.bbcook.cn

Ruby: @name = "x"
来源：http://iti.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://uce.bbcook.cn

[G04] 定义方法
来源：http://fba.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://ban.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ivi.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://qrs.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://mhv.hcnkem.com

Java: String greet() { return name; }
来源：http://bij.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://vpf.wangshuangyany.cn

Ruby: def greet; @name; end
来源：http://qdx.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://eyh.wangdashe.top

[G05] 继承
来源：http://iqp.hywenlv.cn

Py:   class Admin(User): pass
来源：http://zzl.fengsongda.top

PHP:  class Admin extends User {}
来源：http://idt.yuxming.cn

JS:   class Admin extends User {}
来源：http://oxj.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://yty.fengsongda.top

Java: class Admin extends User {}
来源：http://mss.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xnk.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://mpp.xuanzx.com

C#:   class Admin : User {}
来源：http://owd.shuidangran.top

[G06] 重写方法
来源：http://fxt.yongpay.top

Py:   def greet(self): return "admin"
来源：http://hvs.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gxq.vqdsnc.cn

JS:   greet() { return "admin"; }
来源：http://vxg.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://rry.andypj.xyz

Java: @Override String greet() { return "admin"; }
来源：http://myy.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://abo.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://let.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://oth.snrcjt.cn

[G07] 调用父类方法
来源：http://qry.kuanghao11.cn

Py:   super().greet()
来源：http://tnd.ehwqpu.com

PHP:  parent::greet();
来源：http://foj.yonumen.top

JS:   super.greet();
来源：http://dzs.wangshuangyany.cn

TS:   super.greet();
来源：http://sep.0kj1m.cn

Java: super.greet();
来源：http://nnb.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mmw.fehbvm.com

Ruby: super
来源：http://roc.xinyue.icu

C#:   base.Greet();
来源：http://tvv.jqgfzy.top

[G08] 静态方法与属性
来源：http://jir.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://afb.fengsongda.top

PHP:  public static function f() {}
来源：http://geh.nanxinkj.top

JS:   static f() {}
来源：http://rcp.yuxming.cn

TS:   static f(): void {}
来源：http://nco.zdqjudy.top

Java: static void f() {}
来源：http://gya.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://all.hfpthk.cn

Ruby: def self.f; end
来源：http://gla.birdmap.top

C#:   public static void F() {}
来源：http://cjh.cheryme.top

[G09] 接口 / 抽象类
来源：http://qnj.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://lzj.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://gwi.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fpi.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://pyg.sysykeji.top

Java: interface Shape { double area(); }
来源：http://xnw.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://kay.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cip.ydzc1.top

C#:   interface IShape { double Area(); }
来源：http://uqu.jqgfzy.top

[G10] 访问控制
来源：http://bui.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://fng.fktsv.cn

PHP:  public / protected / private
来源：http://tbk.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://msj.ydzc1.top

TS:   public / protected / private
来源：http://iyz.ybcxt.top

Java: public / protected / private / 默认包级
来源：http://gcr.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cky.wangshuangyany.cn

Ruby: public / protected / private
来源：http://bva.0kj1m.cn

C#:   public / protected / private / internal
来源：http://jrg.jinyuanbaomall.cn

[G11] getter / setter
来源：http://fro.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://vnk.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ejq.ivvv.top

JS:   get name() { return this._name; }
来源：http://mnx.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://tcs.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://lqv.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://pjz.9152youxi.cn

Ruby: attr_accessor :name
来源：http://aru.52xcode.cn

C#:   public string Name { get; set; }
来源：http://obx.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://ynm.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://fca.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mhz.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://clt.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://ogy.zhiwuduotai.top

Java: @Override public String toString() { return name; }
来源：http://cct.c1oappe.top

Go:   func (u User) String() string { return u.Name }
来源：http://vgz.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://pxm.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://guj.hesvh.cn

[G13] 判断对象类型
来源：http://vht.9152youxi.cn

Py:   isinstance(u, User)
来源：http://dfv.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://hnm.cucudq.cn

JS:   u instanceof User
来源：http://ywy.xziqi.cn

TS:   u instanceof User
来源：http://ejj.dashuyun.cn

Java: u instanceof User
来源：http://mqh.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://nhq.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://bss.wangshuangyany.cn

C#:   u is User
来源：http://fyx.ybcxt.top

[G14] 数据类 / record
来源：http://evw.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://orx.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://iqe.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://rrr.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://mln.sweek.top

Java: record User(String name, int age) {}
来源：http://nzo.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://flw.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ibl.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://vuy.vehdjk.com

[G15] 枚举
来源：http://ksz.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ync.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dxc.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aww.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://diq.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://rci.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jkf.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://pye.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hon.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://wvd.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ofm.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://grx.snrcjt.cn

JS:   Object.entries(obj)
来源：http://ckh.yonumen.top

TS:   Object.entries(obj)
来源：http://grr.yj20258.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://udx.svipenyu.cn


<!-- 参考信息 -->