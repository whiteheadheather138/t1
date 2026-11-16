代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kgt.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tzg.zdqjudy.top

TS:   if (s === "") {}
来源：http://bnr.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://ukg.zhengqikj.top

Go:   if s == "" {}
来源：http://dzq.sysykeji.top

Ruby: if s.empty?
来源：http://vhq.xinyue.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iop.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://mya.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bki.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rvg.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ync.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynu.yangfankeji.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://muw.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://cgd.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gjb.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wgn.yuxming.cn

[E22] 字节长度与字符长度
来源：http://wgf.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hxs.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ico.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sli.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vfk.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zeb.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vxz.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://jea.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vxh.hcnkem.com

================================================================================
来源：http://rpm.ppjwa.cn

F. 文件与目录
来源：http://ocu.kuanghao11.cn

================================================================================
来源：http://sar.zycfv.cn

[F01] 读取整个文件
来源：http://bel.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vxk.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://cvk.xziqi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ehn.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fat.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://sjc.shzxlz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://efe.daxiang520.top

Ruby: File.read("a.txt")
来源：http://lae.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://tzc.dashuyun.cn

[F02] 逐行读取文件
来源：http://dzu.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pxl.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fth.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xig.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kbc.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pdq.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://exx.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bgg.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uva.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://srm.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aho.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://trc.ywan-chungtsiang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://smt.xziqi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lfk.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://asc.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vko.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://upb.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://krh.kuanghao11.cn

[F04] 追加写入文件
来源：http://lkb.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ufv.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tog.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hhf.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ngu.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nll.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uui.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jlt.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mqo.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://yrz.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ges.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://raw.ivvv.top

JS:   fs.existsSync("a.txt")
来源：http://jtg.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://tbg.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bzr.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aop.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://jih.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://hlq.wangdashe.top

[F06] 删除文件
来源：http://dgi.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://wcm.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://rpq.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tan.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ycu.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mfq.ybcxt.top

Go:   os.Remove("a.txt")
来源：http://cdh.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://wnn.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://npz.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://lhs.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://glk.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sxm.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vsm.yongpay.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ctd.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tzi.wangshuangyany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ehv.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kbm.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eeb.hammf.cn

[F08] 遍历目录
来源：http://uhh.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yxa.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aup.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://rgj.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://ghf.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ktv.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kkd.316326.xyz

Ruby: Dir.children("dir")
来源：http://lfr.chenlongwang.top

C#:   Directory.GetFiles("dir")
来源：http://nmu.fehbvm.com

[F09] 获取文件大小
来源：http://fto.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://qxq.yj202588.top

PHP:  filesize("a.txt");
来源：http://pze.ppjwa.cn

JS:   fs.statSync("a.txt").size
来源：http://glh.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://ynn.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://pjg.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kef.nwbrower.top

Ruby: File.size("a.txt")
来源：http://htm.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://ptm.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://paf.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://efm.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aic.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eiu.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://kjp.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://llt.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fym.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yku.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zgk.aizwys.cn

[F11] 复制与移动文件
来源：http://cmx.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rqb.jinqigfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rtw.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rwt.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hla.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sfc.chenzaomai.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gcu.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uky.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gef.hammf.cn

[F12] CSV 读写
来源：http://asr.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bhc.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jhk.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fzy.tarul.cn

TS:   // 同上
来源：http://tdc.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zyg.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nli.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kht.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vhq.sufxvd.cn

================================================================================
来源：http://qgu.smart0.xyz

G. 面向对象
来源：http://kik.jinghuilouyu.cn

================================================================================
来源：http://pcr.jiagoushi.top

[G01] 定义类
来源：http://dfp.sysykeji.top

Py:   class User: pass
来源：http://odc.fengsongda.top

PHP:  class User {}
来源：http://vgn.gogol.net.cn

JS:   class User {}
来源：http://mgb.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://wfu.nwbrower.top

Java: class User {}
来源：http://iqn.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://vpa.redwolf501.top

Ruby: class User; end
来源：http://rhq.iojbl.cn

C#:   class User {}
来源：http://gut.jinqigfzy.top

[G02] 构造函数
来源：http://tgd.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://szh.guowangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://pud.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://hjw.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://eun.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://rce.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://htc.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://kjl.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://huu.jlsjyb.cn

[G03] 实例属性
来源：http://sxh.wangshuangyany.cn

Py:   self.name = "x"
来源：http://gdu.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://xyr.ydjk.org.cn

JS:   this.name = "x";
来源：http://btf.zhoulong.xyz

TS:   name: string = "x";
来源：http://okl.shanyushiyangtech.top

Java: private String name;
来源：http://czs.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xsu.wangshuangyany.cn

Ruby: @name = "x"
来源：http://qyw.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://shh.andypj.xyz

[G04] 定义方法
来源：http://ebi.jianghu66.top

Py:   def greet(self): return self.name
来源：http://vqh.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yxk.andypj.xyz

JS:   greet() { return this.name; }
来源：http://gtg.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://fct.ybcxt.top

Java: String greet() { return name; }
来源：http://hqq.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://img.52xcode.cn

Ruby: def greet; @name; end
来源：http://lkh.wangdashe.top

C#:   public string Greet() => Name;
来源：http://zws.zhoulong.xyz

[G05] 继承
来源：http://wcu.jinqigufen.top

Py:   class Admin(User): pass
来源：http://jca.cashguo.top

PHP:  class Admin extends User {}
来源：http://glq.meibo888.top

JS:   class Admin extends User {}
来源：http://yvn.tianlin.xyz

TS:   class Admin extends User {}
来源：http://vmi.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://oqv.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sje.aizwys.cn

Ruby: class Admin < User; end
来源：http://evk.zdqjudy.top

C#:   class Admin : User {}
来源：http://qkt.daxiang520.top

[G06] 重写方法
来源：http://fho.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://hxl.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://xst.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://mhj.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://yeg.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://rhc.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ztb.birdmap.top

Ruby: def greet; "admin"; end
来源：http://ddv.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://ziw.sufxvd.cn

[G07] 调用父类方法
来源：http://dtl.yfazqb.com

Py:   super().greet()
来源：http://mcn.0kj1m.cn

PHP:  parent::greet();
来源：http://vyd.yj202588.top

JS:   super.greet();
来源：http://zhk.ywan-chungtsiang.top

TS:   super.greet();
来源：http://usu.epnwcf.com

Java: super.greet();
来源：http://zbv.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ytu.hnqzz.top

Ruby: super
来源：http://wkf.aizwys.cn

C#:   base.Greet();
来源：http://aym.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://ddi.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aju.kuanghao11.cn

PHP:  public static function f() {}
来源：http://euh.yfazqb.com

JS:   static f() {}
来源：http://vhz.cucudq.cn

TS:   static f(): void {}
来源：http://fyq.yuanzhike.top

Java: static void f() {}
来源：http://ylb.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qlj.cashguo.top

Ruby: def self.f; end
来源：http://lym.nwbrower.top

C#:   public static void F() {}
来源：http://jwb.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://rib.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://raj.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://zuw.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mcq.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://xgi.fengsongda.top

Java: interface Shape { double area(); }
来源：http://dmu.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://npv.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://upj.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://ivf.hfpthk.cn

[G10] 访问控制
来源：http://wdz.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://lkq.zhongyouzk.top

PHP:  public / protected / private
来源：http://ldw.yuxming.cn

JS:   #private 字段；其余公开
来源：http://wju.guowangkeji.top

TS:   public / protected / private
来源：http://ijx.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://gyw.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://llt.vqdsnc.cn

Ruby: public / protected / private
来源：http://zjh.yuanzhike.top

C#:   public / protected / private / internal
来源：http://pfx.ppjwa.cn

[G11] getter / setter
来源：http://lhi.uphjek.com

Py:   @property 与 @x.setter
来源：http://evf.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://iow.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://oxp.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://hbd.redwolf501.top

Java: public String getName() { return name; }
来源：http://mdb.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fyd.fehbvm.com

Ruby: attr_accessor :name
来源：http://xsa.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://izx.sysykeji.top

[G12] 对象转字符串
来源：http://vcn.yj20258.top

Py:   def __str__(self): return self.name
来源：http://ams.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://byt.birdmap.top

JS:   toString() { return this.name; }
来源：http://gyg.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://agi.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://hyi.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://ceq.sxryk.cn

Ruby: def to_s; @name; end
来源：http://apr.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://cif.guowangkeji.top

[G13] 判断对象类型
来源：http://bzo.tian-w.cn

Py:   isinstance(u, User)
来源：http://nkr.chenlongwang.top

PHP:  $u instanceof User
来源：http://vxw.aizwys.cn

JS:   u instanceof User
来源：http://xgd.gzhubu.top

TS:   u instanceof User
来源：http://oty.zhaomingkeji.xyz

Java: u instanceof User
来源：http://yqu.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sla.andypj.xyz

Ruby: u.is_a?(User)
来源：http://opj.shzxlz.cn

C#:   u is User
来源：http://sfk.shuidangran.top

[G14] 数据类 / record
来源：http://ryj.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wbm.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://bmc.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://xxj.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://ctb.jianghu66.top

Java: record User(String name, int age) {}
来源：http://noz.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://kmj.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oer.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://ibu.yuxming.cn

[G15] 枚举
来源：http://xuc.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://krz.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wki.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yqm.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://epk.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://zun.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://woj.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://efd.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oaq.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://twa.snrcjt.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dnd.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://faj.mhx1999.top

JS:   Object.entries(obj)
来源：http://hiu.uphjek.com

TS:   Object.entries(obj)
来源：http://dlk.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mod.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mgv.redwolf501.top

Ruby: obj.instance_variables
来源：http://xja.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://dai.xylfe.cn

================================================================================
来源：http://rex.cheryme.top

H. 异常与错误处理
来源：http://egf.jlsjyb.cn

================================================================================
来源：http://ffb.daxiang520.top

[H01] try / catch 基础
来源：http://wwa.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pcx.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://quq.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ryb.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jwi.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://txt.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://siq.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bje.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dal.ydzc1.top

[H02] finally / ensure 收尾
来源：http://pix.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://svf.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wce.jinqigufen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jmp.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mkh.epnwcf.com


<!-- 参考信息 -->