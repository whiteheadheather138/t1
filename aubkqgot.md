代发 wailian999

Ruby: s.lines
来源：http://vdu.jlsjyb.cn

C#:   s.Split('\n')
来源：http://loj.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://lpg.fanxiaobao.xyz

Py:   if not s:
来源：http://duk.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tss.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vxz.vehdjk.com

TS:   if (s === "") {}
来源：http://wre.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://aqp.zhiwuduotai.top

Go:   if s == "" {}
来源：http://oqx.zhongyouzk.top

Ruby: if s.empty?
来源：http://zwm.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ili.hysaishi.cn

[E21] 超长截断加省略号
来源：http://ksj.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ivq.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nmw.sxryk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ogh.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qko.yueranfly.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rpc.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://ptt.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jqw.nwbrower.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://joy.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://haf.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zco.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tyk.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nls.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zpc.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hbd.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bmv.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://tcd.cqqwz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nlo.ydjk.org.cn

================================================================================
来源：http://hcf.xinyue.icu

F. 文件与目录
来源：http://nvh.jiagoushi.top

================================================================================
来源：http://qmp.jinqigufen.top

[F01] 读取整个文件
来源：http://wgf.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://emu.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://wue.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://plm.yuxming.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rvj.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qmn.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pfh.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://xiz.wangshuangyany.cn

C#:   File.ReadAllText("a.txt");
来源：http://yvp.cheryme.top

[F02] 逐行读取文件
来源：http://cgi.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hmd.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://czs.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fez.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tot.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tbi.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sxw.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rvk.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xyr.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://cwt.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qdc.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://snj.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nvs.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wpt.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rwd.zhengqikj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aze.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://sfi.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://udl.daria6918.cn

[F04] 追加写入文件
来源：http://kcq.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dlc.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wqg.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lei.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvu.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wrd.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qzj.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wio.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dkr.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://cnq.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uug.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://jln.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://dqj.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://cag.uphjek.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ocr.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pot.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://gxn.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://acp.jlsjyb.cn

[F06] 删除文件
来源：http://vfu.sxryk.cn

Py:   os.remove("a.txt")
来源：http://vjq.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://ehf.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://epm.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://vah.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cfi.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://uab.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://szr.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://jsy.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://ixu.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hen.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rjp.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tgf.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yex.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gmc.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yde.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dnn.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://was.jinqigfzy.top

[F08] 遍历目录
来源：http://cxa.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mcg.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xwo.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://tjt.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://qsw.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wgu.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://aae.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://osc.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://uvx.wangdashe.top

[F09] 获取文件大小
来源：http://rso.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://hex.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://fvg.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://ego.sysykeji.top

TS:   fs.statSync("a.txt").size
来源：http://zyx.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://cde.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nsz.pycfn.com

Ruby: File.size("a.txt")
来源：http://xin.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://pyo.hnqzz.top

[F10] 取文件扩展名 / 文件名
来源：http://nzb.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gev.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://atg.ppjwa.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wxk.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://wxg.pengpengdd.cyou

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ydc.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yov.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ryd.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bfq.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://dry.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fpf.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vse.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hcn.zdqjudy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cnb.tanke756.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sik.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wye.jinyuanbaomall.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ebs.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lku.xuetiantiany.cn

[F12] CSV 读写
来源：http://ayn.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://acv.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pvk.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zst.kuanghao11.cn

TS:   // 同上
来源：http://mds.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sjf.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ets.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bal.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wah.epnwcf.com

================================================================================
来源：http://tdp.yj20258.top

G. 面向对象
来源：http://zwu.chenlongwang.top

================================================================================
来源：http://tpy.fktsv.cn

[G01] 定义类
来源：http://nkd.quarkkingdee.top

Py:   class User: pass
来源：http://mgt.xuanzx.com

PHP:  class User {}
来源：http://pcq.daria6918.cn

JS:   class User {}
来源：http://oef.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://qzm.iojbl.cn

Java: class User {}
来源：http://tdz.jiagoushi.top

Go:   type User struct { Name string }
来源：http://obi.vehdjk.com

Ruby: class User; end
来源：http://rck.xuetiantiany.cn

C#:   class User {}
来源：http://izp.xuanzx.com

[G02] 构造函数
来源：http://svx.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://tqk.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://gck.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://pry.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://tvb.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://qyi.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ilp.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://iha.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://nzm.nanxinkj.top

[G03] 实例属性
来源：http://mik.jqgufenzy.top

Py:   self.name = "x"
来源：http://owf.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://kjw.feifeiyinyue.top

JS:   this.name = "x";
来源：http://zev.yuxming.cn

TS:   name: string = "x";
来源：http://hio.snrcjt.cn

Java: private String name;
来源：http://zqc.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pvm.tanke756.top

Ruby: @name = "x"
来源：http://oel.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://xje.yonumen.top

[G04] 定义方法
来源：http://gqf.yvedp.cn

Py:   def greet(self): return self.name
来源：http://eoz.zdbjq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hni.wangshuangyany.cn

JS:   greet() { return this.name; }
来源：http://wvg.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://ktm.yvedp.cn

Java: String greet() { return name; }
来源：http://zib.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wki.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://qai.cucudq.cn

C#:   public string Greet() => Name;
来源：http://kod.redwolf501.top

[G05] 继承
来源：http://gsp.snrcjt.cn

Py:   class Admin(User): pass
来源：http://pvq.sweek.top

PHP:  class Admin extends User {}
来源：http://dcu.ehwqpu.com

JS:   class Admin extends User {}
来源：http://wla.ivvv.top

TS:   class Admin extends User {}
来源：http://fre.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://ipg.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eas.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://uya.jyoumei.cn

C#:   class Admin : User {}
来源：http://qva.zhoulong.xyz

[G06] 重写方法
来源：http://wmh.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://wxh.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://agq.andypj.xyz

JS:   greet() { return "admin"; }
来源：http://awj.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://ffu.jinyuanbaomall.cn

Java: @Override String greet() { return "admin"; }
来源：http://hwr.haohaochexian.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xkr.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://xjp.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://bys.smart0.xyz

[G07] 调用父类方法
来源：http://rig.cashguo.top

Py:   super().greet()
来源：http://zgu.yuxming.cn

PHP:  parent::greet();
来源：http://dvh.jinqigufen.top

JS:   super.greet();
来源：http://lwb.jqgufenzy.top

TS:   super.greet();
来源：http://mkr.sxryk.cn

Java: super.greet();
来源：http://rsu.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cha.yfazqb.com

Ruby: super
来源：http://wgt.hnxiangtu.top

C#:   base.Greet();
来源：http://frs.yvedp.cn

[G08] 静态方法与属性
来源：http://vdm.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ixu.cheryme.top

PHP:  public static function f() {}
来源：http://cyv.birdmap.top

JS:   static f() {}
来源：http://ewk.dianchejie.cn

TS:   static f(): void {}
来源：http://sys.jinqigufen.top

Java: static void f() {}
来源：http://bol.yj20258888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qdw.guannengcc.top

Ruby: def self.f; end
来源：http://jrb.shuidangran.top

C#:   public static void F() {}
来源：http://cpa.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://xty.yvedp.cn

Py:   from abc import ABC, abstractmethod
来源：http://tam.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://fco.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://iwv.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://sgj.havefunace.top

Java: interface Shape { double area(); }
来源：http://ygd.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://wxb.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jjx.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://piq.aibaodan.cn

[G10] 访问控制
来源：http://ufa.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://wnz.shuidangran.top

PHP:  public / protected / private
来源：http://jco.yvedp.cn

JS:   #private 字段；其余公开
来源：http://bvx.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://xue.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://nwz.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://btu.dashuyun.cn

Ruby: public / protected / private
来源：http://yki.jianghu66.top

C#:   public / protected / private / internal
来源：http://obz.dianchejie.cn

[G11] getter / setter
来源：http://pnq.fzhhl.top

Py:   @property 与 @x.setter
来源：http://lgp.316326.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ntp.gzhubu.top

JS:   get name() { return this._name; }
来源：http://pqo.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://hmh.aizwys.cn

Java: public String getName() { return name; }
来源：http://ahw.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wiz.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://jru.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://sss.tianlin.xyz

[G12] 对象转字符串
来源：http://fjj.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://ujp.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://cae.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://ibn.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://gpj.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://wvz.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mpc.bbcook.cn

Ruby: def to_s; @name; end
来源：http://ttb.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://xeb.cucudq.cn

[G13] 判断对象类型
来源：http://isz.smart0.xyz

Py:   isinstance(u, User)
来源：http://ygk.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://ctu.tarul.cn

JS:   u instanceof User
来源：http://ynh.sweek.top

TS:   u instanceof User
来源：http://xwb.cheryme.top

Java: u instanceof User
来源：http://igd.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://yrc.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://jtv.yangfankeji.com

C#:   u is User
来源：http://duw.daxiang520.top

[G14] 数据类 / record
来源：http://vhs.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://upo.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://vtt.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://thg.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://qln.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://tjl.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://tbd.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bcu.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://rrx.yanxiufei.cn

[G15] 枚举
来源：http://qjj.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dwc.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sip.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://chv.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kac.yanxiufei.cn

Java: enum Color { RED, GREEN }
来源：http://wty.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qnv.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://gif.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mwd.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://emi.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mnd.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://ijh.xziqi.cn

JS:   Object.entries(obj)
来源：http://utz.tarul.cn

TS:   Object.entries(obj)
来源：http://emf.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zns.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://gyb.cqqwz.cn

Ruby: obj.instance_variables
来源：http://bjj.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://pdp.dianchejie.cn

================================================================================
来源：http://jts.cucudq.cn

H. 异常与错误处理
来源：http://fsg.yanxiufei.cn

================================================================================
来源：http://zrz.smart0.xyz

[H01] try / catch 基础
来源：http://htv.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jbu.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lhl.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://har.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vbn.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://niu.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hlk.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cwy.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hvg.yvedp.cn

[H02] finally / ensure 收尾
来源：http://kyu.yonumen.top


<!-- 参考信息 -->