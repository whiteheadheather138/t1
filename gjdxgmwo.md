代发 wailian999

[F01] 读取整个文件
来源：http://fdr.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pzx.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://lol.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mqc.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pgw.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xcb.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zav.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://ilz.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://kxj.jlsjyb.cn

[F02] 逐行读取文件
来源：http://lja.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nwx.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pjo.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dwx.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lqi.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gqh.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nbn.hammf.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://urb.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rwh.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://utg.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zto.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sij.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vqf.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lau.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pxh.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://foj.316326.xyz

Ruby: File.write("a.txt", "hi")
来源：http://fox.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ovt.zhongyouzk.top

[F04] 追加写入文件
来源：http://dao.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://exk.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uuf.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fep.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iwj.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hkr.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rxr.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fjz.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ugc.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://uie.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bot.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://kka.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://vwo.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://iku.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pvv.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ppj.sjlbkw.cn

Ruby: File.exist?("a.txt")
来源：http://rld.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://cob.hfpthk.cn

[F06] 删除文件
来源：http://ywm.ivvv.top

Py:   os.remove("a.txt")
来源：http://wzs.guannengcc.top

PHP:  unlink("a.txt");
来源：http://ube.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://ugo.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://yin.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cui.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://bpe.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://etq.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://lfx.zhijiandao.cn

[F07] 创建目录（含多级）
来源：http://tuw.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sqn.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://spa.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sze.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rex.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gjg.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://duo.hesvh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mmm.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dgt.hysaishi.cn

[F08] 遍历目录
来源：http://zyq.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ybr.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://azl.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://zqj.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://bwc.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mkz.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wow.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://gcx.zhixingplan.top

C#:   Directory.GetFiles("dir")
来源：http://ufi.hnxiangtu.top

[F09] 获取文件大小
来源：http://vam.zhoulong.xyz

Py:   os.path.getsize("a.txt")
来源：http://szm.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://prt.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://jgp.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://xlq.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zwk.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://two.ivvv.top

Ruby: File.size("a.txt")
来源：http://quj.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://tgq.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://dzj.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bxx.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gqt.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ysx.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://utd.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tqf.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hhl.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://btn.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://twr.daria6918.cn

[F11] 复制与移动文件
来源：http://ptl.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hgm.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://crg.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cno.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dhx.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://muw.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://muq.wangshuangyany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://weg.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mzj.nwbrower.top

[F12] CSV 读写
来源：http://hpg.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dpx.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yww.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://evk.dashuyun.cn

TS:   // 同上
来源：http://zee.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://prs.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://glm.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yvx.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://adb.hnxiangtu.top

================================================================================
来源：http://rvv.ehwqpu.com

G. 面向对象
来源：http://cfn.xuetiantiany.cn

================================================================================
来源：http://gwn.snrcjt.cn

[G01] 定义类
来源：http://tqu.nwbrower.top

Py:   class User: pass
来源：http://inu.zycfv.cn

PHP:  class User {}
来源：http://mij.guowangkeji.top

JS:   class User {}
来源：http://zgy.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://kah.sxryk.cn

Java: class User {}
来源：http://nxj.zhaomingkeji.xyz

Go:   type User struct { Name string }
来源：http://hrz.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://egf.tian-w.cn

C#:   class User {}
来源：http://kjx.xziqi.cn

[G02] 构造函数
来源：http://ybb.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://vtf.guowangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://bar.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://bxo.ivvv.top

TS:   constructor(public name: string) {}
来源：http://jrn.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://wuj.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xlq.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://yst.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://yrb.jinqigufen.top

[G03] 实例属性
来源：http://ibh.hnqzz.top

Py:   self.name = "x"
来源：http://byn.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://sbb.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://dkh.wangdashe.top

TS:   name: string = "x";
来源：http://ztu.jlsjyb.cn

Java: private String name;
来源：http://gpq.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sib.quarkkingdee.top

Ruby: @name = "x"
来源：http://jpr.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://ftt.shuidangran.top

[G04] 定义方法
来源：http://pph.nanxinkj.top

Py:   def greet(self): return self.name
来源：http://yvy.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ipe.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://xiq.haohaochexian.top

TS:   greet(): string { return this.name; }
来源：http://ywi.tianlin.xyz

Java: String greet() { return name; }
来源：http://cqa.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pyo.gotoacloud.top

Ruby: def greet; @name; end
来源：http://qll.zycfv.cn

C#:   public string Greet() => Name;
来源：http://bgt.yuanzhike.top

[G05] 继承
来源：http://bme.sweek.top

Py:   class Admin(User): pass
来源：http://hxn.c1oappe.top

PHP:  class Admin extends User {}
来源：http://qdz.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://jjz.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://mql.jyoumei.cn

Java: class Admin extends User {}
来源：http://swr.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kth.sxryk.cn

Ruby: class Admin < User; end
来源：http://aim.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://exu.hfpthk.cn

[G06] 重写方法
来源：http://egb.tarul.cn

Py:   def greet(self): return "admin"
来源：http://dkb.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://evp.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://urb.daria6918.cn

TS:   greet(): string { return "admin"; }
来源：http://axe.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://lqz.fehbvm.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vno.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://ypk.hnxiangtu.top

C#:   public override string Greet() => "admin";
来源：http://eui.ybcxt.top

[G07] 调用父类方法
来源：http://vbg.uphjek.com

Py:   super().greet()
来源：http://ccz.gaohongyu789.top

PHP:  parent::greet();
来源：http://lzu.chenzaomai.com

JS:   super.greet();
来源：http://xbs.fehbvm.com

TS:   super.greet();
来源：http://dnd.tian-w.cn

Java: super.greet();
来源：http://tsj.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ddv.nanxinkj.top

Ruby: super
来源：http://cfu.ybcxt.top

C#:   base.Greet();
来源：http://ena.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://ydj.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gcb.shzxlz.cn

PHP:  public static function f() {}
来源：http://ykj.wangdashe.top

JS:   static f() {}
来源：http://ppr.tian-w.cn

TS:   static f(): void {}
来源：http://fkv.chenlongwang.top

Java: static void f() {}
来源：http://yfo.pengpengdd.cyou

Go:   // 无 static：用包级函数，按包名调用
来源：http://vvk.sxryk.cn

Ruby: def self.f; end
来源：http://vjd.cheryme.top

C#:   public static void F() {}
来源：http://frt.cdnleiting.top

[G09] 接口 / 抽象类
来源：http://pwy.andypj.xyz

Py:   from abc import ABC, abstractmethod
来源：http://bya.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://vti.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://wvj.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://isj.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://mlx.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://iav.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mun.ydjk.org.cn

C#:   interface IShape { double Area(); }
来源：http://qpu.hysaishi.cn

[G10] 访问控制
来源：http://koa.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://iru.zdqjudy.top

PHP:  public / protected / private
来源：http://gux.yfazqb.com

JS:   #private 字段；其余公开
来源：http://epv.fengsongda.top

TS:   public / protected / private
来源：http://wfb.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://lfs.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://eow.zdbjq.cn

Ruby: public / protected / private
来源：http://wfz.vehdjk.com

C#:   public / protected / private / internal
来源：http://pho.jinyuanbaomall.cn

[G11] getter / setter
来源：http://tkr.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://rdb.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zii.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://mfc.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://isn.mhx1999.top

Java: public String getName() { return name; }
来源：http://ygp.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tcs.smart0.xyz

Ruby: attr_accessor :name
来源：http://xrh.hnqzz.top

C#:   public string Name { get; set; }
来源：http://ywd.hysaishi.cn

[G12] 对象转字符串
来源：http://qtd.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://uls.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xnv.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://nbl.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://fjt.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://qnk.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://kzr.cucudq.cn

Ruby: def to_s; @name; end
来源：http://juc.shzxlz.cn

C#:   public override string ToString() => Name;
来源：http://qew.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://sbr.jiagoushi.top

Py:   isinstance(u, User)
来源：http://npa.zhengqikj.top

PHP:  $u instanceof User
来源：http://esb.hnqzz.top

JS:   u instanceof User
来源：http://dqh.zycfv.cn

TS:   u instanceof User
来源：http://wcr.fehbvm.com

Java: u instanceof User
来源：http://dvp.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jkr.bbcook.cn

Ruby: u.is_a?(User)
来源：http://xgq.sxryk.cn

C#:   u is User
来源：http://lzk.sxryk.cn

[G14] 数据类 / record
来源：http://kgg.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ghh.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://apj.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://klp.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://wrv.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://ytu.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://ogl.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ina.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://cso.gzhubu.top

[G15] 枚举
来源：http://euv.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vvk.zhixingplan.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ycv.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jae.xylfe.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://adn.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://xrz.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tcm.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://scp.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tro.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://dip.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lcr.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://lef.jinqigufen.top

JS:   Object.entries(obj)
来源：http://spu.epnwcf.com

TS:   Object.entries(obj)
来源：http://jhm.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cuo.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gni.cqqwz.cn

Ruby: obj.instance_variables
来源：http://bom.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://dld.chenjidiqi.icu

================================================================================
来源：http://lto.meibo888.top

H. 异常与错误处理
来源：http://chi.kuanghao11.cn

================================================================================
来源：http://hjz.aibaodan.cn

[H01] try / catch 基础
来源：http://wyb.andypj.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gji.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eab.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fbm.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xub.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rmr.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://szw.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kwj.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://syt.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://ryo.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dsr.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gel.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hkb.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jjz.sxryk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fch.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gbz.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dvm.vehdjk.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://kyn.tarul.cn

[H03] 主动抛出异常
来源：http://thv.sweek.top

Py:   raise ValueError("错误信息")
来源：http://tlo.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://taj.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://tfh.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://fwn.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qit.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hhg.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pdb.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://lfd.9152youxi.cn

[H04] 自定义异常类型
来源：http://qek.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://lhq.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://iek.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://ula.yongpay.top

TS:   class MyError extends Error {}
来源：http://ros.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://nsi.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bch.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://aph.daxiang520.top

C#:   class MyException : Exception {}
来源：http://nkp.mhx1999.top

[H05] 捕获特定类型
来源：http://okj.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://lnj.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pso.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://zjn.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ksu.jlsjyb.cn

Java: catch (IOException | SQLException e) {}
来源：http://tla.hcnkem.com


<!-- 参考信息 -->