代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sky.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ldw.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zwg.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ajh.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cxb.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://tjm.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yek.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://myr.sxryk.cn

[E22] 字节长度与字符长度
来源：http://xhr.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://syi.yj20258.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sac.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sek.zhongyouzk.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qxp.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ree.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fng.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://plm.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lis.hnxiangtu.top

================================================================================
来源：http://wbu.jqgfzy.top

F. 文件与目录
来源：http://zzc.yj202588.top

================================================================================
来源：http://xmo.jiagoushi.top

[F01] 读取整个文件
来源：http://eit.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ocb.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://onh.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://snm.kuanghao11.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gmx.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xkn.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vli.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://rpc.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://nju.hcnkem.com

[F02] 逐行读取文件
来源：http://lpm.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tmy.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nzy.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ich.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qcc.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://itu.yj202588.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ifg.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jqh.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gpf.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://rvs.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mlc.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cng.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfv.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ldi.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qtf.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tsl.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://tfk.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uyp.yj202588.top

[F04] 追加写入文件
来源：http://uwg.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jve.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hrj.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hwl.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vlc.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eyv.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oii.gzhubu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ogt.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eav.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://okz.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bvd.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://oco.yangfankeji.com

JS:   fs.existsSync("a.txt")
来源：http://okn.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://tnm.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://iop.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ges.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://tkc.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://fig.fengsongda.top

[F06] 删除文件
来源：http://fkc.bjfxy.top

Py:   os.remove("a.txt")
来源：http://run.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://uky.sufxvd.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nad.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gty.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ojy.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://vtz.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://qcc.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://ppg.tian-w.cn

[F07] 创建目录（含多级）
来源：http://ilx.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ztg.snrcjt.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dto.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ngi.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxb.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jps.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kwp.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://izg.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mum.yj202588.top

[F08] 遍历目录
来源：http://dny.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fzn.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jam.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://lpk.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://pqt.guowangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ejb.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xam.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://mwn.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://yrd.fengsongda.top

[F09] 获取文件大小
来源：http://foq.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://fqr.bbcook.cn

PHP:  filesize("a.txt");
来源：http://yaq.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://rgp.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://kzv.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vdp.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cav.cdnleiting.top

Ruby: File.size("a.txt")
来源：http://ikv.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://pug.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://qos.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gue.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fcm.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bep.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://ikf.mhx1999.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qii.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ddm.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tmr.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kma.xylfe.cn

[F11] 复制与移动文件
来源：http://ypw.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mmc.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://whr.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fsc.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rmz.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qic.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cys.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ats.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xts.xylfe.cn

[F12] CSV 读写
来源：http://xhl.jqgfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bmv.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kqv.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://azq.yj20258.top

TS:   // 同上
来源：http://czd.sweek.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hnz.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wig.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bbu.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ndk.shanyushiyangtech.top

================================================================================
来源：http://mfc.mhx1999.top

G. 面向对象
来源：http://dkf.daria6918.cn

================================================================================
来源：http://ijk.hcnkem.com

[G01] 定义类
来源：http://jha.chenjidiqi.icu

Py:   class User: pass
来源：http://bqv.hnxiangtu.top

PHP:  class User {}
来源：http://jua.gotoacloud.top

JS:   class User {}
来源：http://out.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://mae.yj20258888.top

Java: class User {}
来源：http://yew.dashuyun.cn

Go:   type User struct { Name string }
来源：http://xaz.hfpthk.cn

Ruby: class User; end
来源：http://udb.mhx1999.top

C#:   class User {}
来源：http://krs.fzhhl.top

[G02] 构造函数
来源：http://egk.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://shk.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://noy.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://pqs.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://kxs.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://lai.hesvh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zmh.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://lpb.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://wdf.havefunace.top

[G03] 实例属性
来源：http://qha.gzhubu.top

Py:   self.name = "x"
来源：http://fqd.chenlongwang.top

PHP:  public string $name = "x";
来源：http://yue.fengsongda.top

JS:   this.name = "x";
来源：http://frg.zdqjudy.top

TS:   name: string = "x";
来源：http://wrm.tian-w.cn

Java: private String name;
来源：http://snd.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oai.yj20258.top

Ruby: @name = "x"
来源：http://jcu.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://xwc.jlsjyb.cn

[G04] 定义方法
来源：http://zkc.hesvh.cn

Py:   def greet(self): return self.name
来源：http://shn.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://chx.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://gtp.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://qie.jianghu66.top

Java: String greet() { return name; }
来源：http://ftm.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kcz.fzhhl.top

Ruby: def greet; @name; end
来源：http://yna.yuxming.cn

C#:   public string Greet() => Name;
来源：http://vyw.yuanzhike.top

[G05] 继承
来源：http://sjs.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://onl.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://xbh.yongpay.top

JS:   class Admin extends User {}
来源：http://lyw.ctjpmb.com

TS:   class Admin extends User {}
来源：http://kqi.meibo888.top

Java: class Admin extends User {}
来源：http://wcb.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://soq.ivvv.top

Ruby: class Admin < User; end
来源：http://plv.gzhubu.top

C#:   class Admin : User {}
来源：http://ppd.fzhhl.top

[G06] 重写方法
来源：http://jjn.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://syp.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vmy.yangfankeji.com

JS:   greet() { return "admin"; }
来源：http://fbn.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://bgs.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://kzl.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cxt.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://boh.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://wqc.tianlin.xyz

[G07] 调用父类方法
来源：http://egf.quarkkingdee.top

Py:   super().greet()
来源：http://itc.cucudq.cn

PHP:  parent::greet();
来源：http://dqn.ppjwa.cn

JS:   super.greet();
来源：http://fui.fehbvm.com

TS:   super.greet();
来源：http://ilk.snrcjt.cn

Java: super.greet();
来源：http://obq.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://afq.fktsv.cn

Ruby: super
来源：http://tjf.hesvh.cn

C#:   base.Greet();
来源：http://cmz.hnqzz.top

[G08] 静态方法与属性
来源：http://zpe.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zcb.tianlin.xyz

PHP:  public static function f() {}
来源：http://hbu.guowangkeji.top

JS:   static f() {}
来源：http://jlt.jinqigufen.top

TS:   static f(): void {}
来源：http://tpq.birdmap.top

Java: static void f() {}
来源：http://ttg.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lpf.ivvv.top

Ruby: def self.f; end
来源：http://fnl.fengsongda.top

C#:   public static void F() {}
来源：http://hle.xuanzx.com

[G09] 接口 / 抽象类
来源：http://ede.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://kzb.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://atb.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://liu.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://upb.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://vfu.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://aur.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bnh.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://kvl.jianghu66.top

[G10] 访问控制
来源：http://sfz.shanyushiyangtech.top

Py:   约定 _protected / __private（不强制）
来源：http://sfd.hcnkem.com

PHP:  public / protected / private
来源：http://ynx.yonumen.top

JS:   #private 字段；其余公开
来源：http://vdf.tianlin.xyz

TS:   public / protected / private
来源：http://rnl.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://rqf.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://dry.chenlongwang.top

Ruby: public / protected / private
来源：http://prw.gogol.net.cn

C#:   public / protected / private / internal
来源：http://sen.hnqzz.top

[G11] getter / setter
来源：http://mqe.sxryk.cn

Py:   @property 与 @x.setter
来源：http://lvj.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lbd.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://ffb.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://mby.xinyue.icu

Java: public String getName() { return name; }
来源：http://cke.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hzn.yanxiufei.cn

Ruby: attr_accessor :name
来源：http://dkb.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://bsu.smart0.xyz

[G12] 对象转字符串
来源：http://vaf.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://hlo.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sdu.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://dif.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://olq.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://npq.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://grk.zycfv.cn

Ruby: def to_s; @name; end
来源：http://lhl.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://dbz.hnqzz.top

[G13] 判断对象类型
来源：http://wuo.shzxlz.cn

Py:   isinstance(u, User)
来源：http://iht.hywenlv.cn

PHP:  $u instanceof User
来源：http://jtb.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://fap.nanxuanxn.top

TS:   u instanceof User
来源：http://dys.jinqigfzy.top

Java: u instanceof User
来源：http://vbr.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hki.sxryk.cn

Ruby: u.is_a?(User)
来源：http://wsm.shuidangran.top

C#:   u is User
来源：http://mxi.mhx1999.top

[G14] 数据类 / record
来源：http://hpz.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qij.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://wzl.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pla.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://yrn.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://srr.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://fev.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gzj.316326.xyz

C#:   record User(string Name, int Age);
来源：http://qpf.cdnleiting.top

[G15] 枚举
来源：http://ktf.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tms.yj20258888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://inx.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xxh.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vmk.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://syb.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vuy.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://mjv.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://exl.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://cpt.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tec.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://esh.tianlin.xyz

JS:   Object.entries(obj)
来源：http://ken.dashuyun.cn

TS:   Object.entries(obj)
来源：http://uzh.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://adj.zhoulong.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://kqa.zhixingplan.top

Ruby: obj.instance_variables
来源：http://rqy.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://vkd.guannengcc.top

================================================================================
来源：http://ovw.cdnleiting.top

H. 异常与错误处理
来源：http://uyc.dianchejie.cn

================================================================================
来源：http://iur.hfpthk.cn

[H01] try / catch 基础
来源：http://jqf.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://paz.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ofu.cucudq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wqe.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://grq.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://naa.hammf.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rgw.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pvc.hfpthk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ykx.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://kpo.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sia.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jtc.pengpengdd.cyou

JS:   try { f(); } finally { cleanup(); }
来源：http://rte.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lxv.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://seh.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oee.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jbd.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pza.jlsjyb.cn

[H03] 主动抛出异常
来源：http://uqt.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://ewb.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gys.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://oks.uphjek.com


<!-- 参考信息 -->