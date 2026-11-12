代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bdy.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://lle.guowangkeji.top

Py:   s.splitlines()
来源：http://nra.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://puc.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://lqh.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://mkz.hongshengwenyu.top

Java: s.lines().toList()
来源：http://zgh.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://jtx.jqgfzy.top

Ruby: s.lines
来源：http://nur.svipenyu.cn

C#:   s.Split('\n')
来源：http://twe.uphjek.com

[E20] 判断字符串是否为空
来源：http://zni.zhengqikj.top

Py:   if not s:
来源：http://lhg.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nsw.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uxk.jqgufenzy.top

TS:   if (s === "") {}
来源：http://bmv.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://gwy.uphjek.com

Go:   if s == "" {}
来源：http://fnt.cheryme.top

Ruby: if s.empty?
来源：http://sww.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qsb.yongpay.top

[E21] 超长截断加省略号
来源：http://cbc.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wfp.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ccj.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qln.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jls.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rqr.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://idh.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fnf.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gxi.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://yvl.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wwi.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zxd.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dns.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aif.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fvh.ywan-chungtsiang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eeo.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://loi.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qgs.cheryme.top

================================================================================
来源：http://lev.chenzaomai.com

F. 文件与目录
来源：http://ugf.ppjwa.cn

================================================================================
来源：http://wuz.zycfv.cn

[F01] 读取整个文件
来源：http://gvu.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://olo.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://oql.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bse.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://utw.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sux.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lhx.bbcook.cn

Ruby: File.read("a.txt")
来源：http://uls.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://nye.tanke756.top

[F02] 逐行读取文件
来源：http://xqr.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nnk.tianlin.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mby.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lfp.ywan-chungtsiang.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ooi.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dkz.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vny.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kat.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nnw.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://oow.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mpp.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://fcf.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iro.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jee.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bzx.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ghm.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://now.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bvw.shzxlz.cn

[F04] 追加写入文件
来源：http://nod.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zda.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nuc.shuidangran.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ntx.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rnk.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iqd.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lfw.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cpv.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://opu.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://cog.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wjd.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://rfm.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://rof.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://rqf.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mox.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hto.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://rim.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://fyu.gotoacloud.top

[F06] 删除文件
来源：http://wxp.316326.xyz

Py:   os.remove("a.txt")
来源：http://imn.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://xlz.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://ecb.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ria.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wcg.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://icc.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://xyj.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://ehu.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://drx.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://czl.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ghc.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iaz.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://isd.daria6918.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pfs.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gye.hysaishi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mgj.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yek.gogol.net.cn

[F08] 遍历目录
来源：http://kwx.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vnl.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bhl.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://xff.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://smb.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sln.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://udx.hcnkem.com

Ruby: Dir.children("dir")
来源：http://qun.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://qnl.fktsv.cn

[F09] 获取文件大小
来源：http://gow.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://rmd.aizwys.cn

PHP:  filesize("a.txt");
来源：http://zmo.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://pqi.haohaochexian.top

TS:   fs.statSync("a.txt").size
来源：http://app.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://znq.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gth.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://uam.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://abh.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://glk.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://twq.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dvi.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ehp.sjlbkw.cn

TS:   path.extname("a.txt")
来源：http://cug.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lnx.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mqw.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pyr.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ini.tianlin.xyz

[F11] 复制与移动文件
来源：http://pby.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ckl.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ntg.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://swy.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wtb.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zfc.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zrx.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hph.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gct.dashuyun.cn

[F12] CSV 读写
来源：http://vkb.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hgh.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hzt.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dqw.ydzc1.top

TS:   // 同上
来源：http://pxk.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mzd.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xvn.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xma.gaohongyu789.top

C#:   // 无内置：用 CsvHelper 库
来源：http://euv.jinqigfzy.top

================================================================================
来源：http://ybv.shanyushiyangkeji.top

G. 面向对象
来源：http://jtc.ydzc1.top

================================================================================
来源：http://nps.yfazqb.com

[G01] 定义类
来源：http://cav.quarkkingdee.top

Py:   class User: pass
来源：http://vrt.jyoumei.cn

PHP:  class User {}
来源：http://kfc.hnxiangtu.top

JS:   class User {}
来源：http://fwm.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://zth.nwbrower.top

Java: class User {}
来源：http://alj.tanke756.top

Go:   type User struct { Name string }
来源：http://gry.quarkkingdee.top

Ruby: class User; end
来源：http://eyq.52xcode.cn

C#:   class User {}
来源：http://hlm.yuanzhike.top

[G02] 构造函数
来源：http://mzp.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://hvk.snrcjt.cn

PHP:  public function __construct(public string $name) {}
来源：http://ifz.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://aau.fzhhl.top

TS:   constructor(public name: string) {}
来源：http://eph.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://ykr.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bad.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://qsa.dianchejie.cn

C#:   public User(string name) { Name = name; }
来源：http://yor.jinqigufen.top

[G03] 实例属性
来源：http://faa.jinqigfzy.top

Py:   self.name = "x"
来源：http://fsj.zdqjudy.top

PHP:  public string $name = "x";
来源：http://bpm.jyoumei.cn

JS:   this.name = "x";
来源：http://gzu.ydjk.org.cn

TS:   name: string = "x";
来源：http://ior.tarul.cn

Java: private String name;
来源：http://lgr.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ykr.ivvv.top

Ruby: @name = "x"
来源：http://knl.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://qna.dianchejie.cn

[G04] 定义方法
来源：http://vpm.chenjidiqi.icu

Py:   def greet(self): return self.name
来源：http://ubh.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ozq.hesvh.cn

JS:   greet() { return this.name; }
来源：http://vjr.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://elv.jiagoushi.top

Java: String greet() { return name; }
来源：http://lcw.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tjz.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://dyn.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://vgl.zhaomingkeji.xyz

[G05] 继承
来源：http://iqa.cqqwz.cn

Py:   class Admin(User): pass
来源：http://obl.jinyuanbaomall.cn

PHP:  class Admin extends User {}
来源：http://jse.haohaochexian.top

JS:   class Admin extends User {}
来源：http://isy.guowangkeji.top

TS:   class Admin extends User {}
来源：http://jxh.yongpay.top

Java: class Admin extends User {}
来源：http://jlx.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xjn.nwbrower.top

Ruby: class Admin < User; end
来源：http://zrd.aizwys.cn

C#:   class Admin : User {}
来源：http://xqi.snrcjt.cn

[G06] 重写方法
来源：http://jpc.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://ams.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vfa.pycfn.com

JS:   greet() { return "admin"; }
来源：http://opt.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://wsn.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://mkp.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dth.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://wfj.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://njk.guowangkeji.top

[G07] 调用父类方法
来源：http://kqo.birdmap.top

Py:   super().greet()
来源：http://sdm.chenzaomai.com

PHP:  parent::greet();
来源：http://ntp.zhongyouzk.top

JS:   super.greet();
来源：http://fch.yuxming.cn

TS:   super.greet();
来源：http://bxx.bjfxy.top

Java: super.greet();
来源：http://qry.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ded.jianghu66.top

Ruby: super
来源：http://dhk.snrcjt.cn

C#:   base.Greet();
来源：http://fxg.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://sjd.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ebg.zhoulong.xyz

PHP:  public static function f() {}
来源：http://xxp.svipenyu.cn

JS:   static f() {}
来源：http://rxh.daria6918.cn

TS:   static f(): void {}
来源：http://wrg.zycfv.cn

Java: static void f() {}
来源：http://jyy.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mnw.zhiwuduotai.top

Ruby: def self.f; end
来源：http://cbv.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://yol.fengsongda.top

[G09] 接口 / 抽象类
来源：http://llb.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://ysh.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://crq.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qgb.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://tcc.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://yia.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://nde.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vpp.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://ctk.shuidangran.top

[G10] 访问控制
来源：http://yru.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://rad.fengsongda.top

PHP:  public / protected / private
来源：http://eua.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://kum.zhiwuduotai.top

TS:   public / protected / private
来源：http://awh.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://syn.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wtp.mhx1999.top

Ruby: public / protected / private
来源：http://yji.ivvv.top

C#:   public / protected / private / internal
来源：http://vkz.havefunace.top

[G11] getter / setter
来源：http://sua.andypj.xyz

Py:   @property 与 @x.setter
来源：http://ejd.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pat.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://vck.sweek.top

TS:   get name(): string { return this._name; }
来源：http://igw.zhengqikj.top

Java: public String getName() { return name; }
来源：http://pbo.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wgo.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://hqz.xuanzx.com

C#:   public string Name { get; set; }
来源：http://ozk.jianghu66.top

[G12] 对象转字符串
来源：http://ydx.tarul.cn

Py:   def __str__(self): return self.name
来源：http://rqs.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://msz.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://imk.jinqigufen.top

TS:   toString(): string { return this.name; }
来源：http://cfu.tanke756.top

Java: @Override public String toString() { return name; }
来源：http://csg.yangfankeji.com

Go:   func (u User) String() string { return u.Name }
来源：http://yhl.smart0.xyz

Ruby: def to_s; @name; end
来源：http://twv.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://xmh.0kj1m.cn

[G13] 判断对象类型
来源：http://zco.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://pxf.shangyingyoupin.top

PHP:  $u instanceof User
来源：http://mmr.jinghuilouyu.cn

JS:   u instanceof User
来源：http://nuo.316326.xyz

TS:   u instanceof User
来源：http://nfs.xuetiantiany.cn

Java: u instanceof User
来源：http://bag.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wja.ydzc1.top

Ruby: u.is_a?(User)
来源：http://lol.zdqjudy.top

C#:   u is User
来源：http://ere.iojbl.cn

[G14] 数据类 / record
来源：http://bdl.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ntw.xinyue.icu

PHP:  // 用 readonly 属性模拟
来源：http://erx.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://dhp.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://qcu.ehwqpu.com

Java: record User(String name, int age) {}
来源：http://rtm.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://hry.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zbj.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://ljs.nwbrower.top

[G15] 枚举
来源：http://xbk.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gzm.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://goc.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lfl.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://age.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://lbh.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ntm.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://pbi.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xok.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://syj.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mnf.uphjek.com

PHP:  get_object_vars($obj);
来源：http://wrw.zhengqikj.top

JS:   Object.entries(obj)
来源：http://brq.cheryme.top

TS:   Object.entries(obj)
来源：http://ojq.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nux.yj202588.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qjd.bbcook.cn

Ruby: obj.instance_variables
来源：http://gjg.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://jhc.ctjpmb.com

================================================================================
来源：http://jgp.vehdjk.com

H. 异常与错误处理
来源：http://sba.chenzaomai.com

================================================================================
来源：http://paa.snrcjt.cn

[H01] try / catch 基础
来源：http://laq.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kct.sweek.top


<!-- 参考信息 -->