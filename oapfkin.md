代发 wailian999

[G06] 重写方法
来源：https://pd.zhonguo3118.cn

Py:   def greet(self): return "admin"
来源：https://wr.zhonguo1118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://bl.zhonguo1118.cn

JS:   greet() { return "admin"; }
来源：https://tp.zhonguo5118.cn

TS:   greet(): string { return "admin"; }
来源：https://mu.zhonguo6118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ub.zhonguo7118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://uw.zhonguo2118.cn

Ruby: def greet; "admin"; end
来源：https://if.zhonguo4118.cn

C#:   public override string Greet() => "admin";
来源：https://du.zhonguo8118.cn

[G07] 调用父类方法
来源：https://ts.zhonguo5118.cn

Py:   super().greet()
来源：https://oa.zhonguo2118.cn

PHP:  parent::greet();
来源：https://dq.zhonguo8118.cn

JS:   super.greet();
来源：https://ru.zhonguo1118.cn

TS:   super.greet();
来源：https://ot.zhonguo3118.cn

Java: super.greet();
来源：https://qx.zhonguo8118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://bm.zhonguo2118.cn

Ruby: super
来源：https://qu.zhonguo4118.cn

C#:   base.Greet();
来源：https://io.zhonguo5118.cn

[G08] 静态方法与属性
来源：https://xv.zhonguo6118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://cm.zhonguo5118.cn

PHP:  public static function f() {}
来源：https://co.zhonguo8118.cn

JS:   static f() {}
来源：https://cd.zhonguo6118.cn

TS:   static f(): void {}
来源：https://pl.zhonguo3118.cn

Java: static void f() {}
来源：https://yo.zhonguo7118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://yg.zhonguo8118.cn

Ruby: def self.f; end
来源：https://fr.zhonguo7118.cn

C#:   public static void F() {}
来源：https://rk.zhonguo1118.cn

[G09] 接口 / 抽象类
来源：https://jv.zhonguo1118.cn

Py:   from abc import ABC, abstractmethod
来源：https://vo.zhonguo3118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://fi.zhonguo7118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://pd.zhonguo8118.cn

TS:   interface Shape { area(): number; }
来源：https://tu.zhonguo4118.cn

Java: interface Shape { double area(); }
来源：https://dq.zhonguo3118.cn

Go:   type Shape interface { Area() float64 }
来源：https://su.zhonguo3118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://yd.zhonguo5118.cn

C#:   interface IShape { double Area(); }
来源：https://as.zhonguo7118.cn

[G10] 访问控制
来源：https://cj.zhonguo5118.cn

Py:   约定 _protected / __private（不强制）
来源：https://ou.zhonguo7118.cn

PHP:  public / protected / private
来源：https://im.zhonguo1118.cn

JS:   #private 字段；其余公开
来源：https://ox.zhonguo5118.cn

TS:   public / protected / private
来源：https://cl.zhonguo3118.cn

Java: public / protected / private / 默认包级
来源：https://et.zhonguo2118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://dc.zhonguo8118.cn

Ruby: public / protected / private
来源：https://gh.zhonguo7118.cn

C#:   public / protected / private / internal
来源：https://xf.zhonguo2118.cn

[G11] getter / setter
来源：https://mw.zhonguo8118.cn

Py:   @property 与 @x.setter
来源：https://tk.zhonguo3118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://wo.zhonguo6118.cn

JS:   get name() { return this._name; }
来源：https://zh.zhonguo8118.cn

TS:   get name(): string { return this._name; }
来源：https://uu.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://yc.zhonguo3118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://jk.zhonguo1118.cn

Ruby: attr_accessor :name
来源：https://sd.zhonguo5118.cn

C#:   public string Name { get; set; }
来源：https://vz.zhonguo2118.cn

[G12] 对象转字符串
来源：https://zm.zhonguo4118.cn

Py:   def __str__(self): return self.name
来源：https://bj.zhonguo1118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://eh.zhonguo4118.cn

JS:   toString() { return this.name; }
来源：https://dk.zhonguo8118.cn

TS:   toString(): string { return this.name; }
来源：https://bo.zhonguo8118.cn

Java: @Override public String toString() { return name; }
来源：https://ku.zhonguo1118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://mm.zhonguo6118.cn

Ruby: def to_s; @name; end
来源：https://pu.zhonguo8118.cn

C#:   public override string ToString() => Name;
来源：https://um.zhonguo5118.cn

[G13] 判断对象类型
来源：https://xk.zhonguo4118.cn

Py:   isinstance(u, User)
来源：https://lt.zhonguo7118.cn

PHP:  $u instanceof User
来源：https://tg.zhonguo8118.cn

JS:   u instanceof User
来源：https://df.zhonguo4118.cn

TS:   u instanceof User
来源：https://ju.zhonguo4118.cn

Java: u instanceof User
来源：https://mc.zhonguo1118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ly.zhonguo8118.cn

Ruby: u.is_a?(User)
来源：https://th.zhonguo1118.cn

C#:   u is User
来源：https://ko.zhonguo7118.cn

[G14] 数据类 / record
来源：https://se.zhonguo4118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://bf.zhonguo3118.cn

PHP:  // 用 readonly 属性模拟
来源：https://xv.zhonguo4118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://yh.zhonguo4118.cn

TS:   type User = { name: string; age: number };
来源：https://eo.zhonguo8118.cn

Java: record User(String name, int age) {}
来源：https://ft.zhonguo4118.cn

Go:   type User struct { Name string; Age int }
来源：https://ze.zhonguo8118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://wm.zhonguo7118.cn

C#:   record User(string Name, int Age);
来源：https://ic.zhonguo6118.cn

[G15] 枚举
来源：https://na.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://ch.zhonguo1118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://df.zhonguo4118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://yg.zhonguo7118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://ue.zhonguo6118.cn

Java: enum Color { RED, GREEN }
来源：https://og.zhonguo4118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://ju.zhonguo7118.cn

Ruby: Color = %i[red green].freeze
来源：https://bw.zhonguo4118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://ex.zhonguo8118.cn

[G16] 对象转数组 / 字典
来源：https://ry.zhonguo5118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ld.zhonguo5118.cn

PHP:  get_object_vars($obj);
来源：https://mf.zhonguo1118.cn

JS:   Object.entries(obj)
来源：https://lm.zhonguo8118.cn

TS:   Object.entries(obj)
来源：https://zk.zhonguo2118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://ng.zhonguo7118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://bz.zhonguo7118.cn

Ruby: obj.instance_variables
来源：https://xw.zhonguo2118.cn

C#:   // 用反射或 System.Text.Json
来源：https://na.zhonguo7118.cn

================================================================================
来源：https://sc.zhonguo8118.cn

H. 异常与错误处理
来源：https://aw.zhonguo3118.cn

================================================================================
来源：https://dj.zhonguo7118.cn

[H01] try / catch 基础
来源：https://xr.zhonguo1118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://fw.zhonguo5118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://fs.zhonguo2118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://fs.zhonguo7118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://uk.zhonguo5118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://qg.zhonguo3118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://bd.zhonguo5118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://eh.zhonguo7118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://xc.zhonguo6118.cn

[H02] finally / ensure 收尾
来源：https://mw.zhonguo7118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://cd.zhonguo3118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://mq.zhonguo6118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://vx.zhonguo8118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://vm.zhonguo6118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://qr.zhonguo5118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://am.zhonguo1118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://nw.zhonguo3118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://ge.zhonguo3118.cn

[H03] 主动抛出异常
来源：https://wa.zhonguo7118.cn

Py:   raise ValueError("错误信息")
来源：https://mc.zhonguo4118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ji.zhonguo5118.cn

JS:   throw new Error("错误信息");
来源：https://ie.zhonguo7118.cn

TS:   throw new Error("错误信息");
来源：https://cc.zhonguo5118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://zn.zhonguo1118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://la.zhonguo5118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ew.zhonguo5118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://pd.zhonguo8118.cn

[H04] 自定义异常类型
来源：https://qs.zhonguo6118.cn

Py:   class MyError(Exception): pass
来源：https://si.zhonguo3118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://gy.zhonguo3118.cn

JS:   class MyError extends Error {}
来源：https://xo.zhonguo3118.cn

TS:   class MyError extends Error {}
来源：https://ov.zhonguo4118.cn

Java: class MyException extends RuntimeException {}
来源：https://bw.zhonguo2118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://cf.zhonguo2118.cn

Ruby: class MyError < StandardError; end
来源：https://rf.zhonguo4118.cn

C#:   class MyException : Exception {}
来源：https://ph.zhonguo4118.cn

[H05] 捕获特定类型
来源：https://kk.zhonguo8118.cn

Py:   except ValueError as e:
来源：https://rj.zhonguo3118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://zt.zhonguo5118.cn

JS:   if (e instanceof TypeError) {}
来源：https://ub.zhonguo4118.cn

TS:   if (e instanceof TypeError) {}
来源：https://hy.zhonguo3118.cn

Java: catch (IOException | SQLException e) {}
来源：https://vy.zhonguo2118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://dg.zhonguo6118.cn

Ruby: rescue ArgumentError => e
来源：https://pj.zhonguo7118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://vm.zhonguo5118.cn

[H06] 可选值 / 空值安全访问
来源：https://bs.zhonguo5118.cn

Py:   value = d.get("k") or default
来源：https://rr.zhonguo5118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://zj.zhonguo8118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://ml.zhonguo2118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://ij.zhonguo1118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://cg.zhonguo7118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://nn.zhonguo6118.cn

Ruby: d&.dig(:a, :b)
来源：https://nq.zhonguo1118.cn

C#:   obj?.A?.B ?? default
来源：https://cn.zhonguo1118.cn

[H07] 断言
来源：https://ww.zhonguo3118.cn

Py:   assert x > 0, "必须为正"
来源：https://tn.zhonguo3118.cn

PHP:  assert($x > 0);
来源：https://za.zhonguo6118.cn

JS:   console.assert(x > 0);
来源：https://ob.zhonguo5118.cn

TS:   console.assert(x > 0);
来源：https://rx.zhonguo3118.cn

Java: assert x > 0 : "必须为正";
来源：https://nv.zhonguo2118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://fj.zhonguo7118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://ie.zhonguo4118.cn

C#:   Debug.Assert(x > 0);
来源：https://uj.zhonguo1118.cn

[H08] 获取错误信息与堆栈
来源：https://yb.zhonguo3118.cn

Py:   str(e);  traceback.format_exc()
来源：https://mi.zhonguo4118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://em.zhonguo3118.cn

JS:   e.message;  e.stack
来源：https://bh.zhonguo2118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://qs.zhonguo5118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://cc.zhonguo6118.cn

Go:   err.Error()
来源：https://is.zhonguo7118.cn

Ruby: e.message;  e.backtrace
来源：https://km.zhonguo8118.cn

C#:   e.Message;  e.StackTrace
来源：https://qw.zhonguo3118.cn

[H09] 带错误码的异常
来源：https://vp.zhonguo5118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://fa.zhonguo8118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://to.zhonguo5118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://bc.zhonguo7118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://di.zhonguo2118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://an.zhonguo7118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://wx.zhonguo6118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://sg.zhonguo5118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://pe.zhonguo5118.cn

[H10] 资源自动释放
来源：https://wm.zhonguo2118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://sp.zhonguo1118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://pq.zhonguo5118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://mb.zhonguo6118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://sb.zhonguo1118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://ah.zhonguo1118.cn

Go:   defer f.Close()
来源：https://nw.zhonguo8118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://fb.zhonguo4118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://ut.zhonguo6118.cn

================================================================================
来源：https://oq.zhonguo4118.cn

I. 正则表达式
来源：https://to.zhonguo6118.cn

================================================================================
来源：https://jp.zhonguo4118.cn

[I01] 判断是否匹配
来源：https://je.zhonguo5118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://sl.zhonguo1118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://qq.zhonguo5118.cn

JS:   /\d+/.test(s)
来源：https://ka.zhonguo8118.cn

TS:   /\d+/.test(s)
来源：https://ps.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://xc.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://ud.zhonguo3118.cn

Ruby: s.match?(/\d+/)
来源：https://fj.zhonguo7118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://of.zhonguo5118.cn

[I02] 提取所有匹配
来源：https://ui.zhonguo5118.cn

Py:   re.findall(r"\d+", s)
来源：https://vl.zhonguo6118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://lc.zhonguo7118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://so.zhonguo4118.cn

TS:   s.match(/\d+/g)
来源：https://co.zhonguo7118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://xa.zhonguo2118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://tb.zhonguo8118.cn

Ruby: s.scan(/\d+/)
来源：https://lh.zhonguo7118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://ql.zhonguo5118.cn

[I03] 提取捕获分组
来源：https://sk.zhonguo6118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://am.zhonguo7118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://lg.zhonguo5118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://em.zhonguo4118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://gz.zhonguo1118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://kc.zhonguo6118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://gf.zhonguo4118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://bx.zhonguo6118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://yt.zhonguo8118.cn

[I04] 正则替换
来源：https://hj.zhonguo2118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://vz.zhonguo4118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://lu.zhonguo2118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://wx.zhonguo6118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://eg.zhonguo5118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://pf.zhonguo5118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://sr.zhonguo6118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://vk.zhonguo6118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://iu.zhonguo2118.cn

[I05] 按正则拆分
来源：https://fy.zhonguo4118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://up.zhonguo7118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://tf.zhonguo3118.cn

JS:   s.split(/\s*,\s*/)
来源：https://qc.zhonguo1118.cn

TS:   s.split(/\s*,\s*/)
来源：https://jb.zhonguo6118.cn

Java: s.split("\\s*,\\s*")
来源：https://ep.zhonguo7118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://we.zhonguo3118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://kb.zhonguo5118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://af.zhonguo7118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://yg.zhonguo1118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://yf.zhonguo2118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://br.zhonguo4118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://he.zhonguo3118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://pn.zhonguo4118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://tm.zhonguo6118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://yc.zhonguo1118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://cg.zhonguo7118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://wz.zhonguo8118.cn

[I07] 忽略大小写与多行模式
来源：https://lg.zhonguo2118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://ib.zhonguo3118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://yj.zhonguo1118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://kr.zhonguo4118.cn

TS:   /error/gim
来源：https://ec.zhonguo1118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://sv.zhonguo3118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://xk.zhonguo4118.cn

Ruby: s.scan(/error/i)
来源：https://nj.zhonguo4118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://rb.zhonguo3118.cn

[I08] 贪婪与非贪婪匹配
来源：https://ia.zhonguo2118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://de.zhonguo7118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://na.zhonguo7118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://je.zhonguo7118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://qf.zhonguo2118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://ps.zhonguo5118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://xk.zhonguo7118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://di.zhonguo8118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://ly.zhonguo6118.cn

================================================================================
来源：https://xy.zhonguo2118.cn

J. 日期与时间
来源：https://nu.zhonguo2118.cn

================================================================================
来源：https://pm.zhonguo4118.cn

[J01] 获取当前时间
来源：https://yi.zhonguo8118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://xl.zhonguo1118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://dn.zhonguo4118.cn

JS:   new Date();  Date.now()
来源：https://bi.zhonguo8118.cn

TS:   new Date();  Date.now()
来源：https://uy.zhonguo8118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://zj.zhonguo8118.cn

Go:   time.Now()
来源：https://in.zhonguo6118.cn

Ruby: Time.now
来源：https://xz.zhonguo1118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://on.zhonguo2118.cn

[J02] 格式化输出
来源：https://aq.zhonguo6118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://fn.zhonguo3118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://mu.zhonguo1118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://dm.zhonguo2118.cn

TS:   d.toISOString()
来源：https://sz.zhonguo7118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://ii.zhonguo6118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://dn.zhonguo5118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://ac.zhonguo5118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://ke.zhonguo5118.cn

[J03] 字符串解析为日期
来源：https://sx.zhonguo8118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://fc.zhonguo2118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://qr.zhonguo1118.cn

JS:   new Date("2024-01-02")
来源：https://dm.zhonguo5118.cn

TS:   new Date("2024-01-02")
来源：https://fa.zhonguo6118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://bi.zhonguo2118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://nb.zhonguo8118.cn

Ruby: Date.parse("2024-01-02")
来源：https://mp.zhonguo1118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://ih.zhonguo6118.cn

[J04] 时间戳与日期互转
来源：https://aj.zhonguo5118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://yo.zhonguo7118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://zl.zhonguo6118.cn


<!-- 参考信息 -->