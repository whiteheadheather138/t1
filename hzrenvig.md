代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hcw.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tkt.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tie.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xkv.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://azy.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://pes.chenjidiqi.icu

Py:   s.splitlines()
来源：http://ixx.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hhv.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://vgi.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://fnv.sxryk.cn

Java: s.lines().toList()
来源：http://sia.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://nrv.dianchejie.cn

Ruby: s.lines
来源：http://xdv.yonumen.top

C#:   s.Split('\n')
来源：http://fbs.cashguo.top

[E20] 判断字符串是否为空
来源：http://myx.c1oappe.top

Py:   if not s:
来源：http://cwu.hesvh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://meh.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ovj.cheryme.top

TS:   if (s === "") {}
来源：http://eqs.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://kje.nwbrower.top

Go:   if s == "" {}
来源：http://xqb.wangdashe.top

Ruby: if s.empty?
来源：http://smk.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ryl.cdnleiting.top

[E21] 超长截断加省略号
来源：http://lic.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uov.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kcb.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fma.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vsv.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://usq.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://xwd.xuanzx.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wpw.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qdz.yueranfly.top

[E22] 字节长度与字符长度
来源：http://ngo.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zcm.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iuh.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://obj.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ukr.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rab.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ojj.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://owk.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yss.mhx1999.top

================================================================================
来源：http://tvu.fzhhl.top

F. 文件与目录
来源：http://dvr.c1oappe.top

================================================================================
来源：http://umj.daria6918.cn

[F01] 读取整个文件
来源：http://ejz.jyoumei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wfz.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://yzw.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uza.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sfs.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tyb.epnwcf.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jvx.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://gcr.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://qen.gaohongyu789.top

[F02] 逐行读取文件
来源：http://vse.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jjs.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tmx.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://krh.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lrz.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zdn.aibaodan.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ekb.jqgfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ndw.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://snm.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://ubd.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aqq.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://taw.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xea.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xpj.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uvj.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://knt.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://qsn.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://psw.9152youxi.cn

[F04] 追加写入文件
来源：http://luo.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yqd.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cqa.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gfr.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ans.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dwk.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rqt.zhengqikj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gtx.cheryme.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://myt.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://ckk.jinyuanbaomall.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hiq.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://akp.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://xyo.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://piz.fanxiaobao.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://vwc.yonumen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ccn.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://eky.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://dzp.shanyushiyangkeji.top

[F06] 删除文件
来源：http://sqe.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://rao.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://onj.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://rxo.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kps.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qvr.sweek.top

Go:   os.Remove("a.txt")
来源：http://kht.gotoacloud.top

Ruby: File.delete("a.txt")
来源：http://osu.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://mra.yfazqb.com

[F07] 创建目录（含多级）
来源：http://exl.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xok.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://meh.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hfy.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sxp.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hgu.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uzm.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hjg.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ljl.0kj1m.cn

[F08] 遍历目录
来源：http://knk.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yjw.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uku.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://bjb.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://nfl.jqgfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bvx.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ewc.yj20258888.top

Ruby: Dir.children("dir")
来源：http://qeq.yuanzhike.top

C#:   Directory.GetFiles("dir")
来源：http://vcb.ydjk.org.cn

[F09] 获取文件大小
来源：http://ujt.shzxlz.cn

Py:   os.path.getsize("a.txt")
来源：http://tju.yueranfly.top

PHP:  filesize("a.txt");
来源：http://odj.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://idl.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://dry.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://huu.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hsl.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://rgb.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://rxa.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ibx.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pnv.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://emf.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://taq.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://fli.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cbl.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://chq.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wtf.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nwo.aibaodan.cn

[F11] 复制与移动文件
来源：http://wwk.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lau.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pke.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://saw.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wij.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zfn.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rti.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://foa.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bvy.shuidangran.top

[F12] CSV 读写
来源：http://cwj.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dmr.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gyh.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zve.gaohongyu789.top

TS:   // 同上
来源：http://ide.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zpc.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xrb.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uxf.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bdx.52xcode.cn

================================================================================
来源：http://vyc.bbcook.cn

G. 面向对象
来源：http://nag.ydzc1.top

================================================================================
来源：http://wuc.dashuyun.cn

[G01] 定义类
来源：http://pwm.hfpthk.cn

Py:   class User: pass
来源：http://wur.hysaishi.cn

PHP:  class User {}
来源：http://czb.ctjpmb.com

JS:   class User {}
来源：http://ryu.yongpay.top

TS:   class User { name: string = ""; }
来源：http://kjq.yvedp.cn

Java: class User {}
来源：http://wqx.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://hdj.yangfankeji.com

Ruby: class User; end
来源：http://ffa.yuanzhike.top

C#:   class User {}
来源：http://chq.yj20258.top

[G02] 构造函数
来源：http://ydu.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://hok.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://wwd.fengsongda.top

JS:   constructor(name) { this.name = name; }
来源：http://fpl.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://jyc.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://rwj.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zsb.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://pfp.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://ymh.tanke756.top

[G03] 实例属性
来源：http://wiv.xinyue.icu

Py:   self.name = "x"
来源：http://vct.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://wur.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://bak.zhengqikj.top

TS:   name: string = "x";
来源：http://tnm.hongshengwenyu.top

Java: private String name;
来源：http://xyd.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nhb.zhengqikj.top

Ruby: @name = "x"
来源：http://tdb.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://hkh.cqqwz.cn

[G04] 定义方法
来源：http://qmc.chenjidiqi.icu

Py:   def greet(self): return self.name
来源：http://poa.zhongyouzk.top

PHP:  public function greet(): string { return $this->name; }
来源：http://npp.fehbvm.com

JS:   greet() { return this.name; }
来源：http://txv.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://kml.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://wvy.ywan-chungtsiang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fgx.yfazqb.com

Ruby: def greet; @name; end
来源：http://zyk.shuidangran.top

C#:   public string Greet() => Name;
来源：http://vke.havefunace.top

[G05] 继承
来源：http://bpg.tian-w.cn

Py:   class Admin(User): pass
来源：http://jfr.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://rmz.haohaochexian.top

JS:   class Admin extends User {}
来源：http://ptw.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://pmp.jiagoushi.top

Java: class Admin extends User {}
来源：http://elk.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vpr.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://tgr.aizwys.cn

C#:   class Admin : User {}
来源：http://uwf.0kj1m.cn

[G06] 重写方法
来源：http://mkl.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://tjc.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://roa.ivvv.top

JS:   greet() { return "admin"; }
来源：http://dhy.epnwcf.com

TS:   greet(): string { return "admin"; }
来源：http://ihm.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://scu.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wmd.yongpay.top

Ruby: def greet; "admin"; end
来源：http://gbp.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://kow.ppjwa.cn

[G07] 调用父类方法
来源：http://umh.feifeiyinyue.top

Py:   super().greet()
来源：http://adu.gogol.net.cn

PHP:  parent::greet();
来源：http://uyj.hongshengwenyu.top

JS:   super.greet();
来源：http://fld.jinghuilouyu.cn

TS:   super.greet();
来源：http://doc.zhoulong.xyz

Java: super.greet();
来源：http://vhc.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kwh.hesvh.cn

Ruby: super
来源：http://bid.ctjpmb.com

C#:   base.Greet();
来源：http://poq.yj20258.top

[G08] 静态方法与属性
来源：http://xup.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eyo.sjlbkw.cn

PHP:  public static function f() {}
来源：http://ddt.hnxiangtu.top

JS:   static f() {}
来源：http://oxk.zhengqikj.top

TS:   static f(): void {}
来源：http://jea.ivvv.top

Java: static void f() {}
来源：http://kes.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ywo.hesvh.cn

Ruby: def self.f; end
来源：http://uyx.vehdjk.com

C#:   public static void F() {}
来源：http://cpg.ybcxt.top

[G09] 接口 / 抽象类
来源：http://nwe.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://qmu.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://yvx.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jbb.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://exg.guannengcc.top

Java: interface Shape { double area(); }
来源：http://iri.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://jft.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yfx.dashuyun.cn

C#:   interface IShape { double Area(); }
来源：http://hit.hnqzz.top

[G10] 访问控制
来源：http://tbv.hongshengwenyu.top

Py:   约定 _protected / __private（不强制）
来源：http://bbg.chenlongwang.top

PHP:  public / protected / private
来源：http://loe.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://mlq.aibaodan.cn

TS:   public / protected / private
来源：http://xpo.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://yic.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hln.9152youxi.cn

Ruby: public / protected / private
来源：http://klb.yangfankeji.com

C#:   public / protected / private / internal
来源：http://rnc.shzxlz.cn

[G11] getter / setter
来源：http://qoy.fengsongda.top

Py:   @property 与 @x.setter
来源：http://xdy.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://upf.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://ake.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://pfs.epnwcf.com

Java: public String getName() { return name; }
来源：http://tsv.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mbn.cdnleiting.top

Ruby: attr_accessor :name
来源：http://arq.sysykeji.top

C#:   public string Name { get; set; }
来源：http://uqu.aizwys.cn

[G12] 对象转字符串
来源：http://rqz.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://ebf.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://prz.gzhubu.top

JS:   toString() { return this.name; }
来源：http://jdb.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://yln.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://pkh.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://ljs.cucudq.cn

Ruby: def to_s; @name; end
来源：http://zjj.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://ghm.ywan-chungtsiang.top

[G13] 判断对象类型
来源：http://bea.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://fyw.hesvh.cn

PHP:  $u instanceof User
来源：http://yia.ehwqpu.com

JS:   u instanceof User
来源：http://nej.tanke756.top

TS:   u instanceof User
来源：http://plb.jinqigfzy.top

Java: u instanceof User
来源：http://hhn.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nof.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://isl.meibo888.top

C#:   u is User
来源：http://dbv.nwbrower.top

[G14] 数据类 / record
来源：http://jrp.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://frj.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://wnp.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://cdk.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://vxp.hesvh.cn

Java: record User(String name, int age) {}
来源：http://bii.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://slt.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ucf.kuanghao11.cn

C#:   record User(string Name, int Age);
来源：http://haa.cheryme.top

[G15] 枚举
来源：http://dmg.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zxe.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://dpg.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ovi.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hdn.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://puv.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://szu.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://toc.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vbp.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://qsz.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://owg.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://qrx.jyoumei.cn

JS:   Object.entries(obj)
来源：http://mkb.epnwcf.com

TS:   Object.entries(obj)
来源：http://roy.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oxy.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://umw.jqgufenzy.top

Ruby: obj.instance_variables
来源：http://fnb.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://egm.shangyingyoupin.top

================================================================================
来源：http://uoi.dianchejie.cn


<!-- 参考信息 -->