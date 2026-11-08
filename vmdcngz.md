代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://nr.zhonguo1118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://uj.zhonguo1118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://vu.zhonguo3118.cn

[F08] 遍历目录
来源：https://zg.zhonguo4118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://rh.zhonguo1118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://zc.zhonguo6118.cn

JS:   fs.readdirSync("dir")
来源：https://aj.zhonguo8118.cn

TS:   fs.readdirSync("dir")
来源：https://gk.zhonguo5118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://re.zhonguo5118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://uu.zhonguo3118.cn

Ruby: Dir.children("dir")
来源：https://tt.zhonguo2118.cn

C#:   Directory.GetFiles("dir")
来源：https://qa.zhonguo7118.cn

[F09] 获取文件大小
来源：https://xa.zhonguo1118.cn

Py:   os.path.getsize("a.txt")
来源：https://rn.zhonguo4118.cn

PHP:  filesize("a.txt");
来源：https://ak.zhonguo7118.cn

JS:   fs.statSync("a.txt").size
来源：https://kr.zhonguo6118.cn

TS:   fs.statSync("a.txt").size
来源：https://xg.zhonguo8118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://ua.zhonguo5118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://np.zhonguo6118.cn

Ruby: File.size("a.txt")
来源：https://ld.zhonguo1118.cn

C#:   new FileInfo("a.txt").Length
来源：https://bl.zhonguo5118.cn

[F10] 取文件扩展名 / 文件名
来源：https://uj.zhonguo6118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://mh.zhonguo3118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://ad.zhonguo4118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://xh.zhonguo3118.cn

TS:   path.extname("a.txt")
来源：https://xx.zhonguo7118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://kk.zhonguo1118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://cb.zhonguo1118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://yo.zhonguo7118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://ew.zhonguo7118.cn

[F11] 复制与移动文件
来源：https://fn.zhonguo5118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://pa.zhonguo6118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://zz.zhonguo4118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ym.zhonguo7118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://my.zhonguo3118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://wc.zhonguo5118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://ju.zhonguo5118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://kg.zhonguo6118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://ry.zhonguo7118.cn

[F12] CSV 读写
来源：https://ev.zhonguo1118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://tj.zhonguo4118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://uh.zhonguo2118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://fc.zhonguo8118.cn

TS:   // 同上
来源：https://cl.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://kp.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://vp.zhonguo1118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://qx.zhonguo5118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://om.zhonguo3118.cn

================================================================================
来源：https://xi.zhonguo6118.cn

G. 面向对象
来源：https://xa.zhonguo7118.cn

================================================================================
来源：https://wn.zhonguo1118.cn

[G01] 定义类
来源：https://tc.zhonguo2118.cn

Py:   class User: pass
来源：https://zc.zhonguo4118.cn

PHP:  class User {}
来源：https://pc.zhonguo4118.cn

JS:   class User {}
来源：https://dm.zhonguo3118.cn

TS:   class User { name: string = ""; }
来源：https://xt.zhonguo1118.cn

Java: class User {}
来源：https://bb.zhonguo5118.cn

Go:   type User struct { Name string }
来源：https://zz.zhonguo7118.cn

Ruby: class User; end
来源：https://uq.zhonguo6118.cn

C#:   class User {}
来源：https://vu.zhonguo1118.cn

[G02] 构造函数
来源：https://fk.zhonguo5118.cn

Py:   def __init__(self, name): self.name = name
来源：https://ge.zhonguo7118.cn

PHP:  public function __construct(public string $name) {}
来源：https://lu.zhonguo7118.cn

JS:   constructor(name) { this.name = name; }
来源：https://es.zhonguo7118.cn

TS:   constructor(public name: string) {}
来源：https://oj.zhonguo6118.cn

Java: User(String name) { this.name = name; }
来源：https://qz.zhonguo4118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://uw.zhonguo8118.cn

Ruby: def initialize(name); @name = name; end
来源：https://tz.zhonguo8118.cn

C#:   public User(string name) { Name = name; }
来源：https://ex.zhonguo2118.cn

[G03] 实例属性
来源：https://sm.zhonguo3118.cn

Py:   self.name = "x"
来源：https://ex.zhonguo7118.cn

PHP:  public string $name = "x";
来源：https://bi.zhonguo6118.cn

JS:   this.name = "x";
来源：https://hx.zhonguo2118.cn

TS:   name: string = "x";
来源：https://rp.zhonguo8118.cn

Java: private String name;
来源：https://ag.zhonguo1118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://vu.zhonguo1118.cn

Ruby: @name = "x"
来源：https://zi.zhonguo3118.cn

C#:   public string Name { get; set; } = "x";
来源：https://pb.zhonguo6118.cn

[G04] 定义方法
来源：https://pc.zhonguo3118.cn

Py:   def greet(self): return self.name
来源：https://qd.zhonguo1118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://pg.zhonguo8118.cn

JS:   greet() { return this.name; }
来源：https://kt.zhonguo2118.cn

TS:   greet(): string { return this.name; }
来源：https://ds.zhonguo8118.cn

Java: String greet() { return name; }
来源：https://mw.zhonguo8118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://tb.zhonguo1118.cn

Ruby: def greet; @name; end
来源：https://kc.zhonguo7118.cn

C#:   public string Greet() => Name;
来源：https://kh.zhonguo7118.cn

[G05] 继承
来源：https://wt.zhonguo5118.cn

Py:   class Admin(User): pass
来源：https://fe.zhonguo4118.cn

PHP:  class Admin extends User {}
来源：https://yn.zhonguo4118.cn

JS:   class Admin extends User {}
来源：https://ih.zhonguo7118.cn

TS:   class Admin extends User {}
来源：https://tz.zhonguo8118.cn

Java: class Admin extends User {}
来源：https://rg.zhonguo4118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://yy.zhonguo5118.cn

Ruby: class Admin < User; end
来源：https://sj.zhonguo3118.cn

C#:   class Admin : User {}
来源：https://oj.zhonguo8118.cn

[G06] 重写方法
来源：https://pe.zhonguo4118.cn

Py:   def greet(self): return "admin"
来源：https://mz.zhonguo8118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://iu.zhonguo5118.cn

JS:   greet() { return "admin"; }
来源：https://ux.zhonguo2118.cn

TS:   greet(): string { return "admin"; }
来源：https://nt.zhonguo6118.cn

Java: @Override String greet() { return "admin"; }
来源：https://da.zhonguo6118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://gt.zhonguo6118.cn

Ruby: def greet; "admin"; end
来源：https://wd.zhonguo1118.cn

C#:   public override string Greet() => "admin";
来源：https://jv.zhonguo7118.cn

[G07] 调用父类方法
来源：https://sj.zhonguo8118.cn

Py:   super().greet()
来源：https://jv.zhonguo4118.cn

PHP:  parent::greet();
来源：https://ln.zhonguo5118.cn

JS:   super.greet();
来源：https://np.zhonguo5118.cn

TS:   super.greet();
来源：https://kp.zhonguo6118.cn

Java: super.greet();
来源：https://he.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://xo.zhonguo1118.cn

Ruby: super
来源：https://xf.zhonguo2118.cn

C#:   base.Greet();
来源：https://mu.zhonguo1118.cn

[G08] 静态方法与属性
来源：https://bs.zhonguo8118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://dk.zhonguo2118.cn

PHP:  public static function f() {}
来源：https://mu.zhonguo8118.cn

JS:   static f() {}
来源：https://fd.zhonguo8118.cn

TS:   static f(): void {}
来源：https://fs.zhonguo5118.cn

Java: static void f() {}
来源：https://md.zhonguo8118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://dh.zhonguo5118.cn

Ruby: def self.f; end
来源：https://xz.zhonguo7118.cn

C#:   public static void F() {}
来源：https://gb.zhonguo8118.cn

[G09] 接口 / 抽象类
来源：https://nl.zhonguo6118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ux.zhonguo5118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://eo.zhonguo3118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://ty.zhonguo6118.cn

TS:   interface Shape { area(): number; }
来源：https://un.zhonguo6118.cn

Java: interface Shape { double area(); }
来源：https://mn.zhonguo5118.cn

Go:   type Shape interface { Area() float64 }
来源：https://kf.zhonguo1118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://ao.zhonguo6118.cn

C#:   interface IShape { double Area(); }
来源：https://of.zhonguo1118.cn

[G10] 访问控制
来源：https://gu.zhonguo3118.cn

Py:   约定 _protected / __private（不强制）
来源：https://ya.zhonguo5118.cn

PHP:  public / protected / private
来源：https://yx.zhonguo1118.cn

JS:   #private 字段；其余公开
来源：https://kz.zhonguo6118.cn

TS:   public / protected / private
来源：https://ih.zhonguo7118.cn

Java: public / protected / private / 默认包级
来源：https://ze.zhonguo4118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://vv.zhonguo1118.cn

Ruby: public / protected / private
来源：https://tb.zhonguo2118.cn

C#:   public / protected / private / internal
来源：https://jm.zhonguo5118.cn

[G11] getter / setter
来源：https://jh.zhonguo7118.cn

Py:   @property 与 @x.setter
来源：https://fv.zhonguo2118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://mg.zhonguo3118.cn

JS:   get name() { return this._name; }
来源：https://nw.zhonguo5118.cn

TS:   get name(): string { return this._name; }
来源：https://hg.zhonguo2118.cn

Java: public String getName() { return name; }
来源：https://yx.zhonguo7118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://jg.zhonguo5118.cn

Ruby: attr_accessor :name
来源：https://gc.zhonguo3118.cn

C#:   public string Name { get; set; }
来源：https://gi.zhonguo1118.cn

[G12] 对象转字符串
来源：https://dc.zhonguo7118.cn

Py:   def __str__(self): return self.name
来源：https://af.zhonguo3118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ie.zhonguo2118.cn

JS:   toString() { return this.name; }
来源：https://ah.zhonguo5118.cn

TS:   toString(): string { return this.name; }
来源：https://ap.zhonguo2118.cn

Java: @Override public String toString() { return name; }
来源：https://yt.zhonguo4118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://bp.zhonguo2118.cn

Ruby: def to_s; @name; end
来源：https://zz.zhonguo8118.cn

C#:   public override string ToString() => Name;
来源：https://yu.zhonguo7118.cn

[G13] 判断对象类型
来源：https://dp.zhonguo7118.cn

Py:   isinstance(u, User)
来源：https://gz.zhonguo2118.cn

PHP:  $u instanceof User
来源：https://qg.zhonguo6118.cn

JS:   u instanceof User
来源：https://bq.zhonguo2118.cn

TS:   u instanceof User
来源：https://za.zhonguo3118.cn

Java: u instanceof User
来源：https://fo.zhonguo7118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://bm.zhonguo3118.cn

Ruby: u.is_a?(User)
来源：https://ql.zhonguo5118.cn

C#:   u is User
来源：https://wa.zhonguo7118.cn

[G14] 数据类 / record
来源：https://sy.zhonguo2118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://dt.zhonguo8118.cn

PHP:  // 用 readonly 属性模拟
来源：https://kp.zhonguo2118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://tz.zhonguo5118.cn

TS:   type User = { name: string; age: number };
来源：https://ic.zhonguo1118.cn

Java: record User(String name, int age) {}
来源：https://zs.zhonguo1118.cn

Go:   type User struct { Name string; Age int }
来源：https://cm.zhonguo3118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://in.zhonguo1118.cn

C#:   record User(string Name, int Age);
来源：https://fp.zhonguo3118.cn

[G15] 枚举
来源：https://tk.zhonguo8118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://oo.zhonguo2118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://ra.zhonguo2118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://vf.zhonguo7118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://jf.zhonguo4118.cn

Java: enum Color { RED, GREEN }
来源：https://oq.zhonguo4118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://zk.zhonguo4118.cn

Ruby: Color = %i[red green].freeze
来源：https://dx.zhonguo2118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://vp.zhonguo8118.cn

[G16] 对象转数组 / 字典
来源：https://be.zhonguo4118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://uo.zhonguo1118.cn

PHP:  get_object_vars($obj);
来源：https://eu.zhonguo4118.cn

JS:   Object.entries(obj)
来源：https://sb.zhonguo3118.cn

TS:   Object.entries(obj)
来源：https://pl.zhonguo7118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://pe.zhonguo2118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://lq.zhonguo3118.cn

Ruby: obj.instance_variables
来源：https://zm.zhonguo8118.cn

C#:   // 用反射或 System.Text.Json
来源：https://gv.zhonguo2118.cn

================================================================================
来源：https://fl.zhonguo3118.cn

H. 异常与错误处理
来源：https://lz.zhonguo2118.cn

================================================================================
来源：https://un.zhonguo4118.cn

[H01] try / catch 基础
来源：https://nh.zhonguo7118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://no.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://lp.zhonguo4118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://uq.zhonguo7118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://ar.zhonguo8118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://of.zhonguo2118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://hb.zhonguo3118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://qq.zhonguo1118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://eq.zhonguo8118.cn

[H02] finally / ensure 收尾
来源：https://ij.zhonguo8118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://ez.zhonguo8118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://av.zhonguo2118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://ih.zhonguo8118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://az.zhonguo2118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://cd.zhonguo1118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://pk.zhonguo5118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://lc.zhonguo2118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://oz.zhonguo2118.cn

[H03] 主动抛出异常
来源：https://nl.zhonguo3118.cn

Py:   raise ValueError("错误信息")
来源：https://yv.zhonguo5118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ur.zhonguo3118.cn

JS:   throw new Error("错误信息");
来源：https://cg.zhonguo2118.cn

TS:   throw new Error("错误信息");
来源：https://wj.zhonguo3118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://nm.zhonguo2118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://qe.zhonguo4118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://yv.zhonguo2118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://kc.zhonguo7118.cn

[H04] 自定义异常类型
来源：https://ed.zhonguo8118.cn

Py:   class MyError(Exception): pass
来源：https://ku.zhonguo7118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://gq.zhonguo3118.cn

JS:   class MyError extends Error {}
来源：https://no.zhonguo6118.cn

TS:   class MyError extends Error {}
来源：https://uo.zhonguo3118.cn

Java: class MyException extends RuntimeException {}
来源：https://yy.zhonguo1118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://ae.zhonguo2118.cn

Ruby: class MyError < StandardError; end
来源：https://pr.zhonguo2118.cn

C#:   class MyException : Exception {}
来源：https://ml.zhonguo8118.cn

[H05] 捕获特定类型
来源：https://qo.zhonguo2118.cn

Py:   except ValueError as e:
来源：https://ef.zhonguo4118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://pb.zhonguo1118.cn

JS:   if (e instanceof TypeError) {}
来源：https://up.zhonguo3118.cn

TS:   if (e instanceof TypeError) {}
来源：https://ga.zhonguo1118.cn

Java: catch (IOException | SQLException e) {}
来源：https://gx.zhonguo7118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://ao.zhonguo8118.cn

Ruby: rescue ArgumentError => e
来源：https://qa.zhonguo8118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://ks.zhonguo5118.cn

[H06] 可选值 / 空值安全访问
来源：https://dx.zhonguo2118.cn

Py:   value = d.get("k") or default
来源：https://un.zhonguo6118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://lz.zhonguo1118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://we.zhonguo1118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://fo.zhonguo8118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://da.zhonguo1118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://wk.zhonguo6118.cn

Ruby: d&.dig(:a, :b)
来源：https://yw.zhonguo7118.cn

C#:   obj?.A?.B ?? default
来源：https://uq.zhonguo8118.cn

[H07] 断言
来源：https://cg.zhonguo6118.cn

Py:   assert x > 0, "必须为正"
来源：https://hk.zhonguo1118.cn

PHP:  assert($x > 0);
来源：https://gw.zhonguo6118.cn

JS:   console.assert(x > 0);
来源：https://kd.zhonguo4118.cn

TS:   console.assert(x > 0);
来源：https://ww.zhonguo3118.cn

Java: assert x > 0 : "必须为正";
来源：https://pc.zhonguo1118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://pi.zhonguo6118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://yz.zhonguo5118.cn

C#:   Debug.Assert(x > 0);
来源：https://sn.zhonguo1118.cn

[H08] 获取错误信息与堆栈
来源：https://lz.zhonguo3118.cn

Py:   str(e);  traceback.format_exc()
来源：https://lp.zhonguo7118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://zm.zhonguo2118.cn

JS:   e.message;  e.stack
来源：https://rr.zhonguo2118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://mv.zhonguo1118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://rb.zhonguo3118.cn

Go:   err.Error()
来源：https://ok.zhonguo6118.cn

Ruby: e.message;  e.backtrace
来源：https://kz.zhonguo1118.cn

C#:   e.Message;  e.StackTrace
来源：https://be.zhonguo6118.cn

[H09] 带错误码的异常
来源：https://jg.zhonguo2118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://xz.zhonguo7118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://db.zhonguo5118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://re.zhonguo1118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://rp.zhonguo3118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://ol.zhonguo3118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://io.zhonguo2118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://to.zhonguo1118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://dr.zhonguo7118.cn

[H10] 资源自动释放
来源：https://lg.zhonguo4118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://qf.zhonguo5118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://ca.zhonguo4118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://gn.zhonguo1118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://tg.zhonguo8118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://nl.zhonguo2118.cn

Go:   defer f.Close()
来源：https://yq.zhonguo6118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://dc.zhonguo7118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://kz.zhonguo2118.cn

================================================================================
来源：https://zd.zhonguo2118.cn

I. 正则表达式
来源：https://nf.zhonguo2118.cn

================================================================================
来源：https://ud.zhonguo1118.cn

[I01] 判断是否匹配
来源：https://kw.zhonguo2118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://vt.zhonguo2118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://rs.zhonguo8118.cn

JS:   /\d+/.test(s)
来源：https://tx.zhonguo6118.cn

TS:   /\d+/.test(s)
来源：https://nq.zhonguo7118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://ae.zhonguo4118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://oq.zhonguo2118.cn

Ruby: s.match?(/\d+/)
来源：https://ae.zhonguo3118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://bk.zhonguo3118.cn


<!-- 参考信息 -->