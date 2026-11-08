代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：https://pe.zhonguo1118.cn

JS:   greet() { return this.name; }
来源：https://kb.zhonguo4118.cn

TS:   greet(): string { return this.name; }
来源：https://oa.zhonguo4118.cn

Java: String greet() { return name; }
来源：https://ll.zhonguo5118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://ci.zhonguo6118.cn

Ruby: def greet; @name; end
来源：https://gq.zhonguo1118.cn

C#:   public string Greet() => Name;
来源：https://py.zhonguo2118.cn

[G05] 继承
来源：https://bi.zhonguo8118.cn

Py:   class Admin(User): pass
来源：https://wi.zhonguo3118.cn

PHP:  class Admin extends User {}
来源：https://ur.zhonguo8118.cn

JS:   class Admin extends User {}
来源：https://pu.zhonguo2118.cn

TS:   class Admin extends User {}
来源：https://fo.zhonguo6118.cn

Java: class Admin extends User {}
来源：https://jo.zhonguo7118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://wq.zhonguo8118.cn

Ruby: class Admin < User; end
来源：https://ym.zhonguo7118.cn

C#:   class Admin : User {}
来源：https://zx.zhonguo8118.cn

[G06] 重写方法
来源：https://ak.zhonguo7118.cn

Py:   def greet(self): return "admin"
来源：https://pn.zhonguo5118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://ep.zhonguo3118.cn

JS:   greet() { return "admin"; }
来源：https://kb.zhonguo2118.cn

TS:   greet(): string { return "admin"; }
来源：https://vw.zhonguo5118.cn

Java: @Override String greet() { return "admin"; }
来源：https://ph.zhonguo3118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://sf.zhonguo5118.cn

Ruby: def greet; "admin"; end
来源：https://bs.zhonguo7118.cn

C#:   public override string Greet() => "admin";
来源：https://iw.zhonguo2118.cn

[G07] 调用父类方法
来源：https://pw.zhonguo1118.cn

Py:   super().greet()
来源：https://dg.zhonguo3118.cn

PHP:  parent::greet();
来源：https://us.zhonguo6118.cn

JS:   super.greet();
来源：https://xg.zhonguo5118.cn

TS:   super.greet();
来源：https://mp.zhonguo2118.cn

Java: super.greet();
来源：https://mc.zhonguo1118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://gg.zhonguo4118.cn

Ruby: super
来源：https://os.zhonguo8118.cn

C#:   base.Greet();
来源：https://ff.zhonguo4118.cn

[G08] 静态方法与属性
来源：https://st.zhonguo4118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://xh.zhonguo5118.cn

PHP:  public static function f() {}
来源：https://vl.zhonguo8118.cn

JS:   static f() {}
来源：https://ua.zhonguo3118.cn

TS:   static f(): void {}
来源：https://gm.zhonguo1118.cn

Java: static void f() {}
来源：https://ib.zhonguo4118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://br.zhonguo1118.cn

Ruby: def self.f; end
来源：https://sc.zhonguo3118.cn

C#:   public static void F() {}
来源：https://qp.zhonguo7118.cn

[G09] 接口 / 抽象类
来源：https://jc.zhonguo2118.cn

Py:   from abc import ABC, abstractmethod
来源：https://pf.zhonguo5118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://en.zhonguo5118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://jg.zhonguo3118.cn

TS:   interface Shape { area(): number; }
来源：https://ij.zhonguo7118.cn

Java: interface Shape { double area(); }
来源：https://eq.zhonguo8118.cn

Go:   type Shape interface { Area() float64 }
来源：https://vf.zhonguo7118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://ep.zhonguo2118.cn

C#:   interface IShape { double Area(); }
来源：https://yn.zhonguo3118.cn

[G10] 访问控制
来源：https://pn.zhonguo5118.cn

Py:   约定 _protected / __private（不强制）
来源：https://km.zhonguo4118.cn

PHP:  public / protected / private
来源：https://qh.zhonguo8118.cn

JS:   #private 字段；其余公开
来源：https://fh.zhonguo2118.cn

TS:   public / protected / private
来源：https://jj.zhonguo3118.cn

Java: public / protected / private / 默认包级
来源：https://rx.zhonguo6118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://er.zhonguo7118.cn

Ruby: public / protected / private
来源：https://jw.zhonguo5118.cn

C#:   public / protected / private / internal
来源：https://wh.zhonguo2118.cn

[G11] getter / setter
来源：https://rh.zhonguo4118.cn

Py:   @property 与 @x.setter
来源：https://ai.zhonguo3118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://ek.zhonguo5118.cn

JS:   get name() { return this._name; }
来源：https://mf.zhonguo1118.cn

TS:   get name(): string { return this._name; }
来源：https://je.zhonguo2118.cn

Java: public String getName() { return name; }
来源：https://rr.zhonguo7118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://rx.zhonguo1118.cn

Ruby: attr_accessor :name
来源：https://ma.zhonguo6118.cn

C#:   public string Name { get; set; }
来源：https://gx.zhonguo4118.cn

[G12] 对象转字符串
来源：https://fk.zhonguo7118.cn

Py:   def __str__(self): return self.name
来源：https://wu.zhonguo1118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ee.zhonguo2118.cn

JS:   toString() { return this.name; }
来源：https://ll.zhonguo7118.cn

TS:   toString(): string { return this.name; }
来源：https://bn.zhonguo8118.cn

Java: @Override public String toString() { return name; }
来源：https://sz.zhonguo3118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://pz.zhonguo7118.cn

Ruby: def to_s; @name; end
来源：https://ln.zhonguo2118.cn

C#:   public override string ToString() => Name;
来源：https://br.zhonguo1118.cn

[G13] 判断对象类型
来源：https://mr.zhonguo3118.cn

Py:   isinstance(u, User)
来源：https://vi.zhonguo2118.cn

PHP:  $u instanceof User
来源：https://il.zhonguo3118.cn

JS:   u instanceof User
来源：https://xa.zhonguo8118.cn

TS:   u instanceof User
来源：https://sq.zhonguo3118.cn

Java: u instanceof User
来源：https://bx.zhonguo7118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ft.zhonguo1118.cn

Ruby: u.is_a?(User)
来源：https://gs.zhonguo5118.cn

C#:   u is User
来源：https://of.zhonguo1118.cn

[G14] 数据类 / record
来源：https://ha.zhonguo3118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://pi.zhonguo2118.cn

PHP:  // 用 readonly 属性模拟
来源：https://xr.zhonguo6118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://ib.zhonguo4118.cn

TS:   type User = { name: string; age: number };
来源：https://nr.zhonguo2118.cn

Java: record User(String name, int age) {}
来源：https://xa.zhonguo6118.cn

Go:   type User struct { Name string; Age int }
来源：https://fi.zhonguo4118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://ml.zhonguo3118.cn

C#:   record User(string Name, int Age);
来源：https://kf.zhonguo6118.cn

[G15] 枚举
来源：https://rk.zhonguo6118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://wh.zhonguo4118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://hp.zhonguo8118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://mf.zhonguo4118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://iy.zhonguo1118.cn

Java: enum Color { RED, GREEN }
来源：https://wr.zhonguo1118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://mu.zhonguo2118.cn

Ruby: Color = %i[red green].freeze
来源：https://hn.zhonguo5118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://ft.zhonguo1118.cn

[G16] 对象转数组 / 字典
来源：https://bt.zhonguo6118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://bp.zhonguo1118.cn

PHP:  get_object_vars($obj);
来源：https://rn.zhonguo8118.cn

JS:   Object.entries(obj)
来源：https://ry.zhonguo6118.cn

TS:   Object.entries(obj)
来源：https://ik.zhonguo7118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://st.zhonguo7118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://qa.zhonguo7118.cn

Ruby: obj.instance_variables
来源：https://jg.zhonguo5118.cn

C#:   // 用反射或 System.Text.Json
来源：https://oz.zhonguo6118.cn

================================================================================
来源：https://gs.zhonguo7118.cn

H. 异常与错误处理
来源：https://yv.zhonguo2118.cn

================================================================================
来源：https://tp.zhonguo1118.cn

[H01] try / catch 基础
来源：https://qt.zhonguo5118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://pt.zhonguo5118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://kj.zhonguo4118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://ao.zhonguo6118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://ve.zhonguo8118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://av.zhonguo4118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://wc.zhonguo6118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://li.zhonguo7118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://pm.zhonguo8118.cn

[H02] finally / ensure 收尾
来源：https://jv.zhonguo6118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://ys.zhonguo6118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://ha.zhonguo3118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://as.zhonguo1118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://ok.zhonguo2118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://aw.zhonguo2118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://ik.zhonguo6118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://ww.zhonguo7118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://lw.zhonguo6118.cn

[H03] 主动抛出异常
来源：https://oj.zhonguo6118.cn

Py:   raise ValueError("错误信息")
来源：https://sd.zhonguo8118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://uo.zhonguo8118.cn

JS:   throw new Error("错误信息");
来源：https://ab.zhonguo4118.cn

TS:   throw new Error("错误信息");
来源：https://ak.zhonguo2118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://pk.zhonguo6118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://fq.zhonguo6118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ch.zhonguo7118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://ge.zhonguo8118.cn

[H04] 自定义异常类型
来源：https://ud.zhonguo1118.cn

Py:   class MyError(Exception): pass
来源：https://ti.zhonguo1118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://qw.zhonguo4118.cn

JS:   class MyError extends Error {}
来源：https://bd.zhonguo7118.cn

TS:   class MyError extends Error {}
来源：https://sj.zhonguo8118.cn

Java: class MyException extends RuntimeException {}
来源：https://zu.zhonguo5118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://lk.zhonguo2118.cn

Ruby: class MyError < StandardError; end
来源：https://qf.zhonguo5118.cn

C#:   class MyException : Exception {}
来源：https://ag.zhonguo4118.cn

[H05] 捕获特定类型
来源：https://sm.zhonguo3118.cn

Py:   except ValueError as e:
来源：https://mt.zhonguo8118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://in.zhonguo8118.cn

JS:   if (e instanceof TypeError) {}
来源：https://mj.zhonguo4118.cn

TS:   if (e instanceof TypeError) {}
来源：https://bg.zhonguo3118.cn

Java: catch (IOException | SQLException e) {}
来源：https://wx.zhonguo7118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://xe.zhonguo2118.cn

Ruby: rescue ArgumentError => e
来源：https://zu.zhonguo6118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://gz.zhonguo7118.cn

[H06] 可选值 / 空值安全访问
来源：https://zq.zhonguo7118.cn

Py:   value = d.get("k") or default
来源：https://mc.zhonguo2118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://qk.zhonguo5118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://fn.zhonguo4118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://wd.zhonguo4118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://gh.zhonguo5118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://op.zhonguo7118.cn

Ruby: d&.dig(:a, :b)
来源：https://tz.zhonguo2118.cn

C#:   obj?.A?.B ?? default
来源：https://xh.zhonguo5118.cn

[H07] 断言
来源：https://yz.zhonguo2118.cn

Py:   assert x > 0, "必须为正"
来源：https://js.zhonguo7118.cn

PHP:  assert($x > 0);
来源：https://zm.zhonguo3118.cn

JS:   console.assert(x > 0);
来源：https://bo.zhonguo6118.cn

TS:   console.assert(x > 0);
来源：https://tw.zhonguo5118.cn

Java: assert x > 0 : "必须为正";
来源：https://zj.zhonguo6118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://lv.zhonguo8118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://md.zhonguo5118.cn

C#:   Debug.Assert(x > 0);
来源：https://hk.zhonguo5118.cn

[H08] 获取错误信息与堆栈
来源：https://yc.zhonguo1118.cn

Py:   str(e);  traceback.format_exc()
来源：https://hs.zhonguo6118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://qs.zhonguo2118.cn

JS:   e.message;  e.stack
来源：https://gr.zhonguo1118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://fq.zhonguo7118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://xq.zhonguo4118.cn

Go:   err.Error()
来源：https://im.zhonguo3118.cn

Ruby: e.message;  e.backtrace
来源：https://md.zhonguo2118.cn

C#:   e.Message;  e.StackTrace
来源：https://dl.zhonguo1118.cn

[H09] 带错误码的异常
来源：https://hr.zhonguo4118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://pv.zhonguo1118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://ib.zhonguo5118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://ta.zhonguo2118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://uc.zhonguo1118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://yr.zhonguo8118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://me.zhonguo2118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://bl.zhonguo3118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://wl.zhonguo5118.cn

[H10] 资源自动释放
来源：https://jj.zhonguo8118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://hs.zhonguo7118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://le.zhonguo1118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://ad.zhonguo6118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://av.zhonguo8118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://gv.zhonguo2118.cn

Go:   defer f.Close()
来源：https://uq.zhonguo7118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://tz.zhonguo7118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://uj.zhonguo3118.cn

================================================================================
来源：https://cu.zhonguo1118.cn

I. 正则表达式
来源：https://tj.zhonguo2118.cn

================================================================================
来源：https://md.zhonguo7118.cn

[I01] 判断是否匹配
来源：https://np.zhonguo5118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://vj.zhonguo5118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://ha.zhonguo4118.cn

JS:   /\d+/.test(s)
来源：https://fz.zhonguo6118.cn

TS:   /\d+/.test(s)
来源：https://wq.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://lf.zhonguo1118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://ku.zhonguo8118.cn

Ruby: s.match?(/\d+/)
来源：https://xj.zhonguo4118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://ai.zhonguo2118.cn

[I02] 提取所有匹配
来源：https://ri.zhonguo6118.cn

Py:   re.findall(r"\d+", s)
来源：https://my.zhonguo6118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://ww.zhonguo2118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://ee.zhonguo3118.cn

TS:   s.match(/\d+/g)
来源：https://nr.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://ta.zhonguo3118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://vv.zhonguo8118.cn

Ruby: s.scan(/\d+/)
来源：https://te.zhonguo5118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://tq.zhonguo2118.cn

[I03] 提取捕获分组
来源：https://sy.zhonguo6118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://zb.zhonguo4118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://zk.zhonguo4118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://lv.zhonguo8118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://iq.zhonguo8118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://qq.zhonguo4118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://dl.zhonguo2118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://xc.zhonguo8118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://et.zhonguo5118.cn

[I04] 正则替换
来源：https://rd.zhonguo7118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://ts.zhonguo3118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://uw.zhonguo4118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://dh.zhonguo6118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://hl.zhonguo6118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://cy.zhonguo6118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://hs.zhonguo4118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://th.zhonguo5118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://pf.zhonguo3118.cn

[I05] 按正则拆分
来源：https://kx.zhonguo8118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://id.zhonguo1118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://hh.zhonguo3118.cn

JS:   s.split(/\s*,\s*/)
来源：https://wo.zhonguo4118.cn

TS:   s.split(/\s*,\s*/)
来源：https://vn.zhonguo3118.cn

Java: s.split("\\s*,\\s*")
来源：https://nj.zhonguo8118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://el.zhonguo4118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://nf.zhonguo6118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://ho.zhonguo5118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://mn.zhonguo7118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://cu.zhonguo8118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://in.zhonguo8118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://bq.zhonguo3118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://st.zhonguo7118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://jr.zhonguo2118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://lf.zhonguo7118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://ks.zhonguo7118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://ij.zhonguo6118.cn

[I07] 忽略大小写与多行模式
来源：https://gd.zhonguo7118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://tk.zhonguo8118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://dx.zhonguo7118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://jh.zhonguo5118.cn

TS:   /error/gim
来源：https://ap.zhonguo3118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://jd.zhonguo3118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://dn.zhonguo7118.cn

Ruby: s.scan(/error/i)
来源：https://hl.zhonguo6118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://af.zhonguo6118.cn

[I08] 贪婪与非贪婪匹配
来源：https://hd.zhonguo1118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://pn.zhonguo1118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://nx.zhonguo6118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://xv.zhonguo5118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://cj.zhonguo7118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://fg.zhonguo6118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://hh.zhonguo7118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://de.zhonguo1118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://fp.zhonguo4118.cn

================================================================================
来源：https://sx.zhonguo7118.cn

J. 日期与时间
来源：https://kq.zhonguo6118.cn

================================================================================
来源：https://qp.zhonguo7118.cn

[J01] 获取当前时间
来源：https://by.zhonguo6118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://eu.zhonguo1118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://qz.zhonguo7118.cn

JS:   new Date();  Date.now()
来源：https://ip.zhonguo2118.cn

TS:   new Date();  Date.now()
来源：https://vo.zhonguo4118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://yg.zhonguo8118.cn

Go:   time.Now()
来源：https://dc.zhonguo2118.cn

Ruby: Time.now
来源：https://bl.zhonguo1118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://pk.zhonguo1118.cn

[J02] 格式化输出
来源：https://tw.zhonguo4118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://xx.zhonguo2118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://of.zhonguo2118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://lz.zhonguo7118.cn

TS:   d.toISOString()
来源：https://zv.zhonguo2118.cn


<!-- 参考信息 -->