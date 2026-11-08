代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：https://mr.zhonguo8118.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：https://wz.zhonguo6118.cn

[F03] 写入文件（覆盖）
来源：https://eq.zhonguo7118.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：https://ry.zhonguo1118.cn

PHP:  file_put_contents("a.txt", "hi");
来源：https://sa.zhonguo1118.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://op.zhonguo8118.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：https://fr.zhonguo3118.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：https://ts.zhonguo6118.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：https://ld.zhonguo6118.cn

Ruby: File.write("a.txt", "hi")
来源：https://bb.zhonguo2118.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：https://bj.zhonguo1118.cn

[F04] 追加写入文件
来源：https://ks.zhonguo6118.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://vz.zhonguo3118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://nc.zhonguo7118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://jo.zhonguo4118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ht.zhonguo1118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://cq.zhonguo8118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://lb.zhonguo4118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://ed.zhonguo2118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://an.zhonguo6118.cn

[F05] 判断文件或目录是否存在
来源：https://wh.zhonguo8118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://yx.zhonguo5118.cn

PHP:  file_exists("a.txt");
来源：https://mc.zhonguo3118.cn

JS:   fs.existsSync("a.txt")
来源：https://ae.zhonguo5118.cn

TS:   fs.existsSync("a.txt")
来源：https://uc.zhonguo2118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://bt.zhonguo4118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://ep.zhonguo2118.cn

Ruby: File.exist?("a.txt")
来源：https://sj.zhonguo4118.cn

C#:   File.Exists("a.txt")
来源：https://bk.zhonguo8118.cn

[F06] 删除文件
来源：https://uz.zhonguo7118.cn

Py:   os.remove("a.txt")
来源：https://uh.zhonguo7118.cn

PHP:  unlink("a.txt");
来源：https://pm.zhonguo2118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://sh.zhonguo7118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://ys.zhonguo3118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://lv.zhonguo2118.cn

Go:   os.Remove("a.txt")
来源：https://bk.zhonguo4118.cn

Ruby: File.delete("a.txt")
来源：https://nq.zhonguo1118.cn

C#:   File.Delete("a.txt");
来源：https://qb.zhonguo1118.cn

[F07] 创建目录（含多级）
来源：https://sd.zhonguo3118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://at.zhonguo5118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://ks.zhonguo7118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://mr.zhonguo5118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://tz.zhonguo6118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://no.zhonguo8118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://hx.zhonguo1118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://fr.zhonguo2118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://ke.zhonguo5118.cn

[F08] 遍历目录
来源：https://ki.zhonguo4118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://nk.zhonguo4118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://ap.zhonguo7118.cn

JS:   fs.readdirSync("dir")
来源：https://ju.zhonguo1118.cn

TS:   fs.readdirSync("dir")
来源：https://nf.zhonguo6118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://wl.zhonguo5118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://qr.zhonguo5118.cn

Ruby: Dir.children("dir")
来源：https://mb.zhonguo1118.cn

C#:   Directory.GetFiles("dir")
来源：https://zv.zhonguo6118.cn

[F09] 获取文件大小
来源：https://ss.zhonguo3118.cn

Py:   os.path.getsize("a.txt")
来源：https://qy.zhonguo6118.cn

PHP:  filesize("a.txt");
来源：https://hp.zhonguo6118.cn

JS:   fs.statSync("a.txt").size
来源：https://bi.zhonguo1118.cn

TS:   fs.statSync("a.txt").size
来源：https://zm.zhonguo2118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://pk.zhonguo4118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://bo.zhonguo7118.cn

Ruby: File.size("a.txt")
来源：https://pl.zhonguo7118.cn

C#:   new FileInfo("a.txt").Length
来源：https://rn.zhonguo5118.cn

[F10] 取文件扩展名 / 文件名
来源：https://en.zhonguo7118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://kz.zhonguo6118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://wa.zhonguo2118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://ii.zhonguo3118.cn

TS:   path.extname("a.txt")
来源：https://gc.zhonguo8118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://bb.zhonguo6118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://xv.zhonguo4118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://sj.zhonguo4118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://xl.zhonguo1118.cn

[F11] 复制与移动文件
来源：https://il.zhonguo3118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://wl.zhonguo8118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://nr.zhonguo4118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://bc.zhonguo6118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://zt.zhonguo1118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://ok.zhonguo8118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://rx.zhonguo8118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://bq.zhonguo5118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://jd.zhonguo2118.cn

[F12] CSV 读写
来源：https://zs.zhonguo2118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://bg.zhonguo8118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://ee.zhonguo4118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://jj.zhonguo3118.cn

TS:   // 同上
来源：https://gl.zhonguo1118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://cv.zhonguo7118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://gj.zhonguo3118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://iw.zhonguo7118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://ga.zhonguo3118.cn

================================================================================
来源：https://ri.zhonguo5118.cn

G. 面向对象
来源：https://nn.zhonguo4118.cn

================================================================================
来源：https://vk.zhonguo3118.cn

[G01] 定义类
来源：https://pz.zhonguo4118.cn

Py:   class User: pass
来源：https://jj.zhonguo7118.cn

PHP:  class User {}
来源：https://ps.zhonguo3118.cn

JS:   class User {}
来源：https://lw.zhonguo2118.cn

TS:   class User { name: string = ""; }
来源：https://pm.zhonguo7118.cn

Java: class User {}
来源：https://ai.zhonguo4118.cn

Go:   type User struct { Name string }
来源：https://br.zhonguo5118.cn

Ruby: class User; end
来源：https://kk.zhonguo8118.cn

C#:   class User {}
来源：https://gp.zhonguo3118.cn

[G02] 构造函数
来源：https://kr.zhonguo7118.cn

Py:   def __init__(self, name): self.name = name
来源：https://vl.zhonguo8118.cn

PHP:  public function __construct(public string $name) {}
来源：https://zj.zhonguo3118.cn

JS:   constructor(name) { this.name = name; }
来源：https://oe.zhonguo2118.cn

TS:   constructor(public name: string) {}
来源：https://wn.zhonguo1118.cn

Java: User(String name) { this.name = name; }
来源：https://sz.zhonguo7118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://la.zhonguo7118.cn

Ruby: def initialize(name); @name = name; end
来源：https://nb.zhonguo2118.cn

C#:   public User(string name) { Name = name; }
来源：https://iv.zhonguo6118.cn

[G03] 实例属性
来源：https://fy.zhonguo3118.cn

Py:   self.name = "x"
来源：https://tq.zhonguo6118.cn

PHP:  public string $name = "x";
来源：https://bu.zhonguo7118.cn

JS:   this.name = "x";
来源：https://ct.zhonguo5118.cn

TS:   name: string = "x";
来源：https://og.zhonguo4118.cn

Java: private String name;
来源：https://ai.zhonguo8118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://hx.zhonguo6118.cn

Ruby: @name = "x"
来源：https://wp.zhonguo1118.cn

C#:   public string Name { get; set; } = "x";
来源：https://as.zhonguo5118.cn

[G04] 定义方法
来源：https://og.zhonguo3118.cn

Py:   def greet(self): return self.name
来源：https://zu.zhonguo8118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://wq.zhonguo2118.cn

JS:   greet() { return this.name; }
来源：https://ev.zhonguo4118.cn

TS:   greet(): string { return this.name; }
来源：https://nv.zhonguo6118.cn

Java: String greet() { return name; }
来源：https://wu.zhonguo3118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://nw.zhonguo5118.cn

Ruby: def greet; @name; end
来源：https://hc.zhonguo8118.cn

C#:   public string Greet() => Name;
来源：https://vq.zhonguo4118.cn

[G05] 继承
来源：https://ss.zhonguo7118.cn

Py:   class Admin(User): pass
来源：https://id.zhonguo2118.cn

PHP:  class Admin extends User {}
来源：https://aq.zhonguo6118.cn

JS:   class Admin extends User {}
来源：https://zb.zhonguo4118.cn

TS:   class Admin extends User {}
来源：https://ea.zhonguo5118.cn

Java: class Admin extends User {}
来源：https://cq.zhonguo7118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://om.zhonguo7118.cn

Ruby: class Admin < User; end
来源：https://kw.zhonguo8118.cn

C#:   class Admin : User {}
来源：https://hu.zhonguo4118.cn

[G06] 重写方法
来源：https://ac.zhonguo2118.cn

Py:   def greet(self): return "admin"
来源：https://vc.zhonguo1118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://rt.zhonguo1118.cn

JS:   greet() { return "admin"; }
来源：https://qw.zhonguo1118.cn

TS:   greet(): string { return "admin"; }
来源：https://al.zhonguo5118.cn

Java: @Override String greet() { return "admin"; }
来源：https://lo.zhonguo1118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://ba.zhonguo5118.cn

Ruby: def greet; "admin"; end
来源：https://wh.zhonguo7118.cn

C#:   public override string Greet() => "admin";
来源：https://gb.zhonguo1118.cn

[G07] 调用父类方法
来源：https://vj.zhonguo8118.cn

Py:   super().greet()
来源：https://ar.zhonguo4118.cn

PHP:  parent::greet();
来源：https://qa.zhonguo6118.cn

JS:   super.greet();
来源：https://fu.zhonguo3118.cn

TS:   super.greet();
来源：https://gj.zhonguo6118.cn

Java: super.greet();
来源：https://ab.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://cq.zhonguo1118.cn

Ruby: super
来源：https://zr.zhonguo6118.cn

C#:   base.Greet();
来源：https://gk.zhonguo7118.cn

[G08] 静态方法与属性
来源：https://uh.zhonguo5118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://kh.zhonguo8118.cn

PHP:  public static function f() {}
来源：https://bb.zhonguo8118.cn

JS:   static f() {}
来源：https://tm.zhonguo7118.cn

TS:   static f(): void {}
来源：https://ez.zhonguo6118.cn

Java: static void f() {}
来源：https://pb.zhonguo8118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://vi.zhonguo6118.cn

Ruby: def self.f; end
来源：https://sk.zhonguo1118.cn

C#:   public static void F() {}
来源：https://mc.zhonguo2118.cn

[G09] 接口 / 抽象类
来源：https://bp.zhonguo3118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ja.zhonguo1118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://na.zhonguo1118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://mz.zhonguo6118.cn

TS:   interface Shape { area(): number; }
来源：https://rp.zhonguo6118.cn

Java: interface Shape { double area(); }
来源：https://qd.zhonguo3118.cn

Go:   type Shape interface { Area() float64 }
来源：https://ku.zhonguo6118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://iq.zhonguo5118.cn

C#:   interface IShape { double Area(); }
来源：https://ux.zhonguo2118.cn

[G10] 访问控制
来源：https://co.zhonguo3118.cn

Py:   约定 _protected / __private（不强制）
来源：https://xb.zhonguo3118.cn

PHP:  public / protected / private
来源：https://sb.zhonguo5118.cn

JS:   #private 字段；其余公开
来源：https://no.zhonguo6118.cn

TS:   public / protected / private
来源：https://kl.zhonguo6118.cn

Java: public / protected / private / 默认包级
来源：https://sp.zhonguo8118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://rk.zhonguo4118.cn

Ruby: public / protected / private
来源：https://ry.zhonguo1118.cn

C#:   public / protected / private / internal
来源：https://xa.zhonguo8118.cn

[G11] getter / setter
来源：https://qp.zhonguo2118.cn

Py:   @property 与 @x.setter
来源：https://hs.zhonguo5118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://tr.zhonguo5118.cn

JS:   get name() { return this._name; }
来源：https://xx.zhonguo4118.cn

TS:   get name(): string { return this._name; }
来源：https://rd.zhonguo8118.cn

Java: public String getName() { return name; }
来源：https://ca.zhonguo4118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://tx.zhonguo2118.cn

Ruby: attr_accessor :name
来源：https://zy.zhonguo5118.cn

C#:   public string Name { get; set; }
来源：https://ma.zhonguo2118.cn

[G12] 对象转字符串
来源：https://cq.zhonguo7118.cn

Py:   def __str__(self): return self.name
来源：https://te.zhonguo3118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://gx.zhonguo7118.cn

JS:   toString() { return this.name; }
来源：https://va.zhonguo1118.cn

TS:   toString(): string { return this.name; }
来源：https://or.zhonguo4118.cn

Java: @Override public String toString() { return name; }
来源：https://qm.zhonguo8118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://mu.zhonguo6118.cn

Ruby: def to_s; @name; end
来源：https://kb.zhonguo7118.cn

C#:   public override string ToString() => Name;
来源：https://ft.zhonguo5118.cn

[G13] 判断对象类型
来源：https://fb.zhonguo6118.cn

Py:   isinstance(u, User)
来源：https://jg.zhonguo5118.cn

PHP:  $u instanceof User
来源：https://xa.zhonguo3118.cn

JS:   u instanceof User
来源：https://ph.zhonguo4118.cn

TS:   u instanceof User
来源：https://uy.zhonguo7118.cn

Java: u instanceof User
来源：https://fy.zhonguo7118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://mv.zhonguo2118.cn

Ruby: u.is_a?(User)
来源：https://qm.zhonguo4118.cn

C#:   u is User
来源：https://sg.zhonguo8118.cn

[G14] 数据类 / record
来源：https://og.zhonguo3118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://ve.zhonguo5118.cn

PHP:  // 用 readonly 属性模拟
来源：https://ef.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://bu.zhonguo7118.cn

TS:   type User = { name: string; age: number };
来源：https://nl.zhonguo8118.cn

Java: record User(String name, int age) {}
来源：https://qr.zhonguo6118.cn

Go:   type User struct { Name string; Age int }
来源：https://rw.zhonguo6118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://fh.zhonguo8118.cn

C#:   record User(string Name, int Age);
来源：https://hh.zhonguo3118.cn

[G15] 枚举
来源：https://cc.zhonguo4118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://pw.zhonguo7118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://kb.zhonguo7118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://by.zhonguo8118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://qo.zhonguo8118.cn

Java: enum Color { RED, GREEN }
来源：https://lg.zhonguo1118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://ok.zhonguo4118.cn

Ruby: Color = %i[red green].freeze
来源：https://qo.zhonguo6118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://kq.zhonguo2118.cn

[G16] 对象转数组 / 字典
来源：https://qg.zhonguo8118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://na.zhonguo8118.cn

PHP:  get_object_vars($obj);
来源：https://gh.zhonguo2118.cn

JS:   Object.entries(obj)
来源：https://pc.zhonguo1118.cn

TS:   Object.entries(obj)
来源：https://wl.zhonguo6118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://fb.zhonguo8118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://cl.zhonguo7118.cn

Ruby: obj.instance_variables
来源：https://kc.zhonguo6118.cn

C#:   // 用反射或 System.Text.Json
来源：https://vl.zhonguo1118.cn

================================================================================
来源：https://jp.zhonguo3118.cn

H. 异常与错误处理
来源：https://iy.zhonguo3118.cn

================================================================================
来源：https://hu.zhonguo2118.cn

[H01] try / catch 基础
来源：https://hv.zhonguo4118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://rc.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://ns.zhonguo3118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://mz.zhonguo3118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://pp.zhonguo4118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://wt.zhonguo7118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://oy.zhonguo8118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://ue.zhonguo2118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://te.zhonguo5118.cn

[H02] finally / ensure 收尾
来源：https://ae.zhonguo7118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://zw.zhonguo6118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://cj.zhonguo8118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://cp.zhonguo5118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://wl.zhonguo1118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://hg.zhonguo1118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://hh.zhonguo4118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://ca.zhonguo6118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://et.zhonguo3118.cn

[H03] 主动抛出异常
来源：https://qk.zhonguo7118.cn

Py:   raise ValueError("错误信息")
来源：https://pu.zhonguo4118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://dq.zhonguo2118.cn

JS:   throw new Error("错误信息");
来源：https://wf.zhonguo6118.cn

TS:   throw new Error("错误信息");
来源：https://jg.zhonguo4118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://vj.zhonguo8118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://pa.zhonguo2118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://pf.zhonguo8118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://xl.zhonguo2118.cn

[H04] 自定义异常类型
来源：https://iy.zhonguo2118.cn

Py:   class MyError(Exception): pass
来源：https://ys.zhonguo1118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://qk.zhonguo2118.cn

JS:   class MyError extends Error {}
来源：https://db.zhonguo8118.cn

TS:   class MyError extends Error {}
来源：https://ww.zhonguo5118.cn

Java: class MyException extends RuntimeException {}
来源：https://vn.zhonguo1118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://rk.zhonguo2118.cn

Ruby: class MyError < StandardError; end
来源：https://fc.zhonguo6118.cn

C#:   class MyException : Exception {}
来源：https://ko.zhonguo7118.cn

[H05] 捕获特定类型
来源：https://va.zhonguo3118.cn

Py:   except ValueError as e:
来源：https://fp.zhonguo2118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://oy.zhonguo2118.cn

JS:   if (e instanceof TypeError) {}
来源：https://fy.zhonguo8118.cn

TS:   if (e instanceof TypeError) {}
来源：https://gl.zhonguo8118.cn

Java: catch (IOException | SQLException e) {}
来源：https://lu.zhonguo1118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://fy.zhonguo1118.cn

Ruby: rescue ArgumentError => e
来源：https://zj.zhonguo1118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://wq.zhonguo4118.cn

[H06] 可选值 / 空值安全访问
来源：https://lt.zhonguo1118.cn

Py:   value = d.get("k") or default
来源：https://si.zhonguo8118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://mo.zhonguo6118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://vt.zhonguo2118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://pi.zhonguo2118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://tz.zhonguo1118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://sx.zhonguo7118.cn

Ruby: d&.dig(:a, :b)
来源：https://vy.zhonguo2118.cn

C#:   obj?.A?.B ?? default
来源：https://mv.zhonguo6118.cn

[H07] 断言
来源：https://sn.zhonguo4118.cn

Py:   assert x > 0, "必须为正"
来源：https://wz.zhonguo1118.cn

PHP:  assert($x > 0);
来源：https://xm.zhonguo6118.cn

JS:   console.assert(x > 0);
来源：https://kx.zhonguo6118.cn


<!-- 参考信息 -->