代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://yw.zhonguo1118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://ny.zhonguo7118.cn

Ruby: Dir.children("dir")
来源：https://vf.zhonguo4118.cn

C#:   Directory.GetFiles("dir")
来源：https://we.zhonguo7118.cn

[F09] 获取文件大小
来源：https://ej.zhonguo4118.cn

Py:   os.path.getsize("a.txt")
来源：https://fg.zhonguo6118.cn

PHP:  filesize("a.txt");
来源：https://eq.zhonguo5118.cn

JS:   fs.statSync("a.txt").size
来源：https://yc.zhonguo7118.cn

TS:   fs.statSync("a.txt").size
来源：https://nr.zhonguo7118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://cr.zhonguo2118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://cm.zhonguo5118.cn

Ruby: File.size("a.txt")
来源：https://aq.zhonguo6118.cn

C#:   new FileInfo("a.txt").Length
来源：https://oo.zhonguo4118.cn

[F10] 取文件扩展名 / 文件名
来源：https://ox.zhonguo7118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://kb.zhonguo6118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://ky.zhonguo8118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://cg.zhonguo3118.cn

TS:   path.extname("a.txt")
来源：https://kq.zhonguo7118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://sr.zhonguo5118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://nh.zhonguo8118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://ib.zhonguo1118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://nf.zhonguo4118.cn

[F11] 复制与移动文件
来源：https://mb.zhonguo1118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://ys.zhonguo3118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://ko.zhonguo7118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://sb.zhonguo6118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://pv.zhonguo1118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://dk.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://ou.zhonguo6118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://mt.zhonguo3118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://nk.zhonguo6118.cn

[F12] CSV 读写
来源：https://ml.zhonguo5118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://lk.zhonguo2118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://be.zhonguo3118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://fx.zhonguo8118.cn

TS:   // 同上
来源：https://qz.zhonguo2118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://li.zhonguo3118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://bq.zhonguo4118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://ig.zhonguo2118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://nz.zhonguo8118.cn

================================================================================
来源：https://op.zhonguo7118.cn

G. 面向对象
来源：https://tc.zhonguo4118.cn

================================================================================
来源：https://yd.zhonguo4118.cn

[G01] 定义类
来源：https://zc.zhonguo5118.cn

Py:   class User: pass
来源：https://xj.zhonguo2118.cn

PHP:  class User {}
来源：https://xo.zhonguo8118.cn

JS:   class User {}
来源：https://qm.zhonguo5118.cn

TS:   class User { name: string = ""; }
来源：https://xb.zhonguo5118.cn

Java: class User {}
来源：https://rm.zhonguo6118.cn

Go:   type User struct { Name string }
来源：https://tp.zhonguo2118.cn

Ruby: class User; end
来源：https://su.zhonguo6118.cn

C#:   class User {}
来源：https://pp.zhonguo7118.cn

[G02] 构造函数
来源：https://ad.zhonguo5118.cn

Py:   def __init__(self, name): self.name = name
来源：https://pv.zhonguo6118.cn

PHP:  public function __construct(public string $name) {}
来源：https://nf.zhonguo5118.cn

JS:   constructor(name) { this.name = name; }
来源：https://xj.zhonguo1118.cn

TS:   constructor(public name: string) {}
来源：https://zq.zhonguo8118.cn

Java: User(String name) { this.name = name; }
来源：https://gj.zhonguo2118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://sx.zhonguo8118.cn

Ruby: def initialize(name); @name = name; end
来源：https://ck.zhonguo4118.cn

C#:   public User(string name) { Name = name; }
来源：https://ta.zhonguo1118.cn

[G03] 实例属性
来源：https://tb.zhonguo6118.cn

Py:   self.name = "x"
来源：https://me.zhonguo7118.cn

PHP:  public string $name = "x";
来源：https://lp.zhonguo2118.cn

JS:   this.name = "x";
来源：https://wi.zhonguo5118.cn

TS:   name: string = "x";
来源：https://mu.zhonguo4118.cn

Java: private String name;
来源：https://ne.zhonguo8118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://td.zhonguo5118.cn

Ruby: @name = "x"
来源：https://pb.zhonguo6118.cn

C#:   public string Name { get; set; } = "x";
来源：https://uf.zhonguo1118.cn

[G04] 定义方法
来源：https://ie.zhonguo8118.cn

Py:   def greet(self): return self.name
来源：https://vj.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://de.zhonguo7118.cn

JS:   greet() { return this.name; }
来源：https://my.zhonguo8118.cn

TS:   greet(): string { return this.name; }
来源：https://zt.zhonguo5118.cn

Java: String greet() { return name; }
来源：https://ir.zhonguo3118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://xe.zhonguo1118.cn

Ruby: def greet; @name; end
来源：https://zc.zhonguo2118.cn

C#:   public string Greet() => Name;
来源：https://gj.zhonguo6118.cn

[G05] 继承
来源：https://ao.zhonguo1118.cn

Py:   class Admin(User): pass
来源：https://jn.zhonguo2118.cn

PHP:  class Admin extends User {}
来源：https://tr.zhonguo8118.cn

JS:   class Admin extends User {}
来源：https://ek.zhonguo5118.cn

TS:   class Admin extends User {}
来源：https://tw.zhonguo7118.cn

Java: class Admin extends User {}
来源：https://wq.zhonguo6118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://wy.zhonguo3118.cn

Ruby: class Admin < User; end
来源：https://ju.zhonguo8118.cn

C#:   class Admin : User {}
来源：https://dk.zhonguo2118.cn

[G06] 重写方法
来源：https://qs.zhonguo3118.cn

Py:   def greet(self): return "admin"
来源：https://ep.zhonguo7118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://wq.zhonguo5118.cn

JS:   greet() { return "admin"; }
来源：https://ul.zhonguo3118.cn

TS:   greet(): string { return "admin"; }
来源：https://hm.zhonguo1118.cn

Java: @Override String greet() { return "admin"; }
来源：https://oe.zhonguo5118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://up.zhonguo6118.cn

Ruby: def greet; "admin"; end
来源：https://uy.zhonguo6118.cn

C#:   public override string Greet() => "admin";
来源：https://tu.zhonguo1118.cn

[G07] 调用父类方法
来源：https://rk.zhonguo5118.cn

Py:   super().greet()
来源：https://tc.zhonguo2118.cn

PHP:  parent::greet();
来源：https://fs.zhonguo3118.cn

JS:   super.greet();
来源：https://lx.zhonguo1118.cn

TS:   super.greet();
来源：https://zy.zhonguo3118.cn

Java: super.greet();
来源：https://fl.zhonguo7118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://bq.zhonguo3118.cn

Ruby: super
来源：https://lv.zhonguo5118.cn

C#:   base.Greet();
来源：https://in.zhonguo4118.cn

[G08] 静态方法与属性
来源：https://sm.zhonguo4118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://nq.zhonguo8118.cn

PHP:  public static function f() {}
来源：https://si.zhonguo8118.cn

JS:   static f() {}
来源：https://bn.zhonguo5118.cn

TS:   static f(): void {}
来源：https://sw.zhonguo8118.cn

Java: static void f() {}
来源：https://be.zhonguo1118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://vf.zhonguo7118.cn

Ruby: def self.f; end
来源：https://wp.zhonguo6118.cn

C#:   public static void F() {}
来源：https://gw.zhonguo7118.cn

[G09] 接口 / 抽象类
来源：https://er.zhonguo3118.cn

Py:   from abc import ABC, abstractmethod
来源：https://lw.zhonguo3118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://io.zhonguo7118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://ta.zhonguo2118.cn

TS:   interface Shape { area(): number; }
来源：https://nk.zhonguo8118.cn

Java: interface Shape { double area(); }
来源：https://xg.zhonguo6118.cn

Go:   type Shape interface { Area() float64 }
来源：https://nb.zhonguo7118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://tc.zhonguo8118.cn

C#:   interface IShape { double Area(); }
来源：https://sb.zhonguo3118.cn

[G10] 访问控制
来源：https://vo.zhonguo5118.cn

Py:   约定 _protected / __private（不强制）
来源：https://aj.zhonguo1118.cn

PHP:  public / protected / private
来源：https://tl.zhonguo5118.cn

JS:   #private 字段；其余公开
来源：https://sr.zhonguo4118.cn

TS:   public / protected / private
来源：https://ho.zhonguo3118.cn

Java: public / protected / private / 默认包级
来源：https://li.zhonguo2118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://sv.zhonguo1118.cn

Ruby: public / protected / private
来源：https://zm.zhonguo5118.cn

C#:   public / protected / private / internal
来源：https://sn.zhonguo4118.cn

[G11] getter / setter
来源：https://xr.zhonguo2118.cn

Py:   @property 与 @x.setter
来源：https://nc.zhonguo3118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://tj.zhonguo2118.cn

JS:   get name() { return this._name; }
来源：https://be.zhonguo4118.cn

TS:   get name(): string { return this._name; }
来源：https://wm.zhonguo3118.cn

Java: public String getName() { return name; }
来源：https://xu.zhonguo7118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://ym.zhonguo5118.cn

Ruby: attr_accessor :name
来源：https://xz.zhonguo5118.cn

C#:   public string Name { get; set; }
来源：https://tr.zhonguo4118.cn

[G12] 对象转字符串
来源：https://qr.zhonguo8118.cn

Py:   def __str__(self): return self.name
来源：https://kj.zhonguo7118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://og.zhonguo6118.cn

JS:   toString() { return this.name; }
来源：https://ux.zhonguo1118.cn

TS:   toString(): string { return this.name; }
来源：https://ys.zhonguo8118.cn

Java: @Override public String toString() { return name; }
来源：https://at.zhonguo7118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://wg.zhonguo6118.cn

Ruby: def to_s; @name; end
来源：https://dn.zhonguo1118.cn

C#:   public override string ToString() => Name;
来源：https://go.zhonguo1118.cn

[G13] 判断对象类型
来源：https://xg.zhonguo4118.cn

Py:   isinstance(u, User)
来源：https://nb.zhonguo5118.cn

PHP:  $u instanceof User
来源：https://qr.zhonguo2118.cn

JS:   u instanceof User
来源：https://xu.zhonguo8118.cn

TS:   u instanceof User
来源：https://gi.zhonguo6118.cn

Java: u instanceof User
来源：https://rd.zhonguo1118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ug.zhonguo3118.cn

Ruby: u.is_a?(User)
来源：https://pr.zhonguo2118.cn

C#:   u is User
来源：https://ph.zhonguo8118.cn

[G14] 数据类 / record
来源：https://ny.zhonguo6118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://nb.zhonguo5118.cn

PHP:  // 用 readonly 属性模拟
来源：https://gt.zhonguo4118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://pb.zhonguo4118.cn

TS:   type User = { name: string; age: number };
来源：https://hb.zhonguo8118.cn

Java: record User(String name, int age) {}
来源：https://aj.zhonguo3118.cn

Go:   type User struct { Name string; Age int }
来源：https://pf.zhonguo6118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://qz.zhonguo3118.cn

C#:   record User(string Name, int Age);
来源：https://qx.zhonguo5118.cn

[G15] 枚举
来源：https://en.zhonguo2118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://en.zhonguo7118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://le.zhonguo4118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://yw.zhonguo5118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://qf.zhonguo3118.cn

Java: enum Color { RED, GREEN }
来源：https://zl.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://rg.zhonguo7118.cn

Ruby: Color = %i[red green].freeze
来源：https://lx.zhonguo3118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://bo.zhonguo3118.cn

[G16] 对象转数组 / 字典
来源：https://by.zhonguo4118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://lb.zhonguo7118.cn

PHP:  get_object_vars($obj);
来源：https://ic.zhonguo8118.cn

JS:   Object.entries(obj)
来源：https://xq.zhonguo4118.cn

TS:   Object.entries(obj)
来源：https://vv.zhonguo8118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://pq.zhonguo2118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://po.zhonguo7118.cn

Ruby: obj.instance_variables
来源：https://wp.zhonguo2118.cn

C#:   // 用反射或 System.Text.Json
来源：https://gz.zhonguo7118.cn

================================================================================
来源：https://dv.zhonguo7118.cn

H. 异常与错误处理
来源：https://dw.zhonguo2118.cn

================================================================================
来源：https://cq.zhonguo5118.cn

[H01] try / catch 基础
来源：https://tf.zhonguo7118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://iz.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://dh.zhonguo1118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://vf.zhonguo6118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://rr.zhonguo3118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://di.zhonguo4118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://rg.zhonguo4118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://po.zhonguo1118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://ap.zhonguo5118.cn

[H02] finally / ensure 收尾
来源：https://ii.zhonguo4118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://eu.zhonguo4118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://aj.zhonguo2118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://tg.zhonguo2118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://ih.zhonguo3118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://xk.zhonguo1118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://vk.zhonguo5118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://ld.zhonguo5118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://tt.zhonguo1118.cn

[H03] 主动抛出异常
来源：https://gm.zhonguo2118.cn

Py:   raise ValueError("错误信息")
来源：https://vn.zhonguo2118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://fv.zhonguo1118.cn

JS:   throw new Error("错误信息");
来源：https://vl.zhonguo8118.cn

TS:   throw new Error("错误信息");
来源：https://rk.zhonguo5118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://kr.zhonguo3118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://ei.zhonguo2118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://vn.zhonguo7118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://rp.zhonguo2118.cn

[H04] 自定义异常类型
来源：https://dm.zhonguo2118.cn

Py:   class MyError(Exception): pass
来源：https://gh.zhonguo6118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://nz.zhonguo8118.cn

JS:   class MyError extends Error {}
来源：https://ul.zhonguo4118.cn

TS:   class MyError extends Error {}
来源：https://il.zhonguo6118.cn

Java: class MyException extends RuntimeException {}
来源：https://ac.zhonguo1118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://mw.zhonguo4118.cn

Ruby: class MyError < StandardError; end
来源：https://ps.zhonguo5118.cn

C#:   class MyException : Exception {}
来源：https://ma.zhonguo4118.cn

[H05] 捕获特定类型
来源：https://il.zhonguo3118.cn

Py:   except ValueError as e:
来源：https://mv.zhonguo8118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://jq.zhonguo3118.cn

JS:   if (e instanceof TypeError) {}
来源：https://jc.zhonguo3118.cn

TS:   if (e instanceof TypeError) {}
来源：https://qg.zhonguo1118.cn

Java: catch (IOException | SQLException e) {}
来源：https://zm.zhonguo6118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://gx.zhonguo1118.cn

Ruby: rescue ArgumentError => e
来源：https://an.zhonguo3118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://tj.zhonguo2118.cn

[H06] 可选值 / 空值安全访问
来源：https://vj.zhonguo5118.cn

Py:   value = d.get("k") or default
来源：https://ku.zhonguo3118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://ca.zhonguo1118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://ue.zhonguo8118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://bc.zhonguo8118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://ou.zhonguo6118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://el.zhonguo2118.cn

Ruby: d&.dig(:a, :b)
来源：https://nw.zhonguo6118.cn

C#:   obj?.A?.B ?? default
来源：https://mn.zhonguo7118.cn

[H07] 断言
来源：https://ac.zhonguo3118.cn

Py:   assert x > 0, "必须为正"
来源：https://ew.zhonguo7118.cn

PHP:  assert($x > 0);
来源：https://fw.zhonguo4118.cn

JS:   console.assert(x > 0);
来源：https://gq.zhonguo7118.cn

TS:   console.assert(x > 0);
来源：https://pj.zhonguo3118.cn

Java: assert x > 0 : "必须为正";
来源：https://pu.zhonguo1118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://uw.zhonguo8118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://uc.zhonguo7118.cn

C#:   Debug.Assert(x > 0);
来源：https://pe.zhonguo2118.cn

[H08] 获取错误信息与堆栈
来源：https://lf.zhonguo6118.cn

Py:   str(e);  traceback.format_exc()
来源：https://wp.zhonguo8118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://ec.zhonguo4118.cn

JS:   e.message;  e.stack
来源：https://jf.zhonguo4118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://ey.zhonguo2118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://ca.zhonguo3118.cn

Go:   err.Error()
来源：https://yq.zhonguo3118.cn

Ruby: e.message;  e.backtrace
来源：https://lw.zhonguo7118.cn

C#:   e.Message;  e.StackTrace
来源：https://we.zhonguo5118.cn

[H09] 带错误码的异常
来源：https://vm.zhonguo2118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://lp.zhonguo7118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://eh.zhonguo8118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://wm.zhonguo2118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://if.zhonguo2118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://bd.zhonguo3118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://xa.zhonguo2118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://kj.zhonguo1118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://sc.zhonguo2118.cn

[H10] 资源自动释放
来源：https://gv.zhonguo2118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://yp.zhonguo1118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://ci.zhonguo3118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://rx.zhonguo2118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://ot.zhonguo3118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://xb.zhonguo8118.cn

Go:   defer f.Close()
来源：https://ll.zhonguo6118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://ts.zhonguo3118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://pk.zhonguo1118.cn

================================================================================
来源：https://fl.zhonguo2118.cn

I. 正则表达式
来源：https://rx.zhonguo3118.cn

================================================================================
来源：https://om.zhonguo4118.cn

[I01] 判断是否匹配
来源：https://oe.zhonguo1118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://kk.zhonguo8118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://bv.zhonguo1118.cn

JS:   /\d+/.test(s)
来源：https://ie.zhonguo4118.cn

TS:   /\d+/.test(s)
来源：https://pk.zhonguo3118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://lp.zhonguo2118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://zx.zhonguo6118.cn

Ruby: s.match?(/\d+/)
来源：https://uj.zhonguo1118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://gq.zhonguo7118.cn

[I02] 提取所有匹配
来源：https://je.zhonguo8118.cn

Py:   re.findall(r"\d+", s)
来源：https://pr.zhonguo8118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://xm.zhonguo4118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://jo.zhonguo7118.cn

TS:   s.match(/\d+/g)
来源：https://on.zhonguo1118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://mn.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://rd.zhonguo6118.cn

Ruby: s.scan(/\d+/)
来源：https://vj.zhonguo5118.cn


<!-- 参考信息 -->