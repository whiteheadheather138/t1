代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://ycp.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://dum.nwbrower.top

Java: s.lines().toList()
来源：http://kmk.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://xys.yuxming.cn

Ruby: s.lines
来源：http://jgr.jlsjyb.cn

C#:   s.Split('\n')
来源：http://zvk.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://yhg.epnwcf.com

Py:   if not s:
来源：http://fdu.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lsc.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gdd.epnwcf.com

TS:   if (s === "") {}
来源：http://oyb.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://lms.tanke756.top

Go:   if s == "" {}
来源：http://qxl.fengsongda.top

Ruby: if s.empty?
来源：http://ssy.jinqigufen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zuo.tanke756.top

[E21] 超长截断加省略号
来源：http://ecq.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tyr.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pra.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://erc.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iql.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vyy.xinyue.icu

Go:   // 按 rune 判断长度后截断
来源：http://wcz.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://thr.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hoc.tian-w.cn

[E22] 字节长度与字符长度
来源：http://ppi.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iqm.yongpay.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hnb.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cvd.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://skb.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pee.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iqd.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://uhx.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wvg.meibo888.top

================================================================================
来源：http://dsg.cdnleiting.top

F. 文件与目录
来源：http://qmq.ehwqpu.com

================================================================================
来源：http://vru.svipenyu.cn

[F01] 读取整个文件
来源：http://tpb.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qdm.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://tnp.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jbm.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vpt.meibo888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mwz.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bva.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://tyq.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://bza.nanxinkj.top

[F02] 逐行读取文件
来源：http://zls.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dgh.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cnm.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lnd.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gmg.uphjek.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sln.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kme.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://msc.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cac.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://jrg.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ump.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://uxj.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mnl.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sba.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fmw.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dnt.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://fjs.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://msl.sweek.top

[F04] 追加写入文件
来源：http://rvf.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wvz.sxryk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://atk.gotoacloud.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kfb.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwv.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dim.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uzc.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dtn.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://swt.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://igu.bbcook.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sdb.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://lht.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://rhs.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://vii.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ngb.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://brb.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://fek.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://cbo.chenzaomai.com

[F06] 删除文件
来源：http://nju.ydzc1.top

Py:   os.remove("a.txt")
来源：http://sle.tian-w.cn

PHP:  unlink("a.txt");
来源：http://xnz.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://wqs.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://jtv.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://otn.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://huk.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://jvr.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://qvp.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://rou.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://syf.zhoulong.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uui.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jno.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rrt.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jkf.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jlc.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://udk.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ugv.jlsjyb.cn

[F08] 遍历目录
来源：http://uzn.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://shi.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mll.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://dia.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://mcu.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ffi.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qmp.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://uok.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://jua.yangfankeji.com

[F09] 获取文件大小
来源：http://gzv.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://nzw.c1oappe.top

PHP:  filesize("a.txt");
来源：http://axt.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://rkt.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://oxe.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jfe.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://joj.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://mjl.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://wdx.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://tcc.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qvj.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mbk.xuetiantiany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eph.fktsv.cn

TS:   path.extname("a.txt")
来源：http://amh.pengpengdd.cyou

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jje.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yxs.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cgu.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ahw.xziqi.cn

[F11] 复制与移动文件
来源：http://vrv.ivvv.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hkg.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yae.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mke.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xex.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://liv.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bhq.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://whd.yongpay.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ggj.chenjidiqi.icu

[F12] CSV 读写
来源：http://jkb.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ban.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://khc.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cws.nanxuanxn.top

TS:   // 同上
来源：http://aby.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://crb.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bdc.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bbz.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tmf.9152youxi.cn

================================================================================
来源：http://wsb.zhengqikj.top

G. 面向对象
来源：http://nst.uphjek.com

================================================================================
来源：http://ggv.fehbvm.com

[G01] 定义类
来源：http://yea.dashuyun.cn

Py:   class User: pass
来源：http://kjg.bjfxy.top

PHP:  class User {}
来源：http://gss.yongpay.top

JS:   class User {}
来源：http://tij.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://kft.yonumen.top

Java: class User {}
来源：http://fhp.hnqzz.top

Go:   type User struct { Name string }
来源：http://jua.havefunace.top

Ruby: class User; end
来源：http://xjc.smart0.xyz

C#:   class User {}
来源：http://gva.sweek.top

[G02] 构造函数
来源：http://lih.snrcjt.cn

Py:   def __init__(self, name): self.name = name
来源：http://xbu.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://qki.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://gnd.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://hrq.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://deg.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xzf.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://aiq.yangfankeji.com

C#:   public User(string name) { Name = name; }
来源：http://hwy.guannengcc.top

[G03] 实例属性
来源：http://omm.cucudq.cn

Py:   self.name = "x"
来源：http://huv.yuanzhike.top

PHP:  public string $name = "x";
来源：http://arr.zhixingplan.top

JS:   this.name = "x";
来源：http://bnf.svipenyu.cn

TS:   name: string = "x";
来源：http://qlr.zycfv.cn

Java: private String name;
来源：http://rgk.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gon.hnqzz.top

Ruby: @name = "x"
来源：http://vrf.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://rxa.gotoacloud.top

[G04] 定义方法
来源：http://wdw.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://ytp.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://eip.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://ext.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://ivi.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://elc.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qcy.vehdjk.com

Ruby: def greet; @name; end
来源：http://aaf.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://zew.hongshengwenyu.top

[G05] 继承
来源：http://prw.ybcxt.top

Py:   class Admin(User): pass
来源：http://nwm.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://juk.yj20258.top

JS:   class Admin extends User {}
来源：http://xht.hfpthk.cn

TS:   class Admin extends User {}
来源：http://owh.gaohongyu789.top

Java: class Admin extends User {}
来源：http://zcr.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://okm.andypj.xyz

Ruby: class Admin < User; end
来源：http://cuy.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://hpw.wangdashe.top

[G06] 重写方法
来源：http://uut.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://szd.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bhl.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://ixx.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://amv.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://xxu.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ltc.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://zui.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://wpd.yj20258.top

[G07] 调用父类方法
来源：http://uhx.yfazqb.com

Py:   super().greet()
来源：http://ekt.daria6918.cn

PHP:  parent::greet();
来源：http://qsq.fzhhl.top

JS:   super.greet();
来源：http://kkt.shanyushiyangtech.top

TS:   super.greet();
来源：http://lql.zhoulong.xyz

Java: super.greet();
来源：http://rxf.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vlw.zycfv.cn

Ruby: super
来源：http://tvo.snrcjt.cn

C#:   base.Greet();
来源：http://ugi.zhijiandao.cn

[G08] 静态方法与属性
来源：http://xtn.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hpg.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://sgf.c1oappe.top

JS:   static f() {}
来源：http://upp.sweek.top

TS:   static f(): void {}
来源：http://bnn.xylfe.cn

Java: static void f() {}
来源：http://ftx.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tfj.quarkkingdee.top

Ruby: def self.f; end
来源：http://yqy.hnqzz.top

C#:   public static void F() {}
来源：http://uzy.hongshengwenyu.top

[G09] 接口 / 抽象类
来源：http://olk.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://tiu.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://vmt.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lxo.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://kcc.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://zsl.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://kxr.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fyf.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://nfz.nanxinkj.top

[G10] 访问控制
来源：http://eev.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://nrp.yangfankeji.com

PHP:  public / protected / private
来源：http://uxu.tanke756.top

JS:   #private 字段；其余公开
来源：http://vqq.yj20258.top

TS:   public / protected / private
来源：http://rxq.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://qud.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://jqv.zhixingplan.top

Ruby: public / protected / private
来源：http://ycl.hammf.cn

C#:   public / protected / private / internal
来源：http://ozt.yj20258888.top

[G11] getter / setter
来源：http://jtx.yj20258888.top

Py:   @property 与 @x.setter
来源：http://oyy.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://bhi.ybcxt.top

JS:   get name() { return this._name; }
来源：http://dwl.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://jie.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://pyj.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xcs.yj20258888.top

Ruby: attr_accessor :name
来源：http://lps.ybcxt.top

C#:   public string Name { get; set; }
来源：http://bil.wangdashe.top

[G12] 对象转字符串
来源：http://jsx.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://wfk.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ylf.vehdjk.com

JS:   toString() { return this.name; }
来源：http://atm.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://uuf.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://yhq.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://kod.yueranfly.top

Ruby: def to_s; @name; end
来源：http://iig.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://jgt.epnwcf.com

[G13] 判断对象类型
来源：http://isd.cdnleiting.top

Py:   isinstance(u, User)
来源：http://tkh.birdmap.top

PHP:  $u instanceof User
来源：http://thu.yvedp.cn

JS:   u instanceof User
来源：http://kqo.fehbvm.com

TS:   u instanceof User
来源：http://bca.pengpengdd.cyou

Java: u instanceof User
来源：http://fxr.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hlv.daxiang520.top

Ruby: u.is_a?(User)
来源：http://eli.shzxlz.cn

C#:   u is User
来源：http://qoa.birdmap.top

[G14] 数据类 / record
来源：http://jjl.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://omz.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://vbv.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://soa.tanke756.top

TS:   type User = { name: string; age: number };
来源：http://avn.tanke756.top

Java: record User(String name, int age) {}
来源：http://kej.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://eqy.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tno.fzhhl.top

C#:   record User(string Name, int Age);
来源：http://qjx.9152youxi.cn

[G15] 枚举
来源：http://yer.ydzc1.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://azf.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://gfc.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://grl.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://otn.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://mof.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gvq.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://yek.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ify.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://tmz.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wlz.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://yhx.gogol.net.cn

JS:   Object.entries(obj)
来源：http://xtq.yuanzhike.top

TS:   Object.entries(obj)
来源：http://mbp.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bfh.yongpay.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ane.9152youxi.cn

Ruby: obj.instance_variables
来源：http://fno.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://imi.jinghuilouyu.cn

================================================================================
来源：http://qkw.ybcxt.top

H. 异常与错误处理
来源：http://miw.tanke756.top

================================================================================
来源：http://gaq.haohaochexian.top

[H01] try / catch 基础
来源：http://dsj.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zyz.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wwk.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kbr.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uau.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://efa.xylfe.cn


<!-- 参考信息 -->