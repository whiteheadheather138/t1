代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hwu.birdmap.top

[E19] 多行文本按行拆分
来源：http://oyx.birdmap.top

Py:   s.splitlines()
来源：http://vku.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dvf.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://meb.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://vbn.fengsongda.top

Java: s.lines().toList()
来源：http://nly.ydzc1.top

Go:   strings.Split(s, "\n")
来源：http://eqb.xinyue.icu

Ruby: s.lines
来源：http://izn.jqgfzy.top

C#:   s.Split('\n')
来源：http://mai.fehbvm.com

[E20] 判断字符串是否为空
来源：http://stm.xylfe.cn

Py:   if not s:
来源：http://hzf.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ogu.xziqi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ods.snrcjt.cn

TS:   if (s === "") {}
来源：http://ggn.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://ljh.tianlin.xyz

Go:   if s == "" {}
来源：http://ssj.jinqigfzy.top

Ruby: if s.empty?
来源：http://zkz.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wig.yueranfly.top

[E21] 超长截断加省略号
来源：http://luu.bbcook.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wdg.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kjv.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://euo.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gjr.zycfv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cli.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://uyo.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sjf.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kkv.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://cfv.sufxvd.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wuc.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ney.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://smo.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hwe.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rei.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gun.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://hjo.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hiu.fktsv.cn

================================================================================
来源：http://fmc.zhiwuduotai.top

F. 文件与目录
来源：http://ofh.chenzaomai.com

================================================================================
来源：http://wid.c1oappe.top

[F01] 读取整个文件
来源：http://hxp.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kol.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://ezb.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iwg.sjlbkw.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gzf.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cqs.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nmp.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://ulm.yanxiufei.cn

C#:   File.ReadAllText("a.txt");
来源：http://oun.epnwcf.com

[F02] 逐行读取文件
来源：http://rpr.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fde.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://swe.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vim.zdqjudy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kuz.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tff.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rrm.hammf.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qgl.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://isg.meibo888.top

[F03] 写入文件（覆盖）
来源：http://nwm.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ycz.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://itf.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://htg.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zwa.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ouo.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sbj.xingfuxueyuan.xyz

Ruby: File.write("a.txt", "hi")
来源：http://seo.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bje.hnxiangtu.top

[F04] 追加写入文件
来源：http://jea.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vwg.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wfj.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tti.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nvh.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bay.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fjt.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lwz.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jdb.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://ote.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wqh.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://mrd.zhaomingkeji.xyz

JS:   fs.existsSync("a.txt")
来源：http://xjm.gaohongyu789.top

TS:   fs.existsSync("a.txt")
来源：http://epw.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xmw.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pzx.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://enx.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://edn.redwolf501.top

[F06] 删除文件
来源：http://jef.epnwcf.com

Py:   os.remove("a.txt")
来源：http://xzt.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://knv.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://xvt.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://fki.snrcjt.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gqc.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://qcy.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://nvz.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://mmc.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://gur.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bab.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://khx.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ijf.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hpz.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xmc.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kxm.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gty.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lck.yongpay.top

[F08] 遍历目录
来源：http://wnc.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jln.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://txk.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://fay.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://fts.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tmh.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qkd.fzhhl.top

Ruby: Dir.children("dir")
来源：http://rvs.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://cao.jinghuilouyu.cn

[F09] 获取文件大小
来源：http://qlv.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://gps.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://dwt.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://ymp.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://cuv.vehdjk.com

Java: Files.size(Path.of("a.txt"))
来源：http://qmj.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vkk.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://skp.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://lqw.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://gvd.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lor.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dqv.ppjwa.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zrp.epnwcf.com

TS:   path.extname("a.txt")
来源：http://gfa.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kcj.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bxi.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gqw.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://czg.yongpay.top

[F11] 复制与移动文件
来源：http://cdr.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wkc.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iyr.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jpj.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sxy.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tts.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vsy.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nqe.zycfv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://daw.hnxiangtu.top

[F12] CSV 读写
来源：http://qps.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tuy.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nii.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xtn.sxryk.cn

TS:   // 同上
来源：http://ubb.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mha.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lvl.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ynm.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vgg.ppjwa.cn

================================================================================
来源：http://agq.cashguo.top

G. 面向对象
来源：http://rbc.snrcjt.cn

================================================================================
来源：http://uoc.aizwys.cn

[G01] 定义类
来源：http://qkd.aibaodan.cn

Py:   class User: pass
来源：http://vpc.chenjidiqi.icu

PHP:  class User {}
来源：http://zfj.andypj.xyz

JS:   class User {}
来源：http://izq.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://tts.redwolf501.top

Java: class User {}
来源：http://yyb.9152youxi.cn

Go:   type User struct { Name string }
来源：http://rul.chenlongwang.top

Ruby: class User; end
来源：http://dbd.fktsv.cn

C#:   class User {}
来源：http://uet.fehbvm.com

[G02] 构造函数
来源：http://gne.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://mxd.pycfn.com

PHP:  public function __construct(public string $name) {}
来源：http://bhi.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://qsb.tarul.cn

TS:   constructor(public name: string) {}
来源：http://hmd.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://hlf.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tyq.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ium.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://ltf.xuanzx.com

[G03] 实例属性
来源：http://rlr.hnxiangtu.top

Py:   self.name = "x"
来源：http://zzc.zdbjq.cn

PHP:  public string $name = "x";
来源：http://syd.hongshengwenyu.top

JS:   this.name = "x";
来源：http://dgp.nwbrower.top

TS:   name: string = "x";
来源：http://tuz.meibo888.top

Java: private String name;
来源：http://yiv.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dmp.hnqzz.top

Ruby: @name = "x"
来源：http://thv.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://bqd.birdmap.top

[G04] 定义方法
来源：http://xbn.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://gfy.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://abi.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://rax.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://qyh.xylfe.cn

Java: String greet() { return name; }
来源：http://jqy.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wir.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://waz.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://kub.yfazqb.com

[G05] 继承
来源：http://bka.haohaochexian.top

Py:   class Admin(User): pass
来源：http://fng.sweek.top

PHP:  class Admin extends User {}
来源：http://mll.jiagoushi.top

JS:   class Admin extends User {}
来源：http://oor.yangfankeji.com

TS:   class Admin extends User {}
来源：http://fhi.guannengcc.top

Java: class Admin extends User {}
来源：http://elt.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gqe.hesvh.cn

Ruby: class Admin < User; end
来源：http://eqq.sjlbkw.cn

C#:   class Admin : User {}
来源：http://wrb.zhoulong.xyz

[G06] 重写方法
来源：http://hcl.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://iuk.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tkp.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://dyo.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://rdy.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://kfj.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://utb.tarul.cn

Ruby: def greet; "admin"; end
来源：http://gwm.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://ypj.jinqigufen.top

[G07] 调用父类方法
来源：http://mwy.shangyingyoupin.top

Py:   super().greet()
来源：http://cxd.havefunace.top

PHP:  parent::greet();
来源：http://vdn.hnqzz.top

JS:   super.greet();
来源：http://scq.0kj1m.cn

TS:   super.greet();
来源：http://uuo.nanxinkj.top

Java: super.greet();
来源：http://scj.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pzt.uphjek.com

Ruby: super
来源：http://stm.dianchejie.cn

C#:   base.Greet();
来源：http://jhv.yj20258.top

[G08] 静态方法与属性
来源：http://sju.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fyg.yongpay.top

PHP:  public static function f() {}
来源：http://vqu.zhoulong.xyz

JS:   static f() {}
来源：http://gje.chenjidiqi.icu

TS:   static f(): void {}
来源：http://yli.kuanghao11.cn

Java: static void f() {}
来源：http://zvc.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eem.zdbjq.cn

Ruby: def self.f; end
来源：http://afv.gzhubu.top

C#:   public static void F() {}
来源：http://bxm.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://uhn.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://pkm.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ntu.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dhk.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://vjz.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://gnq.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://bpr.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gfp.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://ssz.zdbjq.cn

[G10] 访问控制
来源：http://sep.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://hei.guannengcc.top

PHP:  public / protected / private
来源：http://nwf.tanke756.top

JS:   #private 字段；其余公开
来源：http://eex.gotoacloud.top

TS:   public / protected / private
来源：http://xzo.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://vfb.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lhc.nwbrower.top

Ruby: public / protected / private
来源：http://uid.iojbl.cn

C#:   public / protected / private / internal
来源：http://unu.daxiang520.top

[G11] getter / setter
来源：http://bsx.guannengcc.top

Py:   @property 与 @x.setter
来源：http://mgt.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://npc.hesvh.cn

JS:   get name() { return this._name; }
来源：http://viu.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://tol.cucudq.cn

Java: public String getName() { return name; }
来源：http://yjs.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lyf.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://ylp.yueranfly.top

C#:   public string Name { get; set; }
来源：http://ttd.jinqigfzy.top

[G12] 对象转字符串
来源：http://wmb.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://mww.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://twj.havefunace.top

JS:   toString() { return this.name; }
来源：http://oyx.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://ctl.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://mio.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://azk.yueranfly.top

Ruby: def to_s; @name; end
来源：http://qek.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://kri.yvedp.cn

[G13] 判断对象类型
来源：http://gmo.bbcook.cn

Py:   isinstance(u, User)
来源：http://wjh.yanxiufei.cn

PHP:  $u instanceof User
来源：http://zsu.shanyushiyangtech.top

JS:   u instanceof User
来源：http://pch.dianchejie.cn

TS:   u instanceof User
来源：http://bmj.pengpengdd.cyou

Java: u instanceof User
来源：http://gzy.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rld.c1oappe.top

Ruby: u.is_a?(User)
来源：http://tip.ppjwa.cn

C#:   u is User
来源：http://oao.0kj1m.cn

[G14] 数据类 / record
来源：http://yif.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://svy.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://gpy.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://lzx.svipenyu.cn

TS:   type User = { name: string; age: number };
来源：http://zqq.nwbrower.top

Java: record User(String name, int age) {}
来源：http://rmk.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://rbm.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nyu.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://gnf.yuxming.cn

[G15] 枚举
来源：http://blq.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tvc.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mdb.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dfz.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mpi.jqgfzy.top

Java: enum Color { RED, GREEN }
来源：http://ciq.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lkj.ydjk.org.cn

Ruby: Color = %i[red green].freeze
来源：http://ibo.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cxv.shanyushiyangtech.top

[G16] 对象转数组 / 字典
来源：http://xpn.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gaw.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://nww.hnqzz.top

JS:   Object.entries(obj)
来源：http://exx.bjfxy.top

TS:   Object.entries(obj)
来源：http://tgy.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rmh.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://twr.bbcook.cn

Ruby: obj.instance_variables
来源：http://faw.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://ltm.ybcxt.top

================================================================================
来源：http://sgg.cqqwz.cn

H. 异常与错误处理
来源：http://kee.andypj.xyz

================================================================================
来源：http://ipo.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://qps.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ejp.316326.xyz


<!-- 参考信息 -->