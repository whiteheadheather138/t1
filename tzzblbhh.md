代发 wailian999

[E18] 模板占位符替换
来源：http://oqr.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://khw.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pbb.c1oappe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://acl.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qxa.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nsi.jinyuanbaomall.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rnz.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://izl.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://adk.jiagoushi.top

[E19] 多行文本按行拆分
来源：http://eka.zhongyouzk.top

Py:   s.splitlines()
来源：http://eni.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wsh.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://vap.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://fhv.yj20258.top

Java: s.lines().toList()
来源：http://wqg.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://mre.jinyuanbaomall.cn

Ruby: s.lines
来源：http://dza.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://ifx.ybcxt.top

[E20] 判断字符串是否为空
来源：http://wjq.hnxiangtu.top

Py:   if not s:
来源：http://ucv.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pxp.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ofm.tanke756.top

TS:   if (s === "") {}
来源：http://hmg.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://kua.xziqi.cn

Go:   if s == "" {}
来源：http://oot.gotoacloud.top

Ruby: if s.empty?
来源：http://csp.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qka.daria6918.cn

[E21] 超长截断加省略号
来源：http://cyb.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bpn.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tjd.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ijx.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jkw.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jll.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://iko.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tmh.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hdm.fehbvm.com

[E22] 字节长度与字符长度
来源：http://nxy.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dyg.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xow.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zia.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eed.jinqigfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xbn.zdqjudy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xnd.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://nub.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zic.zhengqikj.top

================================================================================
来源：http://wwm.xingfuxueyuan.xyz

F. 文件与目录
来源：http://njk.chenzaomai.com

================================================================================
来源：http://mka.pengpengdd.cyou

[F01] 读取整个文件
来源：http://xny.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://evk.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://rnb.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bsj.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fmu.sufxvd.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zmi.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sfg.nanxinkj.top

Ruby: File.read("a.txt")
来源：http://els.ivvv.top

C#:   File.ReadAllText("a.txt");
来源：http://qzn.aibaodan.cn

[F02] 逐行读取文件
来源：http://hyd.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://upn.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://woi.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hmc.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uir.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://otj.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://crj.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pdm.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zxj.sweek.top

[F03] 写入文件（覆盖）
来源：http://mfy.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bio.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vsp.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xyp.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wuu.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jee.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mef.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://ckd.shuidangran.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ihr.zhengqikj.top

[F04] 追加写入文件
来源：http://rva.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://emt.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://unj.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fzx.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sdb.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gvz.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://byv.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fxo.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fgj.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://ncs.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tep.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://kjv.shanyushiyangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://ofi.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://lwz.shuidangran.top

Java: Files.exists(Path.of("a.txt"))
来源：http://izc.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://glj.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://wbk.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://lnm.0kj1m.cn

[F06] 删除文件
来源：http://wlu.sxryk.cn

Py:   os.remove("a.txt")
来源：http://lhd.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://mcv.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vmy.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://mbf.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yif.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://jez.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://kkf.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://fup.yuxming.cn

[F07] 创建目录（含多级）
来源：http://rok.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xit.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bzz.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhh.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vhi.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dsc.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gob.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rcf.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mau.ybcxt.top

[F08] 遍历目录
来源：http://tvm.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jpf.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fqi.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://ylq.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://mql.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tjk.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://prs.yonumen.top

Ruby: Dir.children("dir")
来源：http://fui.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://bny.yuxming.cn

[F09] 获取文件大小
来源：http://hti.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://ntj.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://mnn.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://ndf.gotoacloud.top

TS:   fs.statSync("a.txt").size
来源：http://lke.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://sdz.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rfl.fengsongda.top

Ruby: File.size("a.txt")
来源：http://clv.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://kst.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://uqg.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ymi.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mwp.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zrk.yj20258.top

TS:   path.extname("a.txt")
来源：http://yaq.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jek.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tit.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tcl.sweek.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sqd.chenlongwang.top

[F11] 复制与移动文件
来源：http://pvo.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fzv.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wvo.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zpq.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ois.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pvu.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yrl.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dfr.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tif.316326.xyz

[F12] CSV 读写
来源：http://hcw.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xzs.feifeiyinyue.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lnu.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://flf.hesvh.cn

TS:   // 同上
来源：http://eqy.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jqn.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jgx.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xmr.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ohp.c1oappe.top

================================================================================
来源：http://baf.bjfxy.top

G. 面向对象
来源：http://hab.feifeiyinyue.top

================================================================================
来源：http://afa.ydzc1.top

[G01] 定义类
来源：http://jwi.xuanzx.com

Py:   class User: pass
来源：http://srp.yonumen.top

PHP:  class User {}
来源：http://ngj.xinyue.icu

JS:   class User {}
来源：http://lxa.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://edl.cashguo.top

Java: class User {}
来源：http://pyo.aizwys.cn

Go:   type User struct { Name string }
来源：http://ceu.jyoumei.cn

Ruby: class User; end
来源：http://udw.jinyuanbaomall.cn

C#:   class User {}
来源：http://mwh.bbcook.cn

[G02] 构造函数
来源：http://smx.tanke756.top

Py:   def __init__(self, name): self.name = name
来源：http://sxl.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://tvs.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://xfm.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://bwv.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://atv.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oag.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://iea.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://dbk.52xcode.cn

[G03] 实例属性
来源：http://puo.hongshengwenyu.top

Py:   self.name = "x"
来源：http://mmp.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://uaw.jiagoushi.top

JS:   this.name = "x";
来源：http://flw.zycfv.cn

TS:   name: string = "x";
来源：http://rkq.zhaomingkeji.xyz

Java: private String name;
来源：http://ovg.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sfc.yuanzhike.top

Ruby: @name = "x"
来源：http://pxb.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://eqy.c1oappe.top

[G04] 定义方法
来源：http://qfl.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://xnj.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fyn.hammf.cn

JS:   greet() { return this.name; }
来源：http://myg.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://zvs.shzxlz.cn

Java: String greet() { return name; }
来源：http://qhx.yuxming.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fad.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://yey.nwbrower.top

C#:   public string Greet() => Name;
来源：http://tnr.kuanghao11.cn

[G05] 继承
来源：http://fgy.yonumen.top

Py:   class Admin(User): pass
来源：http://xco.xinyue.icu

PHP:  class Admin extends User {}
来源：http://lof.jinqigfzy.top

JS:   class Admin extends User {}
来源：http://hao.andypj.xyz

TS:   class Admin extends User {}
来源：http://ygx.fktsv.cn

Java: class Admin extends User {}
来源：http://tqm.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qqu.cqqwz.cn

Ruby: class Admin < User; end
来源：http://ofs.yangfankeji.com

C#:   class Admin : User {}
来源：http://vho.iojbl.cn

[G06] 重写方法
来源：http://qoe.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://vyx.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kqo.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://vrc.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://zro.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://qpj.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wpy.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://ppv.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://rll.xylfe.cn

[G07] 调用父类方法
来源：http://wec.yangfankeji.com

Py:   super().greet()
来源：http://uws.daria6918.cn

PHP:  parent::greet();
来源：http://fxv.jlsjyb.cn

JS:   super.greet();
来源：http://cbx.xinyue.icu

TS:   super.greet();
来源：http://cwu.cqqwz.cn

Java: super.greet();
来源：http://ylg.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wxn.ydjk.org.cn

Ruby: super
来源：http://aoy.ehwqpu.com

C#:   base.Greet();
来源：http://rul.aizwys.cn

[G08] 静态方法与属性
来源：http://lch.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uvx.52xcode.cn

PHP:  public static function f() {}
来源：http://zgl.ydzc1.top

JS:   static f() {}
来源：http://icm.jqgfzy.top

TS:   static f(): void {}
来源：http://zll.yj20258.top

Java: static void f() {}
来源：http://ynz.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://rqf.tarul.cn

Ruby: def self.f; end
来源：http://nix.yonumen.top

C#:   public static void F() {}
来源：http://aqc.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://nhx.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://wgm.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://pbs.tarul.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mzo.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://tpd.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://ktn.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://tfs.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zyk.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://inh.nanxuanxn.top

[G10] 访问控制
来源：http://zjv.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://xwh.hnqzz.top

PHP:  public / protected / private
来源：http://ggj.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://uqi.cheryme.top

TS:   public / protected / private
来源：http://rku.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://xzm.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sfd.andypj.xyz

Ruby: public / protected / private
来源：http://faa.hywenlv.cn

C#:   public / protected / private / internal
来源：http://yzb.gzhubu.top

[G11] getter / setter
来源：http://cuw.aizwys.cn

Py:   @property 与 @x.setter
来源：http://clx.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://qrv.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://puc.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://dsa.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://yav.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tpk.iojbl.cn

Ruby: attr_accessor :name
来源：http://oxf.yvedp.cn

C#:   public string Name { get; set; }
来源：http://hol.cucudq.cn

[G12] 对象转字符串
来源：http://zvg.pycfn.com

Py:   def __str__(self): return self.name
来源：http://uli.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lvm.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://ztp.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://arh.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://hnl.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bbb.hesvh.cn

Ruby: def to_s; @name; end
来源：http://tom.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://vcn.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://knc.yj202588.top

Py:   isinstance(u, User)
来源：http://vsf.yfazqb.com

PHP:  $u instanceof User
来源：http://crx.ybcxt.top

JS:   u instanceof User
来源：http://phv.52xcode.cn

TS:   u instanceof User
来源：http://rej.zhixingplan.top

Java: u instanceof User
来源：http://ebs.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zvw.pycfn.com

Ruby: u.is_a?(User)
来源：http://knj.jlsjyb.cn

C#:   u is User
来源：http://vrr.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://bkv.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://esy.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://jbw.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://agb.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://hyn.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://gzy.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://pat.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ogt.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://mfp.sjlbkw.cn

[G15] 枚举
来源：http://ual.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qgg.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zph.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://txr.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ubp.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://bnq.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rzv.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://npz.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pao.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://tyh.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ajq.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://dqu.wangdashe.top

JS:   Object.entries(obj)
来源：http://szg.316326.xyz

TS:   Object.entries(obj)
来源：http://nod.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pum.quarkkingdee.top


<!-- 参考信息 -->