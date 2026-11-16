代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hid.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://mzj.wangshuangyany.cn

Py:   s.splitlines()
来源：http://vad.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wzy.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://lph.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://fkw.daria6918.cn

Java: s.lines().toList()
来源：http://xro.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://fsv.andypj.xyz

Ruby: s.lines
来源：http://aga.jiagoushi.top

C#:   s.Split('\n')
来源：http://oej.shanyushiyangkeji.top

[E20] 判断字符串是否为空
来源：http://dac.fzhhl.top

Py:   if not s:
来源：http://smp.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yrf.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nwb.redwolf501.top

TS:   if (s === "") {}
来源：http://sfh.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://uif.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://ogk.hesvh.cn

Ruby: if s.empty?
来源：http://qqr.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jaa.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://wds.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ieg.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sij.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://whr.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mkw.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sle.jyoumei.cn

Go:   // 按 rune 判断长度后截断
来源：http://hnt.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pom.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cvf.yuxming.cn

[E22] 字节长度与字符长度
来源：http://fpv.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cdc.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://laj.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pxg.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aot.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rld.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://umd.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://qsf.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sij.jqgfzy.top

================================================================================
来源：http://dsl.xuetiantiany.cn

F. 文件与目录
来源：http://fsr.jqgfzy.top

================================================================================
来源：http://xuc.dianchejie.cn

[F01] 读取整个文件
来源：http://uhz.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jbc.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://rpg.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zwn.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gwt.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eft.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://awx.xziqi.cn

Ruby: File.read("a.txt")
来源：http://tee.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://kok.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://bzl.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zva.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jsn.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://joo.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xnv.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hcx.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rat.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lqt.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kri.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://hjm.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ypf.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://nst.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eso.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ugw.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xvj.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ard.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://hug.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qyz.xuanzx.com

[F04] 追加写入文件
来源：http://lrf.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eoo.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fvj.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vld.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dna.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eua.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cpg.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://olu.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qeb.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://gim.yvedp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jjg.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://awj.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://qai.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://xzi.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://unu.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nwy.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://fgt.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://zpu.zhongyouzk.top

[F06] 删除文件
来源：http://ufh.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://xox.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://jqb.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://qyt.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ngh.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pnq.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://psq.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://pfz.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://ube.aizwys.cn

[F07] 创建目录（含多级）
来源：http://cee.jiagoushi.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uoa.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jlc.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mha.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uig.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rtt.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kcp.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cxg.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://frs.zhiwuduotai.top

[F08] 遍历目录
来源：http://vyz.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nii.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xsz.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://udr.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://pox.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rgl.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jbm.fengsongda.top

Ruby: Dir.children("dir")
来源：http://vth.ehwqpu.com

C#:   Directory.GetFiles("dir")
来源：http://fta.gotoacloud.top

[F09] 获取文件大小
来源：http://csj.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://dpr.nwbrower.top

PHP:  filesize("a.txt");
来源：http://tdj.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://oct.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://whn.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ljv.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cgt.tian-w.cn

Ruby: File.size("a.txt")
来源：http://voh.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://veq.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://ofu.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eqz.yanxiufei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bur.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dvq.fengsongda.top

TS:   path.extname("a.txt")
来源：http://oap.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gqn.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pwc.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ozg.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sjd.guowangkeji.top

[F11] 复制与移动文件
来源：http://vfw.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://owe.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tju.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jmo.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zxv.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jui.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yrl.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vbo.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vtz.nwbrower.top

[F12] CSV 读写
来源：http://kba.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rjn.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lkc.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ghp.sufxvd.cn

TS:   // 同上
来源：http://cbm.hfpthk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tji.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vkd.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ooz.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ztj.quarkkingdee.top

================================================================================
来源：http://cjj.zdqjudy.top

G. 面向对象
来源：http://rbi.sxryk.cn

================================================================================
来源：http://bvu.ydjk.org.cn

[G01] 定义类
来源：http://zeq.aibaodan.cn

Py:   class User: pass
来源：http://ukk.zhoulong.xyz

PHP:  class User {}
来源：http://gku.nanxinkj.top

JS:   class User {}
来源：http://xtp.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://gah.bjfxy.top

Java: class User {}
来源：http://yew.zdqjudy.top

Go:   type User struct { Name string }
来源：http://sod.zhengqikj.top

Ruby: class User; end
来源：http://axe.fehbvm.com

C#:   class User {}
来源：http://mqs.ydzc1.top

[G02] 构造函数
来源：http://vsj.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://etl.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://eyz.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://ebh.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://qhk.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://bwx.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://guv.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://jov.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://pkl.fzhhl.top

[G03] 实例属性
来源：http://nej.ybcxt.top

Py:   self.name = "x"
来源：http://yvm.yangfankeji.com

PHP:  public string $name = "x";
来源：http://rbb.feifeiyinyue.top

JS:   this.name = "x";
来源：http://idx.zhongyouzk.top

TS:   name: string = "x";
来源：http://uyr.nwbrower.top

Java: private String name;
来源：http://kpp.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wys.vqdsnc.cn

Ruby: @name = "x"
来源：http://nbl.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://lya.kuanghao11.cn

[G04] 定义方法
来源：http://zly.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://bcw.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://soa.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://jhc.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://ubu.c1oappe.top

Java: String greet() { return name; }
来源：http://sst.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mdh.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://vfo.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://mqe.jyoumei.cn

[G05] 继承
来源：http://npu.hnqzz.top

Py:   class Admin(User): pass
来源：http://okk.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://gpl.birdmap.top

JS:   class Admin extends User {}
来源：http://tri.jinghuilouyu.cn

TS:   class Admin extends User {}
来源：http://sxg.andypj.xyz

Java: class Admin extends User {}
来源：http://aty.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qer.cqqwz.cn

Ruby: class Admin < User; end
来源：http://oxe.zhengqikj.top

C#:   class Admin : User {}
来源：http://dwb.bbcook.cn

[G06] 重写方法
来源：http://lqc.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://wvh.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://arh.cashguo.top

JS:   greet() { return "admin"; }
来源：http://rsv.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://pmy.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://wqa.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://win.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://fyb.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://qcf.xuetiantiany.cn

[G07] 调用父类方法
来源：http://zpc.zdbjq.cn

Py:   super().greet()
来源：http://zat.nanxinkj.top

PHP:  parent::greet();
来源：http://xcs.zhaomingkeji.xyz

JS:   super.greet();
来源：http://tgf.ywan-chungtsiang.top

TS:   super.greet();
来源：http://rqr.wangdashe.top

Java: super.greet();
来源：http://ttx.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nts.gzhubu.top

Ruby: super
来源：http://lky.zdbjq.cn

C#:   base.Greet();
来源：http://une.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://psn.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xci.xingfuxueyuan.xyz

PHP:  public static function f() {}
来源：http://lbj.zhijiandao.cn

JS:   static f() {}
来源：http://vma.zhijiandao.cn

TS:   static f(): void {}
来源：http://vdl.jinqigufen.top

Java: static void f() {}
来源：http://lsx.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wqs.epnwcf.com

Ruby: def self.f; end
来源：http://tjv.bbcook.cn

C#:   public static void F() {}
来源：http://una.pycfn.com

[G09] 接口 / 抽象类
来源：http://ynr.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://pnu.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://zxg.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://frh.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://yjz.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://ero.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://tlh.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xfv.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://knq.jinqigfzy.top

[G10] 访问控制
来源：http://rpb.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://yzm.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://wwj.cucudq.cn

JS:   #private 字段；其余公开
来源：http://lzt.wangshuangyany.cn

TS:   public / protected / private
来源：http://grr.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://lvd.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gmq.9152youxi.cn

Ruby: public / protected / private
来源：http://dby.chenzaomai.com

C#:   public / protected / private / internal
来源：http://zbe.sxryk.cn

[G11] getter / setter
来源：http://xqz.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://eoc.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ijq.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://mlw.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://icp.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://qmy.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jbg.guowangkeji.top

Ruby: attr_accessor :name
来源：http://wxx.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://pyh.sxryk.cn

[G12] 对象转字符串
来源：http://kbt.tarul.cn

Py:   def __str__(self): return self.name
来源：http://vuz.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://glp.aizwys.cn

JS:   toString() { return this.name; }
来源：http://pfj.0kj1m.cn

TS:   toString(): string { return this.name; }
来源：http://fza.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://hvr.c1oappe.top

Go:   func (u User) String() string { return u.Name }
来源：http://nxo.tarul.cn

Ruby: def to_s; @name; end
来源：http://zxg.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://wmp.zhoulong.xyz

[G13] 判断对象类型
来源：http://kfx.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://rkx.aibaodan.cn

PHP:  $u instanceof User
来源：http://edz.jinqigufen.top

JS:   u instanceof User
来源：http://ciy.zdqjudy.top

TS:   u instanceof User
来源：http://hri.gaohongyu789.top

Java: u instanceof User
来源：http://lrh.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xry.shuidangran.top

Ruby: u.is_a?(User)
来源：http://rwz.daria6918.cn

C#:   u is User
来源：http://jud.snrcjt.cn

[G14] 数据类 / record
来源：http://zjg.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iep.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://tnb.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://zix.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://cal.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://heg.cashguo.top

Go:   type User struct { Name string; Age int }
来源：http://ihe.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vhc.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://qgf.hammf.cn

[G15] 枚举
来源：http://qvs.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lig.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lzx.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fxw.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hjn.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://aut.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gdb.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://amf.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kqd.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://mlr.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bac.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://xcu.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://tsi.sysykeji.top

TS:   Object.entries(obj)
来源：http://exj.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iyz.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://jiq.jiagoushi.top

Ruby: obj.instance_variables
来源：http://ivm.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://kax.sysykeji.top

================================================================================
来源：http://ivt.mhx1999.top

H. 异常与错误处理
来源：http://khu.xuanzx.com

================================================================================
来源：http://tgq.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://nfa.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aoy.xuanzx.com


<!-- 参考信息 -->