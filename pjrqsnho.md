代发 wailian999

[E18] 模板占位符替换
来源：http://qzv.jiagoushi.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lbo.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fds.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wyb.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cab.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kve.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rpz.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qsz.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ido.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://qjw.zhijiandao.cn

Py:   s.splitlines()
来源：http://oxf.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ygw.nwbrower.top

JS:   s.split(/\r?\n/)
来源：http://hlf.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://woi.smart0.xyz

Java: s.lines().toList()
来源：http://zsf.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://epo.gzhubu.top

Ruby: s.lines
来源：http://pjx.yonumen.top

C#:   s.Split('\n')
来源：http://wuz.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://yaa.epnwcf.com

Py:   if not s:
来源：http://pbv.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gpw.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zjv.jiagoushi.top

TS:   if (s === "") {}
来源：http://grh.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://vnb.yonumen.top

Go:   if s == "" {}
来源：http://ytd.yanxiufei.cn

Ruby: if s.empty?
来源：http://rig.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sxl.hfpthk.cn

[E21] 超长截断加省略号
来源：http://ulg.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kca.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cez.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fjo.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kil.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mql.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://vlt.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://owg.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://diz.aizwys.cn

[E22] 字节长度与字符长度
来源：http://hwv.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aga.hammf.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dnq.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oqe.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vxy.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jop.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rcp.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://pzl.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yoe.daria6918.cn

================================================================================
来源：http://ayu.xuetiantiany.cn

F. 文件与目录
来源：http://rqm.dashuyun.cn

================================================================================
来源：http://opm.ivvv.top

[F01] 读取整个文件
来源：http://kbg.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xrd.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://bck.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://omx.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hsp.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://obo.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gid.xinyue.icu

Ruby: File.read("a.txt")
来源：http://ost.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://rga.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://kbo.sjlbkw.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vol.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gde.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ldz.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tae.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qvy.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://npp.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cec.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://anw.sweek.top

[F03] 写入文件（覆盖）
来源：http://pcv.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xez.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://dgd.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vdq.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hrd.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wup.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jpr.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://rhj.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tgk.birdmap.top

[F04] 追加写入文件
来源：http://equ.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sjz.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://reu.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gia.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://enk.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://txj.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kbv.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ehk.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tdr.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://qau.jqgfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ner.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://oeg.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://jpx.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://snj.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mhd.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xsq.dianchejie.cn

Ruby: File.exist?("a.txt")
来源：http://ero.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://zrm.hnqzz.top

[F06] 删除文件
来源：http://hka.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://cyi.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://rpa.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://mji.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://cdb.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://byk.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://yjh.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://fdv.yonumen.top

C#:   File.Delete("a.txt");
来源：http://gkw.hcnkem.com

[F07] 创建目录（含多级）
来源：http://mcf.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vkg.52xcode.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ybk.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jol.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nwd.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dgp.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nwp.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tet.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zlj.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://gqh.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tdf.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xyr.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://bqb.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://hay.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lzb.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mbv.xinyue.icu

Ruby: Dir.children("dir")
来源：http://elj.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://wtb.vqdsnc.cn

[F09] 获取文件大小
来源：http://ssu.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://bje.yuxming.cn

PHP:  filesize("a.txt");
来源：http://ajp.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://yup.svipenyu.cn

TS:   fs.statSync("a.txt").size
来源：http://grv.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://npb.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pud.shuidangran.top

Ruby: File.size("a.txt")
来源：http://hou.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://mwc.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://rjq.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dac.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dah.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://efi.iojbl.cn

TS:   path.extname("a.txt")
来源：http://nou.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ijd.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://upx.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nhg.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dpm.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://lgs.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ptd.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wuf.yj20258.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zdc.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uhm.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iez.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wzd.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://him.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rvv.dianchejie.cn

[F12] CSV 读写
来源：http://pps.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mlx.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iha.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cdo.zhixingplan.top

TS:   // 同上
来源：http://ajn.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cnq.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zdm.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://app.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://svw.chenzaomai.com

================================================================================
来源：http://tea.sjlbkw.cn

G. 面向对象
来源：http://chj.yangfankeji.com

================================================================================
来源：http://wrr.jinqigufen.top

[G01] 定义类
来源：http://roi.chenzaomai.com

Py:   class User: pass
来源：http://pjo.dianchejie.cn

PHP:  class User {}
来源：http://xuc.gogol.net.cn

JS:   class User {}
来源：http://tpa.cheryme.top

TS:   class User { name: string = ""; }
来源：http://akd.ybcxt.top

Java: class User {}
来源：http://ott.yongpay.top

Go:   type User struct { Name string }
来源：http://uju.zhixingplan.top

Ruby: class User; end
来源：http://fql.fktsv.cn

C#:   class User {}
来源：http://ocf.nanxuanxn.top

[G02] 构造函数
来源：http://gmo.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://itl.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://cha.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://pca.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://hyh.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://nbm.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dro.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://vfy.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://deb.zhaomingkeji.xyz

[G03] 实例属性
来源：http://jon.cqqwz.cn

Py:   self.name = "x"
来源：http://dwr.haohaochexian.top

PHP:  public string $name = "x";
来源：http://zoz.hongshengwenyu.top

JS:   this.name = "x";
来源：http://gzu.jlsjyb.cn

TS:   name: string = "x";
来源：http://hkp.xziqi.cn

Java: private String name;
来源：http://pze.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rjq.birdmap.top

Ruby: @name = "x"
来源：http://ttd.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://bvf.cucudq.cn

[G04] 定义方法
来源：http://brz.ybcxt.top

Py:   def greet(self): return self.name
来源：http://kjr.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://aji.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://xej.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://wuj.fengsongda.top

Java: String greet() { return name; }
来源：http://chw.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mhm.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://shr.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://bge.zhijiandao.cn

[G05] 继承
来源：http://dxn.sweek.top

Py:   class Admin(User): pass
来源：http://lti.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://pux.bjfxy.top

JS:   class Admin extends User {}
来源：http://pcs.wangdashe.top

TS:   class Admin extends User {}
来源：http://cse.feifeiyinyue.top

Java: class Admin extends User {}
来源：http://agt.sjlbkw.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hts.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://mox.xylfe.cn

C#:   class Admin : User {}
来源：http://hhx.zhongyouzk.top

[G06] 重写方法
来源：http://whn.sysykeji.top

Py:   def greet(self): return "admin"
来源：http://qvu.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://fbm.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://rnu.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://mtf.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://mhq.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qhy.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://hvx.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://eyi.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://irn.cucudq.cn

Py:   super().greet()
来源：http://gol.mhx1999.top

PHP:  parent::greet();
来源：http://feq.hammf.cn

JS:   super.greet();
来源：http://rwl.jiagoushi.top

TS:   super.greet();
来源：http://bnr.sufxvd.cn

Java: super.greet();
来源：http://czc.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pre.ctjpmb.com

Ruby: super
来源：http://dvm.epnwcf.com

C#:   base.Greet();
来源：http://coh.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://pns.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rny.sysykeji.top

PHP:  public static function f() {}
来源：http://fko.redwolf501.top

JS:   static f() {}
来源：http://yij.hcnkem.com

TS:   static f(): void {}
来源：http://xvq.birdmap.top

Java: static void f() {}
来源：http://tph.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wbb.dashuyun.cn

Ruby: def self.f; end
来源：http://esk.aibaodan.cn

C#:   public static void F() {}
来源：http://tzq.yvedp.cn

[G09] 接口 / 抽象类
来源：http://wph.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://zmb.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://dnh.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://owf.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://bzn.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://njz.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://mfy.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nyq.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://xsc.birdmap.top

[G10] 访问控制
来源：http://acz.bjfxy.top

Py:   约定 _protected / __private（不强制）
来源：http://lrp.yanxiufei.cn

PHP:  public / protected / private
来源：http://lzr.gotoacloud.top

JS:   #private 字段；其余公开
来源：http://ody.cashguo.top

TS:   public / protected / private
来源：http://wxi.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://rxf.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://teu.yvedp.cn

Ruby: public / protected / private
来源：http://ggo.ppjwa.cn

C#:   public / protected / private / internal
来源：http://hcn.yuanzhike.top

[G11] getter / setter
来源：http://gbp.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://ehh.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ecj.hnqzz.top

JS:   get name() { return this._name; }
来源：http://dzf.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://vnr.c1oappe.top

Java: public String getName() { return name; }
来源：http://rok.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xco.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://xbe.uphjek.com

C#:   public string Name { get; set; }
来源：http://yxc.nanxinkj.top

[G12] 对象转字符串
来源：http://pyq.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://vai.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://iev.jianghu66.top

JS:   toString() { return this.name; }
来源：http://ewq.tanke756.top

TS:   toString(): string { return this.name; }
来源：http://dsq.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://fld.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://rcv.shuidangran.top

Ruby: def to_s; @name; end
来源：http://isi.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://iid.ywan-chungtsiang.top

[G13] 判断对象类型
来源：http://jdq.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://ops.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://tlh.jinghuilouyu.cn

JS:   u instanceof User
来源：http://gjv.andypj.xyz

TS:   u instanceof User
来源：http://ssr.cashguo.top

Java: u instanceof User
来源：http://wmh.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ktb.fktsv.cn

Ruby: u.is_a?(User)
来源：http://wky.guowangkeji.top

C#:   u is User
来源：http://oao.yj20258888.top

[G14] 数据类 / record
来源：http://che.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nmq.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://puh.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://nac.redwolf501.top

TS:   type User = { name: string; age: number };
来源：http://eoi.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://ock.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://jhy.redwolf501.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rdv.sufxvd.cn

C#:   record User(string Name, int Age);
来源：http://vaz.yuxming.cn

[G15] 枚举
来源：http://efg.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pas.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rfl.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://erh.jyoumei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yqn.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://moz.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qee.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://ebu.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ony.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://qoo.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eyz.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://ckg.jinqigufen.top

JS:   Object.entries(obj)
来源：http://hik.xylfe.cn

TS:   Object.entries(obj)
来源：http://tgl.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xfl.hywenlv.cn


<!-- 参考信息 -->