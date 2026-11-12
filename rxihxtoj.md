代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xby.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://yse.sxryk.cn

Py:   s.splitlines()
来源：http://wzq.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mov.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://ybb.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://uje.mhx1999.top

Java: s.lines().toList()
来源：http://pwg.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://wwa.redwolf501.top

Ruby: s.lines
来源：http://dzt.bjfxy.top

C#:   s.Split('\n')
来源：http://pcd.cucudq.cn

[E20] 判断字符串是否为空
来源：http://met.zdbjq.cn

Py:   if not s:
来源：http://pvc.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rft.shangyingyoupin.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://skt.uphjek.com

TS:   if (s === "") {}
来源：http://sgw.dashuyun.cn

Java: if (s.isEmpty()) {}
来源：http://kqz.dashuyun.cn

Go:   if s == "" {}
来源：http://bne.yvedp.cn

Ruby: if s.empty?
来源：http://wus.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pgf.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://onj.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cfe.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jep.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nyd.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xhv.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xcd.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://ssc.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qli.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://suy.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://qed.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kha.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qac.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mit.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mac.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nrm.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ddf.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://wkh.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uid.tanke756.top

================================================================================
来源：http://bfj.daxiang520.top

F. 文件与目录
来源：http://pxc.epnwcf.com

================================================================================
来源：http://lif.feifeiyinyue.top

[F01] 读取整个文件
来源：http://gap.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hum.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://tbf.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jic.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lmg.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rtj.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://myb.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://bwx.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://fjn.cucudq.cn

[F02] 逐行读取文件
来源：http://yqq.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wsw.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ubl.chenjidiqi.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lbb.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bnn.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sdy.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pgu.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fkg.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://flf.bbcook.cn

[F03] 写入文件（覆盖）
来源：http://dqv.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hzp.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ecu.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vzw.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://krn.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xuy.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://amc.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://ypa.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tvg.nanxuanxn.top

[F04] 追加写入文件
来源：http://pqg.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dol.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fjl.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ctu.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jhy.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eru.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xro.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nqk.chenjidiqi.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hvx.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://hck.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yvu.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://hku.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://bas.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://tle.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kif.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qwa.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://vbt.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://zqk.hnqzz.top

[F06] 删除文件
来源：http://pnw.bjfxy.top

Py:   os.remove("a.txt")
来源：http://nvm.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://znq.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zbi.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://yba.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tph.cashguo.top

Go:   os.Remove("a.txt")
来源：http://nmj.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://wye.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://qdb.tarul.cn

[F07] 创建目录（含多级）
来源：http://qme.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vnd.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vpo.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vmw.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzg.hnxiangtu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jxr.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yjs.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gka.9152youxi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dxk.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://tax.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://unf.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wez.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://zue.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://iji.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yio.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ocj.tarul.cn

Ruby: Dir.children("dir")
来源：http://atg.aizwys.cn

C#:   Directory.GetFiles("dir")
来源：http://xpu.chenzaomai.com

[F09] 获取文件大小
来源：http://qwx.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://lcz.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://lqn.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://cuq.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://stl.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://aid.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nts.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://bkm.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://cgu.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://hbg.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rsr.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vnr.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fvx.tian-w.cn

TS:   path.extname("a.txt")
来源：http://ene.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jwt.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vjj.smart0.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rwe.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://goy.andypj.xyz

[F11] 复制与移动文件
来源：http://gry.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cjz.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ioh.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ulc.yj202588.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gxj.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lew.yuanzhike.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qmv.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rug.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://obz.dianchejie.cn

[F12] CSV 读写
来源：http://mua.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qly.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://shh.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tas.hfpthk.cn

TS:   // 同上
来源：http://rjs.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bwj.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kwr.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sso.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mxp.andypj.xyz

================================================================================
来源：http://qwr.yonumen.top

G. 面向对象
来源：http://pzr.52xcode.cn

================================================================================
来源：http://gyp.yvedp.cn

[G01] 定义类
来源：http://tor.jinyuanbaomall.cn

Py:   class User: pass
来源：http://tkq.yonumen.top

PHP:  class User {}
来源：http://qwk.zhixingplan.top

JS:   class User {}
来源：http://vyt.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://qwu.tianlin.xyz

Java: class User {}
来源：http://ymb.chenzaomai.com

Go:   type User struct { Name string }
来源：http://eat.ydjk.org.cn

Ruby: class User; end
来源：http://wpl.yuanzhike.top

C#:   class User {}
来源：http://dqa.pengpengdd.cyou

[G02] 构造函数
来源：http://uoc.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://oee.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://yms.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://zra.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://cfq.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://ozh.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://urj.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://qru.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://zgm.daria6918.cn

[G03] 实例属性
来源：http://pxq.ybcxt.top

Py:   self.name = "x"
来源：http://rur.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://lng.xinyue.icu

JS:   this.name = "x";
来源：http://ouj.tarul.cn

TS:   name: string = "x";
来源：http://axf.kuanghao11.cn

Java: private String name;
来源：http://vtj.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ztx.dianchejie.cn

Ruby: @name = "x"
来源：http://znc.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://dqv.nanxuanxn.top

[G04] 定义方法
来源：http://bch.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://xkm.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://heb.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://qim.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://fes.xylfe.cn

Java: String greet() { return name; }
来源：http://bav.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://han.hammf.cn

Ruby: def greet; @name; end
来源：http://fpv.yj20258888.top

C#:   public string Greet() => Name;
来源：http://wlp.ywan-chungtsiang.top

[G05] 继承
来源：http://eem.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://tzw.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://svs.ehwqpu.com

JS:   class Admin extends User {}
来源：http://ihq.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://ttz.dashuyun.cn

Java: class Admin extends User {}
来源：http://xnc.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cfa.gotoacloud.top

Ruby: class Admin < User; end
来源：http://fxz.tanke756.top

C#:   class Admin : User {}
来源：http://mym.zdqjudy.top

[G06] 重写方法
来源：http://vjt.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://sgv.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://grg.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://wot.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://cdx.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://qhk.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jhn.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://tlj.dianchejie.cn

C#:   public override string Greet() => "admin";
来源：http://bka.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://cip.jiagoushi.top

Py:   super().greet()
来源：http://tco.hongshengwenyu.top

PHP:  parent::greet();
来源：http://taq.cheryme.top

JS:   super.greet();
来源：http://uxa.zdqjudy.top

TS:   super.greet();
来源：http://xjq.aizwys.cn

Java: super.greet();
来源：http://tty.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wrf.andypj.xyz

Ruby: super
来源：http://cic.sufxvd.cn

C#:   base.Greet();
来源：http://fgy.jianghu66.top

[G08] 静态方法与属性
来源：http://vtp.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fus.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://mje.shanyushiyangkeji.top

JS:   static f() {}
来源：http://ttk.vehdjk.com

TS:   static f(): void {}
来源：http://xxj.pycfn.com

Java: static void f() {}
来源：http://fou.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cvq.cheryme.top

Ruby: def self.f; end
来源：http://sgi.kuanghao11.cn

C#:   public static void F() {}
来源：http://esw.andypj.xyz

[G09] 接口 / 抽象类
来源：http://dlr.9152youxi.cn

Py:   from abc import ABC, abstractmethod
来源：http://qwe.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dih.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rrm.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://xua.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://rdf.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://uol.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rce.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://wgp.birdmap.top

[G10] 访问控制
来源：http://dyl.9152youxi.cn

Py:   约定 _protected / __private（不强制）
来源：http://qwv.yvedp.cn

PHP:  public / protected / private
来源：http://glv.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://xnz.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://otf.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://xvc.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://eed.hcnkem.com

Ruby: public / protected / private
来源：http://xxk.yj20258888.top

C#:   public / protected / private / internal
来源：http://zjw.xziqi.cn

[G11] getter / setter
来源：http://bdu.daxiang520.top

Py:   @property 与 @x.setter
来源：http://ysd.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ifp.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://evf.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://hzd.fzhhl.top

Java: public String getName() { return name; }
来源：http://gkm.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zfe.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://srm.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://eiv.0kj1m.cn

[G12] 对象转字符串
来源：http://kps.sweek.top

Py:   def __str__(self): return self.name
来源：http://fvz.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hrl.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://inp.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://wkz.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://nzm.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://xoh.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://iui.cheryme.top

C#:   public override string ToString() => Name;
来源：http://vre.c1oappe.top

[G13] 判断对象类型
来源：http://fsw.hcnkem.com

Py:   isinstance(u, User)
来源：http://rkb.nwbrower.top

PHP:  $u instanceof User
来源：http://fqk.tianlin.xyz

JS:   u instanceof User
来源：http://jyu.wangshuangyany.cn

TS:   u instanceof User
来源：http://xvl.quarkkingdee.top

Java: u instanceof User
来源：http://nts.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://jbq.9152youxi.cn

Ruby: u.is_a?(User)
来源：http://cvy.yuxming.cn

C#:   u is User
来源：http://bto.bjfxy.top

[G14] 数据类 / record
来源：http://cle.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ihx.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://lsk.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://eqt.svipenyu.cn

TS:   type User = { name: string; age: number };
来源：http://akj.0kj1m.cn

Java: record User(String name, int age) {}
来源：http://dqg.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://edx.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pao.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://pnu.wangshuangyany.cn

[G15] 枚举
来源：http://gcd.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://quv.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dvd.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jhh.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wiu.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://vai.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://shx.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://cki.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jcd.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://gcp.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dok.pycfn.com

PHP:  get_object_vars($obj);
来源：http://xik.bbcook.cn

JS:   Object.entries(obj)
来源：http://kco.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://uvx.yvedp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xzr.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jyl.havefunace.top

Ruby: obj.instance_variables
来源：http://fqw.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://rja.jiagoushi.top

================================================================================
来源：http://prq.shangyingyoupin.top

H. 异常与错误处理
来源：http://gek.mhx1999.top

================================================================================
来源：http://mna.aizwys.cn

[H01] try / catch 基础
来源：http://csi.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fnt.nwbrower.top


<!-- 参考信息 -->