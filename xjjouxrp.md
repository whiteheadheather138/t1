代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://nnu.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://gbt.bjfxy.top

Java: s.lines().toList()
来源：http://hks.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://pvt.hfpthk.cn

Ruby: s.lines
来源：http://xpc.guowangkeji.top

C#:   s.Split('\n')
来源：http://zoq.epnwcf.com

[E20] 判断字符串是否为空
来源：http://vmt.chenjidiqi.icu

Py:   if not s:
来源：http://tgq.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gtg.shuidangran.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sba.yuxming.cn

TS:   if (s === "") {}
来源：http://mca.hnxiangtu.top

Java: if (s.isEmpty()) {}
来源：http://ggu.cashguo.top

Go:   if s == "" {}
来源：http://fes.jiagoushi.top

Ruby: if s.empty?
来源：http://lml.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zjj.aibaodan.cn

[E21] 超长截断加省略号
来源：http://cei.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://piv.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ohq.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mla.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yba.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cyl.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://ada.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://igk.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ama.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://iko.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qxj.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vgw.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://voh.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hgy.yj20258888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://prp.sweek.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oiu.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://yly.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nns.epnwcf.com

================================================================================
来源：http://fmy.smart0.xyz

F. 文件与目录
来源：http://nbr.gogol.net.cn

================================================================================
来源：http://qea.chenzaomai.com

[F01] 读取整个文件
来源：http://vcn.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xip.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://ord.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mlx.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://egk.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dzf.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://myg.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://oey.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://cki.cucudq.cn

[F02] 逐行读取文件
来源：http://bax.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xha.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tak.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jfk.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ygl.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qgh.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ulh.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gmw.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cjo.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://kek.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wsx.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aqb.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lst.xuanzx.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://djo.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tjq.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oba.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://hbe.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qzv.yanxiufei.cn

[F04] 追加写入文件
来源：http://ith.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fqd.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://erp.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rzs.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwp.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zej.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sfn.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wrf.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://scm.shzxlz.cn

[F05] 判断文件或目录是否存在
来源：http://vqh.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jvv.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://uck.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://unx.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://jsl.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xwh.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dhe.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://hvj.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://nfn.gaohongyu789.top

[F06] 删除文件
来源：http://cmg.ybcxt.top

Py:   os.remove("a.txt")
来源：http://zed.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://qou.pycfn.com

JS:   fs.unlinkSync("a.txt")
来源：http://hod.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://jrk.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qxy.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://euc.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://jdj.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://jqo.c1oappe.top

[F07] 创建目录（含多级）
来源：http://suh.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mih.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vyd.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kus.hfpthk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tmj.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nst.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tpc.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pkv.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cct.nanxuanxn.top

[F08] 遍历目录
来源：http://plh.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vhl.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gtr.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://wtr.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://knm.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bum.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tkd.hesvh.cn

Ruby: Dir.children("dir")
来源：http://qvo.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://uqf.nanxinkj.top

[F09] 获取文件大小
来源：http://ldh.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://pvk.chenlongwang.top

PHP:  filesize("a.txt");
来源：http://ajq.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://wnq.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://bnk.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://grs.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ggu.yfazqb.com

Ruby: File.size("a.txt")
来源：http://zbx.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://jta.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://nxc.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fdy.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ueb.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lwf.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://qsh.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cfz.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ypt.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cna.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://die.dianchejie.cn

[F11] 复制与移动文件
来源：http://iiq.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dke.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://soa.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gbe.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://glg.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lep.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dtz.vehdjk.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vgo.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mvz.zhengqikj.top

[F12] CSV 读写
来源：http://ikb.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nfj.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eux.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sei.gzhubu.top

TS:   // 同上
来源：http://iyl.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ykm.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ifl.cqqwz.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lyo.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xtm.vqdsnc.cn

================================================================================
来源：http://lne.bbcook.cn

G. 面向对象
来源：http://oki.epnwcf.com

================================================================================
来源：http://vta.jqgufenzy.top

[G01] 定义类
来源：http://eam.xingfuxueyuan.xyz

Py:   class User: pass
来源：http://mug.ybcxt.top

PHP:  class User {}
来源：http://zxa.yj20258.top

JS:   class User {}
来源：http://fsa.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://nfd.zhoulong.xyz

Java: class User {}
来源：http://zto.chenjidiqi.icu

Go:   type User struct { Name string }
来源：http://cqt.0kj1m.cn

Ruby: class User; end
来源：http://hyg.xuanzx.com

C#:   class User {}
来源：http://xgq.shzxlz.cn

[G02] 构造函数
来源：http://rop.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://jld.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://icx.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://lfz.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://lbg.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://omd.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wmk.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://qei.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://aze.0kj1m.cn

[G03] 实例属性
来源：http://kft.yvedp.cn

Py:   self.name = "x"
来源：http://qjb.sufxvd.cn

PHP:  public string $name = "x";
来源：http://vgi.ppjwa.cn

JS:   this.name = "x";
来源：http://off.nanxuanxn.top

TS:   name: string = "x";
来源：http://xhl.wangdashe.top

Java: private String name;
来源：http://ite.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ofh.ybcxt.top

Ruby: @name = "x"
来源：http://nto.guannengcc.top

C#:   public string Name { get; set; } = "x";
来源：http://onv.nanxuanxn.top

[G04] 定义方法
来源：http://pbn.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://uoh.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ars.yj202588.top

JS:   greet() { return this.name; }
来源：http://ptr.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://keq.nanxuanxn.top

Java: String greet() { return name; }
来源：http://ycj.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gww.xuanzx.com

Ruby: def greet; @name; end
来源：http://gxv.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://ssm.daxiang520.top

[G05] 继承
来源：http://gwl.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://mzz.wangshuangyany.cn

PHP:  class Admin extends User {}
来源：http://ros.nwbrower.top

JS:   class Admin extends User {}
来源：http://mlm.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://bys.hywenlv.cn

Java: class Admin extends User {}
来源：http://oon.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gvz.chenlongwang.top

Ruby: class Admin < User; end
来源：http://cal.hysaishi.cn

C#:   class Admin : User {}
来源：http://qni.daxiang520.top

[G06] 重写方法
来源：http://dck.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://tdp.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xoh.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://bky.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://oyu.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://bax.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jai.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://yff.haohaochexian.top

C#:   public override string Greet() => "admin";
来源：http://tbh.jinqigufen.top

[G07] 调用父类方法
来源：http://djs.ybcxt.top

Py:   super().greet()
来源：http://zwt.kuanghao11.cn

PHP:  parent::greet();
来源：http://wax.ctjpmb.com

JS:   super.greet();
来源：http://zmk.yvedp.cn

TS:   super.greet();
来源：http://sps.cheryme.top

Java: super.greet();
来源：http://uia.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uyn.cheryme.top

Ruby: super
来源：http://uvf.nanxinkj.top

C#:   base.Greet();
来源：http://njq.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://tne.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rbu.guannengcc.top

PHP:  public static function f() {}
来源：http://lpd.dashuyun.cn

JS:   static f() {}
来源：http://eta.snrcjt.cn

TS:   static f(): void {}
来源：http://zzv.snrcjt.cn

Java: static void f() {}
来源：http://dbr.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zfo.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://nmu.yfazqb.com

C#:   public static void F() {}
来源：http://abx.pycfn.com

[G09] 接口 / 抽象类
来源：http://uel.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://gec.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wih.ivvv.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sct.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://agn.havefunace.top

Java: interface Shape { double area(); }
来源：http://dkg.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://tkr.quarkkingdee.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rdy.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://ygg.snrcjt.cn

[G10] 访问控制
来源：http://wcy.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://frz.zhoulong.xyz

PHP:  public / protected / private
来源：http://vfk.xylfe.cn

JS:   #private 字段；其余公开
来源：http://qri.yuanzhike.top

TS:   public / protected / private
来源：http://msn.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://pep.jinqigfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rpw.chenzaomai.com

Ruby: public / protected / private
来源：http://kvy.zhengqikj.top

C#:   public / protected / private / internal
来源：http://gou.sufxvd.cn

[G11] getter / setter
来源：http://esb.cashguo.top

Py:   @property 与 @x.setter
来源：http://bsv.aibaodan.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dwd.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://dms.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://rot.pengpengdd.cyou

Java: public String getName() { return name; }
来源：http://sub.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nxe.c1oappe.top

Ruby: attr_accessor :name
来源：http://fpw.ivvv.top

C#:   public string Name { get; set; }
来源：http://rby.yj20258888.top

[G12] 对象转字符串
来源：http://pmq.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://prx.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yiv.tian-w.cn

JS:   toString() { return this.name; }
来源：http://asv.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://azq.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://rbg.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rlm.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://bgs.cashguo.top

C#:   public override string ToString() => Name;
来源：http://vrh.jyoumei.cn

[G13] 判断对象类型
来源：http://seb.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://wfu.smart0.xyz

PHP:  $u instanceof User
来源：http://cby.jqgfzy.top

JS:   u instanceof User
来源：http://mib.zhengqikj.top

TS:   u instanceof User
来源：http://jnu.haohaochexian.top

Java: u instanceof User
来源：http://apq.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://bdt.shuidangran.top

Ruby: u.is_a?(User)
来源：http://ypm.chenzaomai.com

C#:   u is User
来源：http://mkt.uphjek.com

[G14] 数据类 / record
来源：http://eyb.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wbb.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://dqz.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ofc.meibo888.top

TS:   type User = { name: string; age: number };
来源：http://qap.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://wvo.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://qcc.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xnr.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://rnu.cdnleiting.top

[G15] 枚举
来源：http://ric.mhx1999.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kwg.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://efn.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zom.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xyr.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://usj.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wjf.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://ptf.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://swn.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://efc.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://afe.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://arj.cheryme.top

JS:   Object.entries(obj)
来源：http://ekl.zdbjq.cn

TS:   Object.entries(obj)
来源：http://qzi.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qha.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://edp.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://wrq.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://bbi.chenzaomai.com

================================================================================
来源：http://unm.jinqigufen.top

H. 异常与错误处理
来源：http://hwm.ppjwa.cn

================================================================================
来源：http://zgv.ydzc1.top

[H01] try / catch 基础
来源：http://kep.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xlk.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ttb.cucudq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mkc.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ghn.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zbd.hcnkem.com


<!-- 参考信息 -->