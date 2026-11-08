代发 wailian999

C#:   public User(string name) { Name = name; }
来源：https://jg.zhonguo6118.cn

[G03] 实例属性
来源：https://ii.zhonguo1118.cn

Py:   self.name = "x"
来源：https://cw.zhonguo3118.cn

PHP:  public string $name = "x";
来源：https://ow.zhonguo8118.cn

JS:   this.name = "x";
来源：https://en.zhonguo2118.cn

TS:   name: string = "x";
来源：https://ca.zhonguo3118.cn

Java: private String name;
来源：https://sw.zhonguo1118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://md.zhonguo5118.cn

Ruby: @name = "x"
来源：https://yt.zhonguo8118.cn

C#:   public string Name { get; set; } = "x";
来源：https://ot.zhonguo2118.cn

[G04] 定义方法
来源：https://zo.zhonguo6118.cn

Py:   def greet(self): return self.name
来源：https://ps.zhonguo3118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://ar.zhonguo3118.cn

JS:   greet() { return this.name; }
来源：https://ge.zhonguo8118.cn

TS:   greet(): string { return this.name; }
来源：https://ut.zhonguo1118.cn

Java: String greet() { return name; }
来源：https://mm.zhonguo2118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://fe.zhonguo2118.cn

Ruby: def greet; @name; end
来源：https://mg.zhonguo3118.cn

C#:   public string Greet() => Name;
来源：https://th.zhonguo8118.cn

[G05] 继承
来源：https://dt.zhonguo3118.cn

Py:   class Admin(User): pass
来源：https://wm.zhonguo5118.cn

PHP:  class Admin extends User {}
来源：https://nt.zhonguo5118.cn

JS:   class Admin extends User {}
来源：https://ef.zhonguo1118.cn

TS:   class Admin extends User {}
来源：https://xz.zhonguo1118.cn

Java: class Admin extends User {}
来源：https://eq.zhonguo7118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://gt.zhonguo1118.cn

Ruby: class Admin < User; end
来源：https://an.zhonguo6118.cn

C#:   class Admin : User {}
来源：https://xe.zhonguo8118.cn

[G06] 重写方法
来源：https://dd.zhonguo7118.cn

Py:   def greet(self): return "admin"
来源：https://eu.zhonguo1118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://sa.zhonguo6118.cn

JS:   greet() { return "admin"; }
来源：https://fd.zhonguo1118.cn

TS:   greet(): string { return "admin"; }
来源：https://lv.zhonguo2118.cn

Java: @Override String greet() { return "admin"; }
来源：https://id.zhonguo8118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://zj.zhonguo5118.cn

Ruby: def greet; "admin"; end
来源：https://yo.zhonguo3118.cn

C#:   public override string Greet() => "admin";
来源：https://ue.zhonguo6118.cn

[G07] 调用父类方法
来源：https://ew.zhonguo7118.cn

Py:   super().greet()
来源：https://kv.zhonguo7118.cn

PHP:  parent::greet();
来源：https://kz.zhonguo1118.cn

JS:   super.greet();
来源：https://es.zhonguo5118.cn

TS:   super.greet();
来源：https://tz.zhonguo6118.cn

Java: super.greet();
来源：https://fd.zhonguo1118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://ef.zhonguo4118.cn

Ruby: super
来源：https://vc.zhonguo2118.cn

C#:   base.Greet();
来源：https://ab.zhonguo3118.cn

[G08] 静态方法与属性
来源：https://mz.zhonguo6118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://mj.zhonguo7118.cn

PHP:  public static function f() {}
来源：https://qr.zhonguo5118.cn

JS:   static f() {}
来源：https://vt.zhonguo1118.cn

TS:   static f(): void {}
来源：https://mj.zhonguo5118.cn

Java: static void f() {}
来源：https://kw.zhonguo2118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://yt.zhonguo7118.cn

Ruby: def self.f; end
来源：https://so.zhonguo5118.cn

C#:   public static void F() {}
来源：https://eo.zhonguo5118.cn

[G09] 接口 / 抽象类
来源：https://hc.zhonguo8118.cn

Py:   from abc import ABC, abstractmethod
来源：https://dj.zhonguo3118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://it.zhonguo6118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://hp.zhonguo4118.cn

TS:   interface Shape { area(): number; }
来源：https://bj.zhonguo7118.cn

Java: interface Shape { double area(); }
来源：https://eu.zhonguo7118.cn

Go:   type Shape interface { Area() float64 }
来源：https://js.zhonguo1118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://hd.zhonguo5118.cn

C#:   interface IShape { double Area(); }
来源：https://bc.zhonguo7118.cn

[G10] 访问控制
来源：https://rn.zhonguo3118.cn

Py:   约定 _protected / __private（不强制）
来源：https://rz.zhonguo1118.cn

PHP:  public / protected / private
来源：https://it.zhonguo4118.cn

JS:   #private 字段；其余公开
来源：https://pg.zhonguo3118.cn

TS:   public / protected / private
来源：https://kg.zhonguo7118.cn

Java: public / protected / private / 默认包级
来源：https://ze.zhonguo4118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://ya.zhonguo4118.cn

Ruby: public / protected / private
来源：https://cu.zhonguo2118.cn

C#:   public / protected / private / internal
来源：https://vy.zhonguo6118.cn

[G11] getter / setter
来源：https://ph.zhonguo6118.cn

Py:   @property 与 @x.setter
来源：https://gk.zhonguo1118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://ar.zhonguo6118.cn

JS:   get name() { return this._name; }
来源：https://gx.zhonguo6118.cn

TS:   get name(): string { return this._name; }
来源：https://av.zhonguo8118.cn

Java: public String getName() { return name; }
来源：https://tq.zhonguo3118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://hc.zhonguo1118.cn

Ruby: attr_accessor :name
来源：https://ix.zhonguo7118.cn

C#:   public string Name { get; set; }
来源：https://ff.zhonguo2118.cn

[G12] 对象转字符串
来源：https://pv.zhonguo3118.cn

Py:   def __str__(self): return self.name
来源：https://qi.zhonguo5118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://xz.zhonguo8118.cn

JS:   toString() { return this.name; }
来源：https://md.zhonguo7118.cn

TS:   toString(): string { return this.name; }
来源：https://dn.zhonguo3118.cn

Java: @Override public String toString() { return name; }
来源：https://xx.zhonguo6118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://en.zhonguo6118.cn

Ruby: def to_s; @name; end
来源：https://uo.zhonguo3118.cn

C#:   public override string ToString() => Name;
来源：https://ho.zhonguo4118.cn

[G13] 判断对象类型
来源：https://ot.zhonguo5118.cn

Py:   isinstance(u, User)
来源：https://nb.zhonguo5118.cn

PHP:  $u instanceof User
来源：https://eo.zhonguo7118.cn

JS:   u instanceof User
来源：https://tp.zhonguo6118.cn

TS:   u instanceof User
来源：https://ya.zhonguo1118.cn

Java: u instanceof User
来源：https://rn.zhonguo5118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ey.zhonguo6118.cn

Ruby: u.is_a?(User)
来源：https://xp.zhonguo2118.cn

C#:   u is User
来源：https://ad.zhonguo4118.cn

[G14] 数据类 / record
来源：https://zw.zhonguo3118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://xp.zhonguo5118.cn

PHP:  // 用 readonly 属性模拟
来源：https://fa.zhonguo3118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://ib.zhonguo3118.cn

TS:   type User = { name: string; age: number };
来源：https://zn.zhonguo6118.cn

Java: record User(String name, int age) {}
来源：https://xa.zhonguo8118.cn

Go:   type User struct { Name string; Age int }
来源：https://so.zhonguo3118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://nq.zhonguo4118.cn

C#:   record User(string Name, int Age);
来源：https://kp.zhonguo7118.cn

[G15] 枚举
来源：https://at.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://mc.zhonguo7118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://hv.zhonguo5118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://zu.zhonguo5118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://or.zhonguo1118.cn

Java: enum Color { RED, GREEN }
来源：https://xe.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://gt.zhonguo2118.cn

Ruby: Color = %i[red green].freeze
来源：https://gk.zhonguo6118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://jo.zhonguo8118.cn

[G16] 对象转数组 / 字典
来源：https://ww.zhonguo5118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://kq.zhonguo3118.cn

PHP:  get_object_vars($obj);
来源：https://yk.zhonguo2118.cn

JS:   Object.entries(obj)
来源：https://fw.zhonguo1118.cn

TS:   Object.entries(obj)
来源：https://yq.zhonguo7118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://qi.zhonguo7118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://wk.zhonguo5118.cn

Ruby: obj.instance_variables
来源：https://du.zhonguo4118.cn

C#:   // 用反射或 System.Text.Json
来源：https://tp.zhonguo1118.cn

================================================================================
来源：https://ih.zhonguo3118.cn

H. 异常与错误处理
来源：https://uc.zhonguo1118.cn

================================================================================
来源：https://vf.zhonguo7118.cn

[H01] try / catch 基础
来源：https://kp.zhonguo3118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://qh.zhonguo5118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://bj.zhonguo5118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://pf.zhonguo5118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://zv.zhonguo2118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://cb.zhonguo7118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://nx.zhonguo7118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://zk.zhonguo5118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://yo.zhonguo4118.cn

[H02] finally / ensure 收尾
来源：https://vv.zhonguo3118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://bf.zhonguo2118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://es.zhonguo2118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://se.zhonguo4118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://hq.zhonguo6118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://ca.zhonguo5118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://xm.zhonguo1118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://zd.zhonguo4118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://ki.zhonguo2118.cn

[H03] 主动抛出异常
来源：https://gk.zhonguo6118.cn

Py:   raise ValueError("错误信息")
来源：https://rq.zhonguo8118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://nj.zhonguo1118.cn

JS:   throw new Error("错误信息");
来源：https://oe.zhonguo1118.cn

TS:   throw new Error("错误信息");
来源：https://zs.zhonguo5118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://wt.zhonguo6118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://wm.zhonguo2118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://hi.zhonguo3118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://db.zhonguo4118.cn

[H04] 自定义异常类型
来源：https://rj.zhonguo8118.cn

Py:   class MyError(Exception): pass
来源：https://lr.zhonguo6118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://tx.zhonguo3118.cn

JS:   class MyError extends Error {}
来源：https://yz.zhonguo6118.cn

TS:   class MyError extends Error {}
来源：https://fw.zhonguo6118.cn

Java: class MyException extends RuntimeException {}
来源：https://kj.zhonguo5118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://cs.zhonguo8118.cn

Ruby: class MyError < StandardError; end
来源：https://fx.zhonguo3118.cn

C#:   class MyException : Exception {}
来源：https://np.zhonguo2118.cn

[H05] 捕获特定类型
来源：https://yq.zhonguo8118.cn

Py:   except ValueError as e:
来源：https://kj.zhonguo4118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://wy.zhonguo8118.cn

JS:   if (e instanceof TypeError) {}
来源：https://nl.zhonguo3118.cn

TS:   if (e instanceof TypeError) {}
来源：https://jb.zhonguo4118.cn

Java: catch (IOException | SQLException e) {}
来源：https://mv.zhonguo2118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://an.zhonguo3118.cn

Ruby: rescue ArgumentError => e
来源：https://vd.zhonguo8118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://sd.zhonguo4118.cn

[H06] 可选值 / 空值安全访问
来源：https://he.zhonguo2118.cn

Py:   value = d.get("k") or default
来源：https://pg.zhonguo5118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://nk.zhonguo4118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://vo.zhonguo5118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://kr.zhonguo4118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://xr.zhonguo4118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://cu.zhonguo6118.cn

Ruby: d&.dig(:a, :b)
来源：https://wp.zhonguo2118.cn

C#:   obj?.A?.B ?? default
来源：https://dg.zhonguo8118.cn

[H07] 断言
来源：https://am.zhonguo5118.cn

Py:   assert x > 0, "必须为正"
来源：https://le.zhonguo3118.cn

PHP:  assert($x > 0);
来源：https://rx.zhonguo6118.cn

JS:   console.assert(x > 0);
来源：https://fi.zhonguo6118.cn

TS:   console.assert(x > 0);
来源：https://hc.zhonguo1118.cn

Java: assert x > 0 : "必须为正";
来源：https://ab.zhonguo8118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://wa.zhonguo5118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://cn.zhonguo7118.cn

C#:   Debug.Assert(x > 0);
来源：https://ql.zhonguo6118.cn

[H08] 获取错误信息与堆栈
来源：https://dr.zhonguo8118.cn

Py:   str(e);  traceback.format_exc()
来源：https://na.zhonguo4118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://rk.zhonguo2118.cn

JS:   e.message;  e.stack
来源：https://we.zhonguo4118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://wo.zhonguo3118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://bg.zhonguo8118.cn

Go:   err.Error()
来源：https://gg.zhonguo2118.cn

Ruby: e.message;  e.backtrace
来源：https://tl.zhonguo4118.cn

C#:   e.Message;  e.StackTrace
来源：https://ra.zhonguo6118.cn

[H09] 带错误码的异常
来源：https://oe.zhonguo2118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://uv.zhonguo5118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://mr.zhonguo2118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://tv.zhonguo4118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://tq.zhonguo3118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://fs.zhonguo7118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://be.zhonguo2118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://ww.zhonguo2118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://qt.zhonguo2118.cn

[H10] 资源自动释放
来源：https://tc.zhonguo5118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://pa.zhonguo6118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://gh.zhonguo3118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://cc.zhonguo2118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://qf.zhonguo4118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://th.zhonguo1118.cn

Go:   defer f.Close()
来源：https://xv.zhonguo2118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://hb.zhonguo8118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://iz.zhonguo4118.cn

================================================================================
来源：https://ac.zhonguo3118.cn

I. 正则表达式
来源：https://wp.zhonguo5118.cn

================================================================================
来源：https://dx.zhonguo6118.cn

[I01] 判断是否匹配
来源：https://xq.zhonguo7118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://zd.zhonguo5118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://xd.zhonguo8118.cn

JS:   /\d+/.test(s)
来源：https://jb.zhonguo5118.cn

TS:   /\d+/.test(s)
来源：https://pm.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://sp.zhonguo3118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://kx.zhonguo5118.cn

Ruby: s.match?(/\d+/)
来源：https://za.zhonguo6118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://fj.zhonguo5118.cn

[I02] 提取所有匹配
来源：https://pq.zhonguo1118.cn

Py:   re.findall(r"\d+", s)
来源：https://kz.zhonguo3118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://ql.zhonguo2118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://kg.zhonguo6118.cn

TS:   s.match(/\d+/g)
来源：https://zf.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://zf.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://iz.zhonguo4118.cn

Ruby: s.scan(/\d+/)
来源：https://vf.zhonguo7118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://ae.zhonguo7118.cn

[I03] 提取捕获分组
来源：https://ar.zhonguo2118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://nn.zhonguo5118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://rh.zhonguo3118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://kq.zhonguo6118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://cv.zhonguo2118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://pq.zhonguo6118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://uh.zhonguo6118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://gl.zhonguo1118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://kj.zhonguo2118.cn

[I04] 正则替换
来源：https://ta.zhonguo7118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://lk.zhonguo1118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://wn.zhonguo5118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://fg.zhonguo1118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://je.zhonguo8118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://xi.zhonguo7118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://xd.zhonguo3118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://gu.zhonguo7118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://fc.zhonguo3118.cn

[I05] 按正则拆分
来源：https://fd.zhonguo2118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://mv.zhonguo5118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://fn.zhonguo7118.cn

JS:   s.split(/\s*,\s*/)
来源：https://kr.zhonguo7118.cn

TS:   s.split(/\s*,\s*/)
来源：https://mb.zhonguo8118.cn

Java: s.split("\\s*,\\s*")
来源：https://xq.zhonguo2118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://ao.zhonguo7118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://ky.zhonguo3118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://dy.zhonguo5118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://pa.zhonguo7118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://cw.zhonguo6118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://mk.zhonguo1118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://pu.zhonguo6118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://lm.zhonguo7118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://nt.zhonguo2118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://oz.zhonguo6118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://ck.zhonguo6118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://ii.zhonguo6118.cn

[I07] 忽略大小写与多行模式
来源：https://kg.zhonguo3118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://vl.zhonguo4118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://ja.zhonguo2118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://wm.zhonguo2118.cn

TS:   /error/gim
来源：https://pk.zhonguo8118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://po.zhonguo4118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://tb.zhonguo1118.cn

Ruby: s.scan(/error/i)
来源：https://ft.zhonguo3118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://jg.zhonguo1118.cn

[I08] 贪婪与非贪婪匹配
来源：https://ej.zhonguo2118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://zd.zhonguo6118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://kw.zhonguo3118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://wp.zhonguo6118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://kp.zhonguo5118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://ll.zhonguo3118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://mo.zhonguo1118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://xe.zhonguo7118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://sy.zhonguo3118.cn

================================================================================
来源：https://dp.zhonguo8118.cn

J. 日期与时间
来源：https://qo.zhonguo2118.cn

================================================================================
来源：https://ay.zhonguo5118.cn

[J01] 获取当前时间
来源：https://al.zhonguo8118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://cw.zhonguo8118.cn


<!-- 参考信息 -->