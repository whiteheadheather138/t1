代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：https://pp.zhonguo4118.cn

Java: Files.readString(Path.of("a.txt"))
来源：https://wj.zhonguo2118.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：https://lo.zhonguo6118.cn

Ruby: File.read("a.txt")
来源：https://vj.zhonguo8118.cn

C#:   File.ReadAllText("a.txt");
来源：https://kb.zhonguo4118.cn

[F02] 逐行读取文件
来源：https://kw.zhonguo4118.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：https://db.zhonguo1118.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：https://rb.zhonguo6118.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://mn.zhonguo6118.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：https://ou.zhonguo7118.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：https://ul.zhonguo8118.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：https://ns.zhonguo5118.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://ql.zhonguo2118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://xw.zhonguo6118.cn

[F03] 写入文件（覆盖）
来源：https://ad.zhonguo2118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://ra.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://cy.zhonguo7118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://fn.zhonguo8118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ar.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://xz.zhonguo5118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://yi.zhonguo8118.cn

Ruby: File.write("a.txt", "hi")
来源：https://tj.zhonguo4118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://ig.zhonguo5118.cn

[F04] 追加写入文件
来源：https://ug.zhonguo3118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://fe.zhonguo6118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://nk.zhonguo1118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://gf.zhonguo3118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://lx.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://he.zhonguo7118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://xc.zhonguo3118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://ki.zhonguo3118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://rr.zhonguo3118.cn

[F05] 判断文件或目录是否存在
来源：https://ja.zhonguo5118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://ct.zhonguo2118.cn

PHP:  file_exists("a.txt");
来源：https://ss.zhonguo3118.cn

JS:   fs.existsSync("a.txt")
来源：https://sp.zhonguo2118.cn

TS:   fs.existsSync("a.txt")
来源：https://py.zhonguo8118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://ws.zhonguo7118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://ex.zhonguo8118.cn

Ruby: File.exist?("a.txt")
来源：https://lm.zhonguo4118.cn

C#:   File.Exists("a.txt")
来源：https://bf.zhonguo4118.cn

[F06] 删除文件
来源：https://oh.zhonguo3118.cn

Py:   os.remove("a.txt")
来源：https://ms.zhonguo1118.cn

PHP:  unlink("a.txt");
来源：https://ii.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://zh.zhonguo2118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://eu.zhonguo7118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://uc.zhonguo1118.cn

Go:   os.Remove("a.txt")
来源：https://an.zhonguo6118.cn

Ruby: File.delete("a.txt")
来源：https://aw.zhonguo4118.cn

C#:   File.Delete("a.txt");
来源：https://jk.zhonguo5118.cn

[F07] 创建目录（含多级）
来源：https://wr.zhonguo1118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://km.zhonguo3118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://eb.zhonguo7118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://hq.zhonguo8118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://py.zhonguo1118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://fk.zhonguo1118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://mh.zhonguo8118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://ea.zhonguo1118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://uu.zhonguo6118.cn

[F08] 遍历目录
来源：https://ox.zhonguo6118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://je.zhonguo4118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://jh.zhonguo8118.cn

JS:   fs.readdirSync("dir")
来源：https://qc.zhonguo1118.cn

TS:   fs.readdirSync("dir")
来源：https://td.zhonguo7118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://ai.zhonguo8118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://hi.zhonguo2118.cn

Ruby: Dir.children("dir")
来源：https://uh.zhonguo8118.cn

C#:   Directory.GetFiles("dir")
来源：https://ol.zhonguo2118.cn

[F09] 获取文件大小
来源：https://vx.zhonguo3118.cn

Py:   os.path.getsize("a.txt")
来源：https://af.zhonguo2118.cn

PHP:  filesize("a.txt");
来源：https://cm.zhonguo7118.cn

JS:   fs.statSync("a.txt").size
来源：https://zl.zhonguo5118.cn

TS:   fs.statSync("a.txt").size
来源：https://rx.zhonguo7118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://tj.zhonguo2118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://lg.zhonguo2118.cn

Ruby: File.size("a.txt")
来源：https://xp.zhonguo6118.cn

C#:   new FileInfo("a.txt").Length
来源：https://be.zhonguo3118.cn

[F10] 取文件扩展名 / 文件名
来源：https://aa.zhonguo7118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://aw.zhonguo2118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://lr.zhonguo7118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://am.zhonguo6118.cn

TS:   path.extname("a.txt")
来源：https://kz.zhonguo5118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://tc.zhonguo3118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://vx.zhonguo2118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://dg.zhonguo1118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://op.zhonguo7118.cn

[F11] 复制与移动文件
来源：https://wu.zhonguo8118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://yk.zhonguo2118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://mr.zhonguo7118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ke.zhonguo4118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ba.zhonguo2118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://io.zhonguo5118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://fu.zhonguo5118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://ru.zhonguo6118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://lt.zhonguo3118.cn

[F12] CSV 读写
来源：https://kf.zhonguo2118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://zi.zhonguo6118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://dt.zhonguo2118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://pu.zhonguo2118.cn

TS:   // 同上
来源：https://mx.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://ox.zhonguo4118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://nx.zhonguo5118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://th.zhonguo3118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://ba.zhonguo8118.cn

================================================================================
来源：https://nw.zhonguo2118.cn

G. 面向对象
来源：https://qv.zhonguo4118.cn

================================================================================
来源：https://vq.zhonguo4118.cn

[G01] 定义类
来源：https://ns.zhonguo2118.cn

Py:   class User: pass
来源：https://xl.zhonguo1118.cn

PHP:  class User {}
来源：https://ud.zhonguo1118.cn

JS:   class User {}
来源：https://zg.zhonguo7118.cn

TS:   class User { name: string = ""; }
来源：https://vm.zhonguo2118.cn

Java: class User {}
来源：https://lh.zhonguo4118.cn

Go:   type User struct { Name string }
来源：https://ia.zhonguo4118.cn

Ruby: class User; end
来源：https://ld.zhonguo7118.cn

C#:   class User {}
来源：https://bs.zhonguo3118.cn

[G02] 构造函数
来源：https://th.zhonguo2118.cn

Py:   def __init__(self, name): self.name = name
来源：https://rq.zhonguo3118.cn

PHP:  public function __construct(public string $name) {}
来源：https://kw.zhonguo1118.cn

JS:   constructor(name) { this.name = name; }
来源：https://wa.zhonguo3118.cn

TS:   constructor(public name: string) {}
来源：https://eg.zhonguo2118.cn

Java: User(String name) { this.name = name; }
来源：https://jt.zhonguo8118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://tx.zhonguo5118.cn

Ruby: def initialize(name); @name = name; end
来源：https://kw.zhonguo5118.cn

C#:   public User(string name) { Name = name; }
来源：https://jn.zhonguo8118.cn

[G03] 实例属性
来源：https://vu.zhonguo2118.cn

Py:   self.name = "x"
来源：https://vn.zhonguo4118.cn

PHP:  public string $name = "x";
来源：https://ej.zhonguo4118.cn

JS:   this.name = "x";
来源：https://fx.zhonguo3118.cn

TS:   name: string = "x";
来源：https://an.zhonguo1118.cn

Java: private String name;
来源：https://uc.zhonguo7118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://ix.zhonguo2118.cn

Ruby: @name = "x"
来源：https://gx.zhonguo5118.cn

C#:   public string Name { get; set; } = "x";
来源：https://rg.zhonguo1118.cn

[G04] 定义方法
来源：https://ba.zhonguo5118.cn

Py:   def greet(self): return self.name
来源：https://ix.zhonguo4118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://ut.zhonguo8118.cn

JS:   greet() { return this.name; }
来源：https://tz.zhonguo4118.cn

TS:   greet(): string { return this.name; }
来源：https://dp.zhonguo6118.cn

Java: String greet() { return name; }
来源：https://ls.zhonguo2118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://co.zhonguo4118.cn

Ruby: def greet; @name; end
来源：https://ik.zhonguo6118.cn

C#:   public string Greet() => Name;
来源：https://ac.zhonguo2118.cn

[G05] 继承
来源：https://qd.zhonguo4118.cn

Py:   class Admin(User): pass
来源：https://ba.zhonguo2118.cn

PHP:  class Admin extends User {}
来源：https://qh.zhonguo5118.cn

JS:   class Admin extends User {}
来源：https://fx.zhonguo8118.cn

TS:   class Admin extends User {}
来源：https://rs.zhonguo2118.cn

Java: class Admin extends User {}
来源：https://xo.zhonguo5118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://vh.zhonguo3118.cn

Ruby: class Admin < User; end
来源：https://hv.zhonguo7118.cn

C#:   class Admin : User {}
来源：https://ii.zhonguo3118.cn

[G06] 重写方法
来源：https://va.zhonguo8118.cn

Py:   def greet(self): return "admin"
来源：https://yv.zhonguo7118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://uu.zhonguo4118.cn

JS:   greet() { return "admin"; }
来源：https://zz.zhonguo2118.cn

TS:   greet(): string { return "admin"; }
来源：https://jr.zhonguo8118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ju.zhonguo7118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://kh.zhonguo2118.cn

Ruby: def greet; "admin"; end
来源：https://va.zhonguo4118.cn

C#:   public override string Greet() => "admin";
来源：https://mt.zhonguo3118.cn

[G07] 调用父类方法
来源：https://li.zhonguo8118.cn

Py:   super().greet()
来源：https://ag.zhonguo1118.cn

PHP:  parent::greet();
来源：https://jw.zhonguo5118.cn

JS:   super.greet();
来源：https://ru.zhonguo3118.cn

TS:   super.greet();
来源：https://nc.zhonguo8118.cn

Java: super.greet();
来源：https://ci.zhonguo5118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://oz.zhonguo3118.cn

Ruby: super
来源：https://dc.zhonguo4118.cn

C#:   base.Greet();
来源：https://gw.zhonguo1118.cn

[G08] 静态方法与属性
来源：https://gr.zhonguo5118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://mi.zhonguo2118.cn

PHP:  public static function f() {}
来源：https://ea.zhonguo2118.cn

JS:   static f() {}
来源：https://om.zhonguo7118.cn

TS:   static f(): void {}
来源：https://jh.zhonguo2118.cn

Java: static void f() {}
来源：https://fr.zhonguo8118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://ls.zhonguo5118.cn

Ruby: def self.f; end
来源：https://up.zhonguo5118.cn

C#:   public static void F() {}
来源：https://hq.zhonguo4118.cn

[G09] 接口 / 抽象类
来源：https://ol.zhonguo2118.cn

Py:   from abc import ABC, abstractmethod
来源：https://qs.zhonguo7118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://gn.zhonguo8118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://uc.zhonguo7118.cn

TS:   interface Shape { area(): number; }
来源：https://om.zhonguo5118.cn

Java: interface Shape { double area(); }
来源：https://rv.zhonguo6118.cn

Go:   type Shape interface { Area() float64 }
来源：https://ka.zhonguo7118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://oo.zhonguo3118.cn

C#:   interface IShape { double Area(); }
来源：https://hs.zhonguo1118.cn

[G10] 访问控制
来源：https://fm.zhonguo7118.cn

Py:   约定 _protected / __private（不强制）
来源：https://om.zhonguo7118.cn

PHP:  public / protected / private
来源：https://vf.zhonguo5118.cn

JS:   #private 字段；其余公开
来源：https://js.zhonguo3118.cn

TS:   public / protected / private
来源：https://qf.zhonguo2118.cn

Java: public / protected / private / 默认包级
来源：https://jm.zhonguo2118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://vq.zhonguo3118.cn

Ruby: public / protected / private
来源：https://sm.zhonguo1118.cn

C#:   public / protected / private / internal
来源：https://uj.zhonguo4118.cn

[G11] getter / setter
来源：https://ae.zhonguo5118.cn

Py:   @property 与 @x.setter
来源：https://ry.zhonguo3118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://nl.zhonguo7118.cn

JS:   get name() { return this._name; }
来源：https://yb.zhonguo7118.cn

TS:   get name(): string { return this._name; }
来源：https://qy.zhonguo6118.cn

Java: public String getName() { return name; }
来源：https://xq.zhonguo4118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://uu.zhonguo4118.cn

Ruby: attr_accessor :name
来源：https://rf.zhonguo8118.cn

C#:   public string Name { get; set; }
来源：https://cm.zhonguo2118.cn

[G12] 对象转字符串
来源：https://fj.zhonguo6118.cn

Py:   def __str__(self): return self.name
来源：https://iy.zhonguo5118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ym.zhonguo8118.cn

JS:   toString() { return this.name; }
来源：https://vd.zhonguo1118.cn

TS:   toString(): string { return this.name; }
来源：https://xu.zhonguo2118.cn

Java: @Override public String toString() { return name; }
来源：https://sy.zhonguo3118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://gt.zhonguo1118.cn

Ruby: def to_s; @name; end
来源：https://ft.zhonguo6118.cn

C#:   public override string ToString() => Name;
来源：https://kg.zhonguo6118.cn

[G13] 判断对象类型
来源：https://sh.zhonguo3118.cn

Py:   isinstance(u, User)
来源：https://cm.zhonguo5118.cn

PHP:  $u instanceof User
来源：https://fp.zhonguo8118.cn

JS:   u instanceof User
来源：https://qf.zhonguo4118.cn

TS:   u instanceof User
来源：https://eb.zhonguo1118.cn

Java: u instanceof User
来源：https://am.zhonguo8118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://kf.zhonguo1118.cn

Ruby: u.is_a?(User)
来源：https://hd.zhonguo5118.cn

C#:   u is User
来源：https://if.zhonguo4118.cn

[G14] 数据类 / record
来源：https://cs.zhonguo4118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://ju.zhonguo4118.cn

PHP:  // 用 readonly 属性模拟
来源：https://cq.zhonguo8118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://ue.zhonguo3118.cn

TS:   type User = { name: string; age: number };
来源：https://uc.zhonguo4118.cn

Java: record User(String name, int age) {}
来源：https://db.zhonguo7118.cn

Go:   type User struct { Name string; Age int }
来源：https://vx.zhonguo7118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://by.zhonguo7118.cn

C#:   record User(string Name, int Age);
来源：https://yq.zhonguo2118.cn

[G15] 枚举
来源：https://hr.zhonguo6118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://vp.zhonguo4118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://mk.zhonguo7118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://qm.zhonguo5118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://ds.zhonguo8118.cn

Java: enum Color { RED, GREEN }
来源：https://ql.zhonguo6118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://da.zhonguo7118.cn

Ruby: Color = %i[red green].freeze
来源：https://gx.zhonguo8118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://ri.zhonguo3118.cn

[G16] 对象转数组 / 字典
来源：https://hf.zhonguo3118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://vs.zhonguo1118.cn

PHP:  get_object_vars($obj);
来源：https://jg.zhonguo2118.cn

JS:   Object.entries(obj)
来源：https://vo.zhonguo3118.cn

TS:   Object.entries(obj)
来源：https://rd.zhonguo2118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://yu.zhonguo7118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://eg.zhonguo6118.cn

Ruby: obj.instance_variables
来源：https://yd.zhonguo2118.cn

C#:   // 用反射或 System.Text.Json
来源：https://ti.zhonguo3118.cn

================================================================================
来源：https://ch.zhonguo3118.cn

H. 异常与错误处理
来源：https://ef.zhonguo7118.cn

================================================================================
来源：https://ir.zhonguo6118.cn

[H01] try / catch 基础
来源：https://up.zhonguo6118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://gd.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://vg.zhonguo8118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://ii.zhonguo4118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://mz.zhonguo6118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://ld.zhonguo6118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://ma.zhonguo8118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://eq.zhonguo5118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://hq.zhonguo5118.cn

[H02] finally / ensure 收尾
来源：https://sq.zhonguo7118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://nc.zhonguo3118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://xs.zhonguo2118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://hn.zhonguo6118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://ef.zhonguo6118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://jk.zhonguo8118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://ga.zhonguo4118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://gj.zhonguo3118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://es.zhonguo2118.cn

[H03] 主动抛出异常
来源：https://qv.zhonguo6118.cn

Py:   raise ValueError("错误信息")
来源：https://ez.zhonguo2118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://rr.zhonguo8118.cn

JS:   throw new Error("错误信息");
来源：https://ws.zhonguo2118.cn

TS:   throw new Error("错误信息");
来源：https://ly.zhonguo2118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://zd.zhonguo2118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://yn.zhonguo3118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://eg.zhonguo2118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://jd.zhonguo6118.cn

[H04] 自定义异常类型
来源：https://bh.zhonguo1118.cn

Py:   class MyError(Exception): pass
来源：https://za.zhonguo7118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://ew.zhonguo5118.cn

JS:   class MyError extends Error {}
来源：https://xz.zhonguo1118.cn

TS:   class MyError extends Error {}
来源：https://iu.zhonguo7118.cn

Java: class MyException extends RuntimeException {}
来源：https://yt.zhonguo7118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://om.zhonguo6118.cn

Ruby: class MyError < StandardError; end
来源：https://ed.zhonguo6118.cn

C#:   class MyException : Exception {}
来源：https://zu.zhonguo2118.cn

[H05] 捕获特定类型
来源：https://za.zhonguo2118.cn

Py:   except ValueError as e:
来源：https://jn.zhonguo8118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://fg.zhonguo2118.cn

JS:   if (e instanceof TypeError) {}
来源：https://lc.zhonguo5118.cn

TS:   if (e instanceof TypeError) {}
来源：https://tz.zhonguo7118.cn

Java: catch (IOException | SQLException e) {}
来源：https://xq.zhonguo2118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://ge.zhonguo3118.cn

Ruby: rescue ArgumentError => e
来源：https://vw.zhonguo2118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://vw.zhonguo2118.cn

[H06] 可选值 / 空值安全访问
来源：https://eg.zhonguo3118.cn


<!-- 参考信息 -->