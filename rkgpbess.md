代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qaa.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://saq.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lux.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://egt.shzxlz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nub.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rqw.ydjk.org.cn

[F03] 写入文件（覆盖）
来源：http://rzc.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tun.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yrp.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wye.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bhn.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://emm.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bjb.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://ycd.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cbe.cqqwz.cn

[F04] 追加写入文件
来源：http://kmj.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mzf.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://edp.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cca.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://upn.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rzi.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tvf.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fbc.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qzq.sweek.top

[F05] 判断文件或目录是否存在
来源：http://aar.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mom.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://zmx.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://lke.vqdsnc.cn

TS:   fs.existsSync("a.txt")
来源：http://rci.meibo888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fkc.ehwqpu.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vdl.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://prs.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://stx.zhiwuduotai.top

[F06] 删除文件
来源：http://cws.fzhhl.top

Py:   os.remove("a.txt")
来源：http://mfk.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://ooh.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://fso.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://yuf.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fif.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://iqg.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://ijw.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://nlw.aizwys.cn

[F07] 创建目录（含多级）
来源：http://mmu.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://glv.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tph.guowangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pya.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wmt.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kqa.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://srr.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mla.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vku.xinyue.icu

[F08] 遍历目录
来源：http://rwx.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mqp.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zsp.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://knq.aibaodan.cn

TS:   fs.readdirSync("dir")
来源：http://ugo.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lzn.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fyc.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://fql.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://pdq.shuidangran.top

[F09] 获取文件大小
来源：http://cue.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://nwu.wangdashe.top

PHP:  filesize("a.txt");
来源：http://tdr.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://xxm.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://wzp.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://pzx.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hpf.guannengcc.top

Ruby: File.size("a.txt")
来源：http://xpw.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://tzj.xinyue.icu

[F10] 取文件扩展名 / 文件名
来源：http://kkv.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uyp.kuanghao11.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://npk.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://reu.ybcxt.top

TS:   path.extname("a.txt")
来源：http://ovx.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xhg.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ngv.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://puj.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qgn.tanke756.top

[F11] 复制与移动文件
来源：http://etq.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nfg.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://epa.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wmt.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qzl.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cgr.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mpv.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aze.yanxiufei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wzf.yuxming.cn

[F12] CSV 读写
来源：http://mqh.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uba.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://day.cdnleiting.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qpz.yuanzhike.top

TS:   // 同上
来源：http://kyy.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fkl.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vno.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://off.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dlu.xinyue.icu

================================================================================
来源：http://zau.xingfuxueyuan.xyz

G. 面向对象
来源：http://sit.hongshengwenyu.top

================================================================================
来源：http://ivh.zycfv.cn

[G01] 定义类
来源：http://nxt.gotoacloud.top

Py:   class User: pass
来源：http://zgj.shangyingyoupin.top

PHP:  class User {}
来源：http://ukf.aizwys.cn

JS:   class User {}
来源：http://xzb.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://eip.jinyuanbaomall.cn

Java: class User {}
来源：http://qni.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://yfb.kuanghao11.cn

Ruby: class User; end
来源：http://wew.zhiwuduotai.top

C#:   class User {}
来源：http://mjs.svipenyu.cn

[G02] 构造函数
来源：http://urf.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://ghs.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://rhd.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://cza.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://uyf.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://vcd.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ahc.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://oob.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://fok.zhengqikj.top

[G03] 实例属性
来源：http://rxp.yueranfly.top

Py:   self.name = "x"
来源：http://txq.xylfe.cn

PHP:  public string $name = "x";
来源：http://jwn.gogol.net.cn

JS:   this.name = "x";
来源：http://dfo.sjlbkw.cn

TS:   name: string = "x";
来源：http://bne.sweek.top

Java: private String name;
来源：http://bxq.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ypr.jqgfzy.top

Ruby: @name = "x"
来源：http://dhi.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://lhc.jianghu66.top

[G04] 定义方法
来源：http://xpc.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://yvp.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://chl.cheryme.top

JS:   greet() { return this.name; }
来源：http://arb.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://voh.shuidangran.top

Java: String greet() { return name; }
来源：http://lpk.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://myq.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://epx.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://hft.yueranfly.top

[G05] 继承
来源：http://dwn.birdmap.top

Py:   class Admin(User): pass
来源：http://jym.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://snm.0kj1m.cn

JS:   class Admin extends User {}
来源：http://rbs.jianghu66.top

TS:   class Admin extends User {}
来源：http://iau.hnxiangtu.top

Java: class Admin extends User {}
来源：http://ase.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zcn.9152youxi.cn

Ruby: class Admin < User; end
来源：http://mzd.dashuyun.cn

C#:   class Admin : User {}
来源：http://vca.gzhubu.top

[G06] 重写方法
来源：http://llt.tanke756.top

Py:   def greet(self): return "admin"
来源：http://lox.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mty.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://bmz.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://gbt.daxiang520.top

Java: @Override String greet() { return "admin"; }
来源：http://kph.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://npe.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://sby.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://sbe.jyoumei.cn

[G07] 调用父类方法
来源：http://yhz.cqqwz.cn

Py:   super().greet()
来源：http://wkh.cheryme.top

PHP:  parent::greet();
来源：http://hsr.tarul.cn

JS:   super.greet();
来源：http://jyc.fehbvm.com

TS:   super.greet();
来源：http://ubd.jqgfzy.top

Java: super.greet();
来源：http://skt.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cwf.hysaishi.cn

Ruby: super
来源：http://nqq.yj20258888.top

C#:   base.Greet();
来源：http://fct.xuanzx.com

[G08] 静态方法与属性
来源：http://iri.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://syd.c1oappe.top

PHP:  public static function f() {}
来源：http://tac.cashguo.top

JS:   static f() {}
来源：http://vli.yvedp.cn

TS:   static f(): void {}
来源：http://cwc.hammf.cn

Java: static void f() {}
来源：http://yry.kuanghao11.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ajj.fzhhl.top

Ruby: def self.f; end
来源：http://shr.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://srt.fengsongda.top

[G09] 接口 / 抽象类
来源：http://rdf.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://iex.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nmw.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gfd.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://eor.andypj.xyz

Java: interface Shape { double area(); }
来源：http://eni.cashguo.top

Go:   type Shape interface { Area() float64 }
来源：http://ygi.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bbc.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://rvh.ydjk.org.cn

[G10] 访问控制
来源：http://kni.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://kkq.xylfe.cn

PHP:  public / protected / private
来源：http://ido.fehbvm.com

JS:   #private 字段；其余公开
来源：http://bbz.daxiang520.top

TS:   public / protected / private
来源：http://snd.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://yuz.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://jje.9152youxi.cn

Ruby: public / protected / private
来源：http://qez.jqgfzy.top

C#:   public / protected / private / internal
来源：http://ijx.nanxinkj.top

[G11] getter / setter
来源：http://yig.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://mrl.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://mon.gzhubu.top

JS:   get name() { return this._name; }
来源：http://xqo.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://nwt.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://aaf.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dfa.wangdashe.top

Ruby: attr_accessor :name
来源：http://prd.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://dtj.snrcjt.cn

[G12] 对象转字符串
来源：http://klm.sweek.top

Py:   def __str__(self): return self.name
来源：http://ixk.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cfr.zycfv.cn

JS:   toString() { return this.name; }
来源：http://bmj.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://ltu.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://kpu.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://ake.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://dzx.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://sah.yj20258888.top

[G13] 判断对象类型
来源：http://cwh.ehwqpu.com

Py:   isinstance(u, User)
来源：http://jld.c1oappe.top

PHP:  $u instanceof User
来源：http://dmc.hammf.cn

JS:   u instanceof User
来源：http://rie.yangfankeji.com

TS:   u instanceof User
来源：http://uul.daxiang520.top

Java: u instanceof User
来源：http://cwc.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ach.yueranfly.top

Ruby: u.is_a?(User)
来源：http://gch.fengsongda.top

C#:   u is User
来源：http://hyf.ydzc1.top

[G14] 数据类 / record
来源：http://bdj.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qbt.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://yve.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://jxs.nanxinkj.top

TS:   type User = { name: string; age: number };
来源：http://qwj.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://pua.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://kwh.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fol.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://tly.mhx1999.top

[G15] 枚举
来源：http://nbb.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lmb.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://loi.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xja.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hzg.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://zqh.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bwe.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://rtv.hongshengwenyu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hpd.birdmap.top

[G16] 对象转数组 / 字典
来源：http://nti.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mgw.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://big.xingfuxueyuan.xyz

JS:   Object.entries(obj)
来源：http://nmg.cashguo.top

TS:   Object.entries(obj)
来源：http://inp.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wbk.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rmp.yueranfly.top

Ruby: obj.instance_variables
来源：http://ias.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://zgf.kuanghao11.cn

================================================================================
来源：http://rml.hywenlv.cn

H. 异常与错误处理
来源：http://guk.xziqi.cn

================================================================================
来源：http://ceo.dianchejie.cn

[H01] try / catch 基础
来源：http://hdn.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ker.vehdjk.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jiz.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://urk.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://byl.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dij.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vjh.9152youxi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bli.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xus.yfazqb.com

[H02] finally / ensure 收尾
来源：http://ltl.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uni.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hvx.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wmh.haohaochexian.top

TS:   try { f(); } finally { cleanup(); }
来源：http://btt.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://ynj.ivvv.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wun.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mlj.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qik.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://xib.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://bmr.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vle.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://hci.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://nmh.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bru.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eji.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://axf.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://twy.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://poq.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://jwf.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://xyi.tian-w.cn

JS:   class MyError extends Error {}
来源：http://mwp.zycfv.cn

TS:   class MyError extends Error {}
来源：http://tcq.fehbvm.com

Java: class MyException extends RuntimeException {}
来源：http://iwk.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ahc.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://osd.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://utm.cashguo.top

[H05] 捕获特定类型
来源：http://ivx.tian-w.cn

Py:   except ValueError as e:
来源：http://lch.hnxiangtu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nja.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://rwe.aizwys.cn

TS:   if (e instanceof TypeError) {}
来源：http://nto.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://fwt.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lbn.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://edk.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hrr.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://wuz.yj20258.top

Py:   value = d.get("k") or default
来源：http://brb.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://uav.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://fwu.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://php.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dri.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hlq.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://xem.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://rhd.316326.xyz


<!-- 参考信息 -->