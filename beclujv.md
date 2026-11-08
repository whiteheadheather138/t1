代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://bp.zhonguo5118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://mf.zhonguo6118.cn

[F03] 写入文件（覆盖）
来源：https://up.zhonguo2118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://nq.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://dj.zhonguo1118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://am.zhonguo3118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://ib.zhonguo5118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://ob.zhonguo4118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://cc.zhonguo3118.cn

Ruby: File.write("a.txt", "hi")
来源：https://wz.zhonguo5118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://pm.zhonguo3118.cn

[F04] 追加写入文件
来源：https://qe.zhonguo3118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://zh.zhonguo2118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://bk.zhonguo5118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ql.zhonguo1118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://sy.zhonguo4118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://tw.zhonguo4118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://un.zhonguo7118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://zc.zhonguo8118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://ei.zhonguo4118.cn

[F05] 判断文件或目录是否存在
来源：https://qw.zhonguo4118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://nf.zhonguo1118.cn

PHP:  file_exists("a.txt");
来源：https://lc.zhonguo1118.cn

JS:   fs.existsSync("a.txt")
来源：https://xn.zhonguo8118.cn

TS:   fs.existsSync("a.txt")
来源：https://zz.zhonguo8118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://os.zhonguo4118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://kh.zhonguo2118.cn

Ruby: File.exist?("a.txt")
来源：https://bh.zhonguo5118.cn

C#:   File.Exists("a.txt")
来源：https://us.zhonguo5118.cn

[F06] 删除文件
来源：https://qr.zhonguo1118.cn

Py:   os.remove("a.txt")
来源：https://nv.zhonguo4118.cn

PHP:  unlink("a.txt");
来源：https://dh.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://xo.zhonguo8118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://ah.zhonguo3118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://yc.zhonguo2118.cn

Go:   os.Remove("a.txt")
来源：https://sa.zhonguo2118.cn

Ruby: File.delete("a.txt")
来源：https://fz.zhonguo6118.cn

C#:   File.Delete("a.txt");
来源：https://tt.zhonguo4118.cn

[F07] 创建目录（含多级）
来源：https://mx.zhonguo4118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://wc.zhonguo7118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://re.zhonguo6118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://ts.zhonguo2118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://uy.zhonguo8118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://qj.zhonguo4118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://kp.zhonguo3118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://hw.zhonguo5118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://uz.zhonguo8118.cn

[F08] 遍历目录
来源：https://lz.zhonguo7118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://jy.zhonguo3118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://tx.zhonguo5118.cn

JS:   fs.readdirSync("dir")
来源：https://lw.zhonguo5118.cn

TS:   fs.readdirSync("dir")
来源：https://ay.zhonguo6118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://xv.zhonguo4118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://dr.zhonguo3118.cn

Ruby: Dir.children("dir")
来源：https://qk.zhonguo3118.cn

C#:   Directory.GetFiles("dir")
来源：https://ad.zhonguo5118.cn

[F09] 获取文件大小
来源：https://bi.zhonguo7118.cn

Py:   os.path.getsize("a.txt")
来源：https://ne.zhonguo3118.cn

PHP:  filesize("a.txt");
来源：https://ti.zhonguo8118.cn

JS:   fs.statSync("a.txt").size
来源：https://rk.zhonguo4118.cn

TS:   fs.statSync("a.txt").size
来源：https://uq.zhonguo4118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://wr.zhonguo2118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://cq.zhonguo5118.cn

Ruby: File.size("a.txt")
来源：https://zi.zhonguo3118.cn

C#:   new FileInfo("a.txt").Length
来源：https://ly.zhonguo7118.cn

[F10] 取文件扩展名 / 文件名
来源：https://mr.zhonguo8118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://ny.zhonguo6118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://uj.zhonguo7118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://il.zhonguo6118.cn

TS:   path.extname("a.txt")
来源：https://rd.zhonguo2118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://cx.zhonguo1118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://mv.zhonguo5118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://ga.zhonguo6118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://tj.zhonguo6118.cn

[F11] 复制与移动文件
来源：https://rf.zhonguo1118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://gd.zhonguo4118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ty.zhonguo3118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://zr.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://sy.zhonguo5118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://vm.zhonguo1118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://cv.zhonguo8118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://jq.zhonguo6118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://kb.zhonguo3118.cn

[F12] CSV 读写
来源：https://pj.zhonguo3118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://sl.zhonguo1118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://sv.zhonguo4118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://hi.zhonguo8118.cn

TS:   // 同上
来源：https://gb.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://qx.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://cy.zhonguo5118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://so.zhonguo1118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://in.zhonguo4118.cn

================================================================================
来源：https://qv.zhonguo6118.cn

G. 面向对象
来源：https://wc.zhonguo7118.cn

================================================================================
来源：https://ie.zhonguo4118.cn

[G01] 定义类
来源：https://up.zhonguo5118.cn

Py:   class User: pass
来源：https://nu.zhonguo7118.cn

PHP:  class User {}
来源：https://ad.zhonguo6118.cn

JS:   class User {}
来源：https://qs.zhonguo2118.cn

TS:   class User { name: string = ""; }
来源：https://si.zhonguo1118.cn

Java: class User {}
来源：https://om.zhonguo7118.cn

Go:   type User struct { Name string }
来源：https://fy.zhonguo8118.cn

Ruby: class User; end
来源：https://iu.zhonguo6118.cn

C#:   class User {}
来源：https://ah.zhonguo1118.cn

[G02] 构造函数
来源：https://ka.zhonguo5118.cn

Py:   def __init__(self, name): self.name = name
来源：https://ec.zhonguo3118.cn

PHP:  public function __construct(public string $name) {}
来源：https://ma.zhonguo7118.cn

JS:   constructor(name) { this.name = name; }
来源：https://bn.zhonguo7118.cn

TS:   constructor(public name: string) {}
来源：https://mb.zhonguo5118.cn

Java: User(String name) { this.name = name; }
来源：https://xz.zhonguo7118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://lb.zhonguo2118.cn

Ruby: def initialize(name); @name = name; end
来源：https://ri.zhonguo4118.cn

C#:   public User(string name) { Name = name; }
来源：https://dz.zhonguo8118.cn

[G03] 实例属性
来源：https://bb.zhonguo2118.cn

Py:   self.name = "x"
来源：https://ol.zhonguo8118.cn

PHP:  public string $name = "x";
来源：https://gf.zhonguo1118.cn

JS:   this.name = "x";
来源：https://ba.zhonguo5118.cn

TS:   name: string = "x";
来源：https://xp.zhonguo2118.cn

Java: private String name;
来源：https://tm.zhonguo5118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://tl.zhonguo2118.cn

Ruby: @name = "x"
来源：https://bm.zhonguo6118.cn

C#:   public string Name { get; set; } = "x";
来源：https://qi.zhonguo6118.cn

[G04] 定义方法
来源：https://hy.zhonguo5118.cn

Py:   def greet(self): return self.name
来源：https://yo.zhonguo1118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://it.zhonguo4118.cn

JS:   greet() { return this.name; }
来源：https://qs.zhonguo8118.cn

TS:   greet(): string { return this.name; }
来源：https://ok.zhonguo5118.cn

Java: String greet() { return name; }
来源：https://ba.zhonguo1118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://ep.zhonguo7118.cn

Ruby: def greet; @name; end
来源：https://bc.zhonguo1118.cn

C#:   public string Greet() => Name;
来源：https://yz.zhonguo4118.cn

[G05] 继承
来源：https://gy.zhonguo8118.cn

Py:   class Admin(User): pass
来源：https://ju.zhonguo3118.cn

PHP:  class Admin extends User {}
来源：https://ka.zhonguo3118.cn

JS:   class Admin extends User {}
来源：https://lp.zhonguo4118.cn

TS:   class Admin extends User {}
来源：https://xj.zhonguo8118.cn

Java: class Admin extends User {}
来源：https://ti.zhonguo2118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://xa.zhonguo7118.cn

Ruby: class Admin < User; end
来源：https://or.zhonguo2118.cn

C#:   class Admin : User {}
来源：https://le.zhonguo7118.cn

[G06] 重写方法
来源：https://rp.zhonguo7118.cn

Py:   def greet(self): return "admin"
来源：https://mx.zhonguo6118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://ba.zhonguo8118.cn

JS:   greet() { return "admin"; }
来源：https://zz.zhonguo3118.cn

TS:   greet(): string { return "admin"; }
来源：https://kn.zhonguo5118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ac.zhonguo6118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://go.zhonguo4118.cn

Ruby: def greet; "admin"; end
来源：https://zr.zhonguo5118.cn

C#:   public override string Greet() => "admin";
来源：https://pg.zhonguo6118.cn

[G07] 调用父类方法
来源：https://tm.zhonguo8118.cn

Py:   super().greet()
来源：https://pg.zhonguo7118.cn

PHP:  parent::greet();
来源：https://tq.zhonguo4118.cn

JS:   super.greet();
来源：https://zx.zhonguo5118.cn

TS:   super.greet();
来源：https://co.zhonguo3118.cn

Java: super.greet();
来源：https://vo.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://wp.zhonguo8118.cn

Ruby: super
来源：https://mm.zhonguo1118.cn

C#:   base.Greet();
来源：https://cs.zhonguo5118.cn

[G08] 静态方法与属性
来源：https://sx.zhonguo5118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://yg.zhonguo6118.cn

PHP:  public static function f() {}
来源：https://rx.zhonguo3118.cn

JS:   static f() {}
来源：https://jv.zhonguo7118.cn

TS:   static f(): void {}
来源：https://ui.zhonguo3118.cn

Java: static void f() {}
来源：https://ke.zhonguo6118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://zv.zhonguo6118.cn

Ruby: def self.f; end
来源：https://ic.zhonguo6118.cn

C#:   public static void F() {}
来源：https://jn.zhonguo3118.cn

[G09] 接口 / 抽象类
来源：https://cp.zhonguo5118.cn

Py:   from abc import ABC, abstractmethod
来源：https://su.zhonguo4118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://pz.zhonguo1118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://ek.zhonguo7118.cn

TS:   interface Shape { area(): number; }
来源：https://eh.zhonguo1118.cn

Java: interface Shape { double area(); }
来源：https://oi.zhonguo3118.cn

Go:   type Shape interface { Area() float64 }
来源：https://ej.zhonguo5118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://dv.zhonguo7118.cn

C#:   interface IShape { double Area(); }
来源：https://zg.zhonguo4118.cn

[G10] 访问控制
来源：https://yw.zhonguo6118.cn

Py:   约定 _protected / __private（不强制）
来源：https://bz.zhonguo3118.cn

PHP:  public / protected / private
来源：https://ex.zhonguo7118.cn

JS:   #private 字段；其余公开
来源：https://lt.zhonguo3118.cn

TS:   public / protected / private
来源：https://mb.zhonguo2118.cn

Java: public / protected / private / 默认包级
来源：https://lf.zhonguo8118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://ly.zhonguo7118.cn

Ruby: public / protected / private
来源：https://fe.zhonguo1118.cn

C#:   public / protected / private / internal
来源：https://rf.zhonguo4118.cn

[G11] getter / setter
来源：https://hd.zhonguo1118.cn

Py:   @property 与 @x.setter
来源：https://uz.zhonguo3118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://lt.zhonguo6118.cn

JS:   get name() { return this._name; }
来源：https://gf.zhonguo5118.cn

TS:   get name(): string { return this._name; }
来源：https://fk.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://ly.zhonguo4118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://vd.zhonguo8118.cn

Ruby: attr_accessor :name
来源：https://xb.zhonguo7118.cn

C#:   public string Name { get; set; }
来源：https://tp.zhonguo3118.cn

[G12] 对象转字符串
来源：https://kr.zhonguo6118.cn

Py:   def __str__(self): return self.name
来源：https://hz.zhonguo2118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ow.zhonguo7118.cn

JS:   toString() { return this.name; }
来源：https://sq.zhonguo7118.cn

TS:   toString(): string { return this.name; }
来源：https://hi.zhonguo7118.cn

Java: @Override public String toString() { return name; }
来源：https://hq.zhonguo1118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://my.zhonguo5118.cn

Ruby: def to_s; @name; end
来源：https://za.zhonguo2118.cn

C#:   public override string ToString() => Name;
来源：https://ih.zhonguo6118.cn

[G13] 判断对象类型
来源：https://zq.zhonguo8118.cn

Py:   isinstance(u, User)
来源：https://op.zhonguo5118.cn

PHP:  $u instanceof User
来源：https://hc.zhonguo5118.cn

JS:   u instanceof User
来源：https://mr.zhonguo3118.cn

TS:   u instanceof User
来源：https://de.zhonguo3118.cn

Java: u instanceof User
来源：https://px.zhonguo4118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://qd.zhonguo1118.cn

Ruby: u.is_a?(User)
来源：https://oi.zhonguo8118.cn

C#:   u is User
来源：https://pc.zhonguo4118.cn

[G14] 数据类 / record
来源：https://di.zhonguo3118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://qm.zhonguo2118.cn

PHP:  // 用 readonly 属性模拟
来源：https://jb.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://vu.zhonguo4118.cn

TS:   type User = { name: string; age: number };
来源：https://ib.zhonguo4118.cn

Java: record User(String name, int age) {}
来源：https://yi.zhonguo7118.cn

Go:   type User struct { Name string; Age int }
来源：https://rq.zhonguo2118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://ko.zhonguo6118.cn

C#:   record User(string Name, int Age);
来源：https://yq.zhonguo7118.cn

[G15] 枚举
来源：https://ml.zhonguo2118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://tz.zhonguo2118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://zn.zhonguo1118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://kd.zhonguo4118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://or.zhonguo3118.cn

Java: enum Color { RED, GREEN }
来源：https://vb.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://nm.zhonguo1118.cn

Ruby: Color = %i[red green].freeze
来源：https://bh.zhonguo3118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://tg.zhonguo3118.cn

[G16] 对象转数组 / 字典
来源：https://px.zhonguo4118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ro.zhonguo3118.cn

PHP:  get_object_vars($obj);
来源：https://me.zhonguo8118.cn

JS:   Object.entries(obj)
来源：https://wz.zhonguo4118.cn

TS:   Object.entries(obj)
来源：https://bh.zhonguo1118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://fy.zhonguo6118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://gc.zhonguo3118.cn

Ruby: obj.instance_variables
来源：https://zl.zhonguo6118.cn

C#:   // 用反射或 System.Text.Json
来源：https://uw.zhonguo8118.cn

================================================================================
来源：https://yt.zhonguo6118.cn

H. 异常与错误处理
来源：https://er.zhonguo2118.cn

================================================================================
来源：https://bk.zhonguo4118.cn

[H01] try / catch 基础
来源：https://xw.zhonguo7118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://wd.zhonguo2118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://fl.zhonguo7118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://ya.zhonguo8118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://mw.zhonguo5118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://fw.zhonguo2118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://lw.zhonguo7118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://fa.zhonguo7118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://zx.zhonguo7118.cn

[H02] finally / ensure 收尾
来源：https://xg.zhonguo2118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://ae.zhonguo1118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://ik.zhonguo8118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://hv.zhonguo6118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://yb.zhonguo4118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://nn.zhonguo4118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://aw.zhonguo3118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://dp.zhonguo3118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://ny.zhonguo8118.cn

[H03] 主动抛出异常
来源：https://bl.zhonguo4118.cn

Py:   raise ValueError("错误信息")
来源：https://ad.zhonguo5118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://mu.zhonguo6118.cn

JS:   throw new Error("错误信息");
来源：https://wb.zhonguo8118.cn

TS:   throw new Error("错误信息");
来源：https://sk.zhonguo2118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://ln.zhonguo3118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://lw.zhonguo7118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://xf.zhonguo8118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://qe.zhonguo8118.cn

[H04] 自定义异常类型
来源：https://rd.zhonguo3118.cn

Py:   class MyError(Exception): pass
来源：https://bb.zhonguo3118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://vt.zhonguo2118.cn

JS:   class MyError extends Error {}
来源：https://da.zhonguo2118.cn

TS:   class MyError extends Error {}
来源：https://ba.zhonguo4118.cn

Java: class MyException extends RuntimeException {}
来源：https://pi.zhonguo1118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://so.zhonguo2118.cn

Ruby: class MyError < StandardError; end
来源：https://dd.zhonguo7118.cn

C#:   class MyException : Exception {}
来源：https://ev.zhonguo5118.cn

[H05] 捕获特定类型
来源：https://lt.zhonguo5118.cn

Py:   except ValueError as e:
来源：https://fd.zhonguo3118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://wz.zhonguo6118.cn

JS:   if (e instanceof TypeError) {}
来源：https://cr.zhonguo3118.cn

TS:   if (e instanceof TypeError) {}
来源：https://az.zhonguo6118.cn

Java: catch (IOException | SQLException e) {}
来源：https://qq.zhonguo7118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://ez.zhonguo6118.cn

Ruby: rescue ArgumentError => e
来源：https://uq.zhonguo3118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://vb.zhonguo7118.cn

[H06] 可选值 / 空值安全访问
来源：https://xw.zhonguo4118.cn

Py:   value = d.get("k") or default
来源：https://rk.zhonguo5118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://fa.zhonguo4118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://pn.zhonguo7118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://nc.zhonguo1118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://dn.zhonguo2118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://dv.zhonguo6118.cn

Ruby: d&.dig(:a, :b)
来源：https://qw.zhonguo6118.cn

C#:   obj?.A?.B ?? default
来源：https://my.zhonguo8118.cn

[H07] 断言
来源：https://xi.zhonguo4118.cn

Py:   assert x > 0, "必须为正"
来源：https://tm.zhonguo5118.cn

PHP:  assert($x > 0);
来源：https://ij.zhonguo7118.cn

JS:   console.assert(x > 0);
来源：https://qc.zhonguo6118.cn


<!-- 参考信息 -->