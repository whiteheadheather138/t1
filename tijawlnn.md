代发 wailian999

Ruby: s.lines
来源：http://vvh.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://ask.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://dtz.bjfxy.top

Py:   if not s:
来源：http://xlz.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xku.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aey.hnqzz.top

TS:   if (s === "") {}
来源：http://xwq.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://pik.jianghu66.top

Go:   if s == "" {}
来源：http://ypy.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://alb.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rlc.epnwcf.com

[E21] 超长截断加省略号
来源：http://dnb.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gxo.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ahd.ctjpmb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hdy.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nbw.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://isg.vqdsnc.cn

Go:   // 按 rune 判断长度后截断
来源：http://rkl.zhengqikj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wgi.dianchejie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nuh.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://xpk.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nnz.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uev.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tsr.cqqwz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wae.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://szn.fehbvm.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vdp.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://njy.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qgy.shanyushiyangtech.top

================================================================================
来源：http://czj.nanxuanxn.top

F. 文件与目录
来源：http://sgj.sysykeji.top

================================================================================
来源：http://acv.yj20258.top

[F01] 读取整个文件
来源：http://jue.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wdh.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://qst.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tmd.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://myt.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cgx.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bfy.xziqi.cn

Ruby: File.read("a.txt")
来源：http://fou.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://tow.fengsongda.top

[F02] 逐行读取文件
来源：http://vfr.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dlp.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xzn.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ade.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ufs.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bwt.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gav.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://srp.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kgv.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://zrs.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yqq.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://fjn.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cio.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dpc.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://csi.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lzw.uphjek.com

Ruby: File.write("a.txt", "hi")
来源：http://ozr.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xmc.tarul.cn

[F04] 追加写入文件
来源：http://nlq.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pvr.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fht.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyx.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qlc.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wbz.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ltv.gzhubu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eil.sxryk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hgh.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://xcl.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ngv.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://qnf.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://rfg.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://poy.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://guy.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nqk.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://qjo.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://hxh.hywenlv.cn

[F06] 删除文件
来源：http://anm.mhx1999.top

Py:   os.remove("a.txt")
来源：http://ebt.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://ieq.gogol.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://anp.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://zxi.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://drh.daxiang520.top

Go:   os.Remove("a.txt")
来源：http://fpx.316326.xyz

Ruby: File.delete("a.txt")
来源：http://dak.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://hje.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://vpn.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nnq.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nmk.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iqg.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ffd.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ugh.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cae.chenjidiqi.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hto.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bxq.gotoacloud.top

[F08] 遍历目录
来源：http://aqe.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ggb.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ado.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://vss.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://umy.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ngh.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lma.fengsongda.top

Ruby: Dir.children("dir")
来源：http://tcb.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://oip.meibo888.top

[F09] 获取文件大小
来源：http://nvy.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://shl.bjfxy.top

PHP:  filesize("a.txt");
来源：http://gmo.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://snw.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://kur.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://zvz.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://itx.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://yrm.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://mcf.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://atl.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uxa.ydzc1.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fhu.redwolf501.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uws.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://oaf.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ksq.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://beb.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://epx.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zqf.ivvv.top

[F11] 复制与移动文件
来源：http://gaz.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nqs.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bwe.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fow.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://krv.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rzb.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uow.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pzq.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jlo.gogol.net.cn

[F12] CSV 读写
来源：http://lua.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vwm.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hux.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fcd.xinyue.icu

TS:   // 同上
来源：http://beq.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jvi.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lqh.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qvs.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lmt.0kj1m.cn

================================================================================
来源：http://bkx.ehwqpu.com

G. 面向对象
来源：http://rqt.feifeiyinyue.top

================================================================================
来源：http://efv.yfazqb.com

[G01] 定义类
来源：http://kmp.guowangkeji.top

Py:   class User: pass
来源：http://oii.yangfankeji.com

PHP:  class User {}
来源：http://eee.vqdsnc.cn

JS:   class User {}
来源：http://brb.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://ivk.hnxiangtu.top

Java: class User {}
来源：http://chl.ybcxt.top

Go:   type User struct { Name string }
来源：http://khe.aibaodan.cn

Ruby: class User; end
来源：http://ojn.snrcjt.cn

C#:   class User {}
来源：http://xok.iojbl.cn

[G02] 构造函数
来源：http://kvd.xylfe.cn

Py:   def __init__(self, name): self.name = name
来源：http://aos.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://dkz.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://vll.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://tqx.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://bqi.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wfi.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://tnq.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://rjb.daxiang520.top

[G03] 实例属性
来源：http://ccw.ybcxt.top

Py:   self.name = "x"
来源：http://dhu.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://bmw.zhongyouzk.top

JS:   this.name = "x";
来源：http://nsh.hnqzz.top

TS:   name: string = "x";
来源：http://nxx.ctjpmb.com

Java: private String name;
来源：http://ukl.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://usb.guowangkeji.top

Ruby: @name = "x"
来源：http://xtk.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://all.nwbrower.top

[G04] 定义方法
来源：http://zoj.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://gxw.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://dun.hesvh.cn

JS:   greet() { return this.name; }
来源：http://uzi.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://iat.sjlbkw.cn

Java: String greet() { return name; }
来源：http://jjj.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://nnz.zhijiandao.cn

Ruby: def greet; @name; end
来源：http://gwk.yueranfly.top

C#:   public string Greet() => Name;
来源：http://dlt.aizwys.cn

[G05] 继承
来源：http://psv.hywenlv.cn

Py:   class Admin(User): pass
来源：http://dfg.yueranfly.top

PHP:  class Admin extends User {}
来源：http://cut.ctjpmb.com

JS:   class Admin extends User {}
来源：http://blo.bbcook.cn

TS:   class Admin extends User {}
来源：http://vtf.fehbvm.com

Java: class Admin extends User {}
来源：http://okm.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ogh.jianghu66.top

Ruby: class Admin < User; end
来源：http://qdq.9152youxi.cn

C#:   class Admin : User {}
来源：http://lat.zhiwuduotai.top

[G06] 重写方法
来源：http://npe.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://rys.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tqg.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://flz.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://mmb.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://jcp.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eci.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://kbe.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://dsv.hysaishi.cn

[G07] 调用父类方法
来源：http://qcb.zhiwuduotai.top

Py:   super().greet()
来源：http://vzd.hfpthk.cn

PHP:  parent::greet();
来源：http://qmg.jinqigfzy.top

JS:   super.greet();
来源：http://aqd.jinqigfzy.top

TS:   super.greet();
来源：http://wmv.sysykeji.top

Java: super.greet();
来源：http://yas.guowangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nqp.zhijiandao.cn

Ruby: super
来源：http://fyn.yangfankeji.com

C#:   base.Greet();
来源：http://mem.jqgfzy.top

[G08] 静态方法与属性
来源：http://rkj.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xtg.aizwys.cn

PHP:  public static function f() {}
来源：http://wrm.xinyue.icu

JS:   static f() {}
来源：http://qjq.birdmap.top

TS:   static f(): void {}
来源：http://srp.zhijiandao.cn

Java: static void f() {}
来源：http://smo.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ynl.yanxiufei.cn

Ruby: def self.f; end
来源：http://gpq.shangyingyoupin.top

C#:   public static void F() {}
来源：http://lmg.cdnleiting.top

[G09] 接口 / 抽象类
来源：http://mip.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://pmw.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tpo.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jks.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://glo.cashguo.top

Java: interface Shape { double area(); }
来源：http://nef.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://uos.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nqo.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://fzj.fanxiaobao.xyz

[G10] 访问控制
来源：http://uvp.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://txw.fehbvm.com

PHP:  public / protected / private
来源：http://yny.hesvh.cn

JS:   #private 字段；其余公开
来源：http://khn.sxryk.cn

TS:   public / protected / private
来源：http://rnp.zhaomingkeji.xyz

Java: public / protected / private / 默认包级
来源：http://jmp.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://vmx.chenzaomai.com

Ruby: public / protected / private
来源：http://rit.ehwqpu.com

C#:   public / protected / private / internal
来源：http://czo.gogol.net.cn

[G11] getter / setter
来源：http://dni.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://lxb.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yue.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://zbl.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://hao.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://ygf.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://byd.sweek.top

Ruby: attr_accessor :name
来源：http://bql.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://fug.aizwys.cn

[G12] 对象转字符串
来源：http://vgl.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://lth.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ocw.bbcook.cn

JS:   toString() { return this.name; }
来源：http://tcp.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://lnx.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://awm.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://qmz.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://csq.havefunace.top

C#:   public override string ToString() => Name;
来源：http://pux.yanxiufei.cn

[G13] 判断对象类型
来源：http://xml.gzhubu.top

Py:   isinstance(u, User)
来源：http://pjp.zhijiandao.cn

PHP:  $u instanceof User
来源：http://idf.sxryk.cn

JS:   u instanceof User
来源：http://unx.zhengqikj.top

TS:   u instanceof User
来源：http://kug.yvedp.cn

Java: u instanceof User
来源：http://tox.yueranfly.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kvg.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://llt.daria6918.cn

C#:   u is User
来源：http://lld.yfazqb.com

[G14] 数据类 / record
来源：http://hga.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rzo.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://zmh.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://yqo.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://zoy.feifeiyinyue.top

Java: record User(String name, int age) {}
来源：http://sga.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://qjg.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dzp.52xcode.cn

C#:   record User(string Name, int Age);
来源：http://tnt.sjlbkw.cn

[G15] 枚举
来源：http://woj.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://snl.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bmm.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tbk.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hip.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://qjn.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tdm.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://dep.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hgc.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://wiz.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://neo.bjfxy.top

PHP:  get_object_vars($obj);
来源：http://rcl.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://bcu.hnqzz.top

TS:   Object.entries(obj)
来源：http://eul.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eal.yvedp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kmr.xylfe.cn

Ruby: obj.instance_variables
来源：http://vns.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://smr.feifeiyinyue.top

================================================================================
来源：http://eao.hongshengwenyu.top

H. 异常与错误处理
来源：http://qtn.haohaochexian.top

================================================================================
来源：http://dzp.tianlin.xyz

[H01] try / catch 基础
来源：http://hve.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zct.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gqo.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://swr.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jfo.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kox.jinqigfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dfo.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qka.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cms.aizwys.cn

[H02] finally / ensure 收尾
来源：http://hgi.zhixingplan.top


<!-- 参考信息 -->