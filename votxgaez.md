代发 wailian999

[E18] 模板占位符替换
来源：http://vjx.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oat.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ysd.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rpr.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://biv.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zui.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cfe.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://igd.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://szv.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://sta.fzhhl.top

Py:   s.splitlines()
来源：http://ydv.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ift.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://xcz.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://dqo.dianchejie.cn

Java: s.lines().toList()
来源：http://hvn.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://bfc.zdbjq.cn

Ruby: s.lines
来源：http://tym.nanxinkj.top

C#:   s.Split('\n')
来源：http://zmp.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://iyp.shzxlz.cn

Py:   if not s:
来源：http://wjx.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://swx.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aav.gzhubu.top

TS:   if (s === "") {}
来源：http://oak.havefunace.top

Java: if (s.isEmpty()) {}
来源：http://nzv.dashuyun.cn

Go:   if s == "" {}
来源：http://jwh.sjlbkw.cn

Ruby: if s.empty?
来源：http://pts.vehdjk.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iil.ppjwa.cn

[E21] 超长截断加省略号
来源：http://bcl.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lxz.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rlg.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ejb.bbcook.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dag.cucudq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yjq.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://eqd.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gjg.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ivg.hammf.cn

[E22] 字节长度与字符长度
来源：http://wtl.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://liq.meibo888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ghe.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://duk.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhh.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kms.ivvv.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xgf.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://saw.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://akt.yj202588.top

================================================================================
来源：http://fev.xuetiantiany.cn

F. 文件与目录
来源：http://odu.cucudq.cn

================================================================================
来源：http://ynj.zhongyouzk.top

[F01] 读取整个文件
来源：http://vbt.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yql.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://alv.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yuu.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wjh.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://hog.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gcq.zycfv.cn

Ruby: File.read("a.txt")
来源：http://flp.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://fck.guowangkeji.top

[F02] 逐行读取文件
来源：http://omm.hesvh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wlt.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sgx.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sad.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kme.zhixingplan.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://phv.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mlp.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gct.ppjwa.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wvd.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://wys.hnxiangtu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gnn.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rto.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oxk.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gjz.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gon.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vir.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://cad.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ent.xuetiantiany.cn

[F04] 追加写入文件
来源：http://qxx.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://smm.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://knk.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aai.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vuq.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bae.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nxg.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rwe.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xux.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://wwe.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tkk.uphjek.com

PHP:  file_exists("a.txt");
来源：http://bym.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://tus.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://ykg.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://upv.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nou.yj202588.top

Ruby: File.exist?("a.txt")
来源：http://jzu.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://rop.tianlin.xyz

[F06] 删除文件
来源：http://rex.birdmap.top

Py:   os.remove("a.txt")
来源：http://abf.ydzc1.top

PHP:  unlink("a.txt");
来源：http://bfb.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://aaa.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://urv.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cbc.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://wuu.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://txj.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://quc.meibo888.top

[F07] 创建目录（含多级）
来源：http://rlx.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfq.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jcl.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eew.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ehx.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wbk.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nvo.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fxp.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bvj.jyoumei.cn

[F08] 遍历目录
来源：http://epp.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gbo.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qeu.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://brt.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://edr.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://irc.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ujp.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://rey.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://jpd.havefunace.top

[F09] 获取文件大小
来源：http://yox.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://phm.c1oappe.top

PHP:  filesize("a.txt");
来源：http://xhw.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://uib.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://fcu.epnwcf.com

Java: Files.size(Path.of("a.txt"))
来源：http://ipk.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mjt.tarul.cn

Ruby: File.size("a.txt")
来源：http://amj.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://mcg.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://upx.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ntg.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xkx.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mrp.xuanzx.com

TS:   path.extname("a.txt")
来源：http://pmi.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xjr.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ygr.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oat.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uqe.sysykeji.top

[F11] 复制与移动文件
来源：http://vaf.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cai.fehbvm.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kbm.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qhk.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oyq.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://onv.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vny.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ubz.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pjk.sjlbkw.cn

[F12] CSV 读写
来源：http://kry.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://awu.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bcx.tianlin.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gmo.nanxinkj.top

TS:   // 同上
来源：http://aqa.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jwc.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ggy.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ipc.fanxiaobao.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://miw.zdbjq.cn

================================================================================
来源：http://xzc.tianlin.xyz

G. 面向对象
来源：http://dkt.wangshuangyany.cn

================================================================================
来源：http://fle.mhx1999.top

[G01] 定义类
来源：http://tvh.gogol.net.cn

Py:   class User: pass
来源：http://fgl.shangyingyoupin.top

PHP:  class User {}
来源：http://jcq.pycfn.com

JS:   class User {}
来源：http://pme.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://dph.fanxiaobao.xyz

Java: class User {}
来源：http://rhj.nwbrower.top

Go:   type User struct { Name string }
来源：http://ial.316326.xyz

Ruby: class User; end
来源：http://tkj.chenjidiqi.icu

C#:   class User {}
来源：http://szp.9152youxi.cn

[G02] 构造函数
来源：http://nba.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://bns.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://vns.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://xcz.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://bml.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://ovs.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vdp.hcnkem.com

Ruby: def initialize(name); @name = name; end
来源：http://wgx.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://kex.haohaochexian.top

[G03] 实例属性
来源：http://prd.jlsjyb.cn

Py:   self.name = "x"
来源：http://xtq.ybcxt.top

PHP:  public string $name = "x";
来源：http://afe.nanxuanxn.top

JS:   this.name = "x";
来源：http://rdp.vqdsnc.cn

TS:   name: string = "x";
来源：http://pwq.yangfankeji.com

Java: private String name;
来源：http://bll.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cjr.feifeiyinyue.top

Ruby: @name = "x"
来源：http://ouf.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://ein.zhengqikj.top

[G04] 定义方法
来源：http://eia.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://bws.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sjb.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://crs.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://gkc.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://wtg.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://shy.hammf.cn

Ruby: def greet; @name; end
来源：http://yth.cheryme.top

C#:   public string Greet() => Name;
来源：http://jvl.xingfuxueyuan.xyz

[G05] 继承
来源：http://grh.snrcjt.cn

Py:   class Admin(User): pass
来源：http://cts.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://ipb.fehbvm.com

JS:   class Admin extends User {}
来源：http://qds.redwolf501.top

TS:   class Admin extends User {}
来源：http://xkq.hfpthk.cn

Java: class Admin extends User {}
来源：http://pih.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kfs.ivvv.top

Ruby: class Admin < User; end
来源：http://eof.iojbl.cn

C#:   class Admin : User {}
来源：http://jgg.52xcode.cn

[G06] 重写方法
来源：http://inr.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://rpu.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fvs.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://hwo.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://qqq.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://cnt.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://owh.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://zmp.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://zha.iojbl.cn

[G07] 调用父类方法
来源：http://yzc.dianchejie.cn

Py:   super().greet()
来源：http://hzw.bbcook.cn

PHP:  parent::greet();
来源：http://hcl.bjfxy.top

JS:   super.greet();
来源：http://ghf.andypj.xyz

TS:   super.greet();
来源：http://smv.vehdjk.com

Java: super.greet();
来源：http://rxu.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ytn.jinqigufen.top

Ruby: super
来源：http://bbl.ppjwa.cn

C#:   base.Greet();
来源：http://rej.snrcjt.cn

[G08] 静态方法与属性
来源：http://rpq.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sga.iojbl.cn

PHP:  public static function f() {}
来源：http://nze.sxryk.cn

JS:   static f() {}
来源：http://rwu.sysykeji.top

TS:   static f(): void {}
来源：http://csd.cashguo.top

Java: static void f() {}
来源：http://uwf.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qru.zhiwuduotai.top

Ruby: def self.f; end
来源：http://kal.ydzc1.top

C#:   public static void F() {}
来源：http://iaf.cheryme.top

[G09] 接口 / 抽象类
来源：http://tet.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://iko.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nhs.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ugc.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://vkp.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://sfc.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://ddq.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iyg.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://kcc.yvedp.cn

[G10] 访问控制
来源：http://nxl.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://lnt.yueranfly.top

PHP:  public / protected / private
来源：http://nys.havefunace.top

JS:   #private 字段；其余公开
来源：http://wka.chenzaomai.com

TS:   public / protected / private
来源：http://fcg.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://ozo.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uwa.hnqzz.top

Ruby: public / protected / private
来源：http://cfu.yongpay.top

C#:   public / protected / private / internal
来源：http://hms.xziqi.cn

[G11] getter / setter
来源：http://qor.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://owf.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yic.zdbjq.cn

JS:   get name() { return this._name; }
来源：http://wcj.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://fje.cucudq.cn

Java: public String getName() { return name; }
来源：http://dsf.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mdd.chenzaomai.com

Ruby: attr_accessor :name
来源：http://yfa.xinyue.icu

C#:   public string Name { get; set; }
来源：http://qza.svipenyu.cn

[G12] 对象转字符串
来源：http://ugl.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://ggc.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://riv.hcnkem.com

JS:   toString() { return this.name; }
来源：http://qdt.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://ole.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://oak.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ncj.yj202588.top

Ruby: def to_s; @name; end
来源：http://zyy.meibo888.top

C#:   public override string ToString() => Name;
来源：http://cae.bjfxy.top

[G13] 判断对象类型
来源：http://vzz.yuanzhike.top

Py:   isinstance(u, User)
来源：http://wuu.chenlongwang.top

PHP:  $u instanceof User
来源：http://lib.jqgufenzy.top

JS:   u instanceof User
来源：http://uym.yongpay.top

TS:   u instanceof User
来源：http://bzo.svipenyu.cn

Java: u instanceof User
来源：http://wep.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ntz.uphjek.com

Ruby: u.is_a?(User)
来源：http://nba.bjfxy.top

C#:   u is User
来源：http://rdu.pycfn.com

[G14] 数据类 / record
来源：http://mmh.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fdq.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://jrk.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rry.shuidangran.top

TS:   type User = { name: string; age: number };
来源：http://pqj.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://edw.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://ami.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wig.9152youxi.cn

C#:   record User(string Name, int Age);
来源：http://ioq.yj20258.top

[G15] 枚举
来源：http://ssq.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ytw.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qxj.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ifh.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dsb.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://rzn.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nad.tianlin.xyz

Ruby: Color = %i[red green].freeze
来源：http://emh.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sgh.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://kkz.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zmj.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://fab.xinyue.icu

JS:   Object.entries(obj)
来源：http://znj.zhixingplan.top

TS:   Object.entries(obj)
来源：http://zlz.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pel.yonumen.top


<!-- 参考信息 -->