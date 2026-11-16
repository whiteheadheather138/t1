代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://osq.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nfo.shangyingyoupin.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://urv.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mck.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xdf.havefunace.top

[E19] 多行文本按行拆分
来源：http://vou.chenlongwang.top

Py:   s.splitlines()
来源：http://nyt.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://syj.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://frq.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://xha.ydjk.org.cn

Java: s.lines().toList()
来源：http://ach.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://gqk.birdmap.top

Ruby: s.lines
来源：http://hcv.mhx1999.top

C#:   s.Split('\n')
来源：http://kqk.aizwys.cn

[E20] 判断字符串是否为空
来源：http://xci.snrcjt.cn

Py:   if not s:
来源：http://rat.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nby.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vhz.jqgufenzy.top

TS:   if (s === "") {}
来源：http://xfo.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://pwu.ehwqpu.com

Go:   if s == "" {}
来源：http://hrm.quarkkingdee.top

Ruby: if s.empty?
来源：http://wdl.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ldx.ivvv.top

[E21] 超长截断加省略号
来源：http://tgv.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://irf.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kei.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ede.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zqj.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://may.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://rwd.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sag.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lnl.fehbvm.com

[E22] 字节长度与字符长度
来源：http://akb.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jud.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rua.svipenyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jxt.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gbw.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wxz.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ogf.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://aij.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ghd.tianlin.xyz

================================================================================
来源：http://kyr.shangyingyoupin.top

F. 文件与目录
来源：http://guz.kuanghao11.cn

================================================================================
来源：http://nmn.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://lwr.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vpj.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://mvi.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wju.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wsp.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gex.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dkn.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://nak.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://iiv.chenzaomai.com

[F02] 逐行读取文件
来源：http://mry.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tmm.cdnleiting.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cdz.svipenyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ndo.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lqw.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nfj.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mww.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tmd.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zll.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://api.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cbx.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pwd.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oft.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://luw.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dvh.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dxt.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://hzy.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dpi.gotoacloud.top

[F04] 追加写入文件
来源：http://rcj.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gby.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://obg.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://veg.jinghuilouyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ccj.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rcp.zycfv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nah.fzhhl.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zcj.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tmm.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://qhy.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vgx.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://uwl.feifeiyinyue.top

JS:   fs.existsSync("a.txt")
来源：http://oko.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://ftw.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jtl.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ohm.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://vrq.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://cab.bjfxy.top

[F06] 删除文件
来源：http://hfm.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://zwu.daria6918.cn

PHP:  unlink("a.txt");
来源：http://dnj.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://zih.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://rsi.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wkd.wangshuangyany.cn

Go:   os.Remove("a.txt")
来源：http://xee.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://cvw.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://nod.tanke756.top

[F07] 创建目录（含多级）
来源：http://uox.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cbo.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ijx.yongpay.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mht.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rii.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cqe.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dxy.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vhs.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jhw.xziqi.cn

[F08] 遍历目录
来源：http://rpl.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://mgg.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wuo.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://vux.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://yes.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ehj.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ocu.tian-w.cn

Ruby: Dir.children("dir")
来源：http://ecb.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://wsc.gogol.net.cn

[F09] 获取文件大小
来源：http://hdh.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://ydb.bbcook.cn

PHP:  filesize("a.txt");
来源：http://chn.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://ekj.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://yax.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kay.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://taa.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://wql.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://nki.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://rev.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hpj.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vel.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kbo.guowangkeji.top

TS:   path.extname("a.txt")
来源：http://lff.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ips.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uec.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gnq.zycfv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xqq.cashguo.top

[F11] 复制与移动文件
来源：http://yly.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://msc.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://shx.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yvi.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://myo.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ctc.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zqq.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://elx.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zge.yuanzhike.top

[F12] CSV 读写
来源：http://giy.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://exl.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://quy.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jwb.feifeiyinyue.top

TS:   // 同上
来源：http://mud.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hlt.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rot.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ozc.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pwf.cdnleiting.top

================================================================================
来源：http://cvo.zhongyouzk.top

G. 面向对象
来源：http://mzg.c1oappe.top

================================================================================
来源：http://nah.xuanzx.com

[G01] 定义类
来源：http://zkp.316326.xyz

Py:   class User: pass
来源：http://vki.feifeiyinyue.top

PHP:  class User {}
来源：http://enc.yj20258888.top

JS:   class User {}
来源：http://ttp.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://mnu.c1oappe.top

Java: class User {}
来源：http://lhy.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://wcj.bbcook.cn

Ruby: class User; end
来源：http://qtt.zhijiandao.cn

C#:   class User {}
来源：http://knq.jqgfzy.top

[G02] 构造函数
来源：http://lfb.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://mad.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://oog.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://jaj.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://bto.snrcjt.cn

Java: User(String name) { this.name = name; }
来源：http://zeg.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lwk.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://brn.hysaishi.cn

C#:   public User(string name) { Name = name; }
来源：http://dfy.chenlongwang.top

[G03] 实例属性
来源：http://awl.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://tkg.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://mav.zhijiandao.cn

JS:   this.name = "x";
来源：http://spw.pycfn.com

TS:   name: string = "x";
来源：http://apt.jlsjyb.cn

Java: private String name;
来源：http://zqj.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mol.zhongyouzk.top

Ruby: @name = "x"
来源：http://dwo.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://nqr.ywan-chungtsiang.top

[G04] 定义方法
来源：http://rwi.andypj.xyz

Py:   def greet(self): return self.name
来源：http://zek.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dbf.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://vyd.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://zdf.sjlbkw.cn

Java: String greet() { return name; }
来源：http://anu.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://esg.snrcjt.cn

Ruby: def greet; @name; end
来源：http://sus.yuxming.cn

C#:   public string Greet() => Name;
来源：http://ksq.zycfv.cn

[G05] 继承
来源：http://bjl.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://zcx.sxryk.cn

PHP:  class Admin extends User {}
来源：http://fdf.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://cni.sweek.top

TS:   class Admin extends User {}
来源：http://nlm.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://obl.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xly.ctjpmb.com

Ruby: class Admin < User; end
来源：http://qep.hfpthk.cn

C#:   class Admin : User {}
来源：http://vzq.jianghu66.top

[G06] 重写方法
来源：http://vme.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://esh.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ypo.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://btd.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://oox.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://kio.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jwl.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://nxl.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://vld.hongshengwenyu.top

[G07] 调用父类方法
来源：http://zod.jinghuilouyu.cn

Py:   super().greet()
来源：http://cmn.cqqwz.cn

PHP:  parent::greet();
来源：http://xsh.vehdjk.com

JS:   super.greet();
来源：http://abs.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://xbo.gaohongyu789.top

Java: super.greet();
来源：http://cfl.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rwf.zhoulong.xyz

Ruby: super
来源：http://eyu.chenzaomai.com

C#:   base.Greet();
来源：http://kyy.jiagoushi.top

[G08] 静态方法与属性
来源：http://xlx.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ufc.yonumen.top

PHP:  public static function f() {}
来源：http://hkp.zhixingplan.top

JS:   static f() {}
来源：http://cvm.fzhhl.top

TS:   static f(): void {}
来源：http://vdr.shangyingyoupin.top

Java: static void f() {}
来源：http://arf.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qaw.yj20258888.top

Ruby: def self.f; end
来源：http://qiz.ybcxt.top

C#:   public static void F() {}
来源：http://uoq.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://mmr.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://mim.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://dgu.jinyuanbaomall.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eej.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://eun.52xcode.cn

Java: interface Shape { double area(); }
来源：http://fzm.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://xar.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aaw.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://aez.fanxiaobao.xyz

[G10] 访问控制
来源：http://ntr.tianlin.xyz

Py:   约定 _protected / __private（不强制）
来源：http://sfz.birdmap.top

PHP:  public / protected / private
来源：http://rza.fktsv.cn

JS:   #private 字段；其余公开
来源：http://pds.pengpengdd.cyou

TS:   public / protected / private
来源：http://ete.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://zfo.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jup.ydzc1.top

Ruby: public / protected / private
来源：http://wcx.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://fnf.ivvv.top

[G11] getter / setter
来源：http://qbz.tanke756.top

Py:   @property 与 @x.setter
来源：http://zvd.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://afr.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://zvb.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://oth.redwolf501.top

Java: public String getName() { return name; }
来源：http://wdn.chenzaomai.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ngc.zycfv.cn

Ruby: attr_accessor :name
来源：http://uwh.cheryme.top

C#:   public string Name { get; set; }
来源：http://lex.epnwcf.com

[G12] 对象转字符串
来源：http://dgq.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://nar.epnwcf.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://pyr.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://tva.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://hsl.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://ukg.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://mno.yangfankeji.com

Ruby: def to_s; @name; end
来源：http://wlf.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://yhg.hcnkem.com

[G13] 判断对象类型
来源：http://igw.guowangkeji.top

Py:   isinstance(u, User)
来源：http://koe.sysykeji.top

PHP:  $u instanceof User
来源：http://unt.guannengcc.top

JS:   u instanceof User
来源：http://ego.52xcode.cn

TS:   u instanceof User
来源：http://nnt.daria6918.cn

Java: u instanceof User
来源：http://umu.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ccp.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://bsh.vqdsnc.cn

C#:   u is User
来源：http://gin.tarul.cn

[G14] 数据类 / record
来源：http://unt.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ejj.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://dfk.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bzu.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://eoi.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://jod.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://wsf.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zif.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://arn.redwolf501.top

[G15] 枚举
来源：http://wza.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qob.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://igr.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ozz.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qfh.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://uvy.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uja.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://htd.hnqzz.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://crc.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://tbw.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cln.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://jee.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://rqt.yuanzhike.top

TS:   Object.entries(obj)
来源：http://pft.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pav.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mhl.jinqigufen.top

Ruby: obj.instance_variables
来源：http://qvh.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://sgn.kuanghao11.cn

================================================================================
来源：http://nlf.hammf.cn


<!-- 参考信息 -->