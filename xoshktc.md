代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：https://pa.zhonguo8118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://pb.zhonguo7118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://gk.zhonguo7118.cn

TS:   interface Shape { area(): number; }
来源：https://nd.zhonguo1118.cn

Java: interface Shape { double area(); }
来源：https://en.zhonguo5118.cn

Go:   type Shape interface { Area() float64 }
来源：https://qg.zhonguo3118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://qw.zhonguo5118.cn

C#:   interface IShape { double Area(); }
来源：https://ts.zhonguo3118.cn

[G10] 访问控制
来源：https://rc.zhonguo4118.cn

Py:   约定 _protected / __private（不强制）
来源：https://fx.zhonguo4118.cn

PHP:  public / protected / private
来源：https://kt.zhonguo4118.cn

JS:   #private 字段；其余公开
来源：https://em.zhonguo8118.cn

TS:   public / protected / private
来源：https://sk.zhonguo2118.cn

Java: public / protected / private / 默认包级
来源：https://hi.zhonguo8118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://lo.zhonguo8118.cn

Ruby: public / protected / private
来源：https://sa.zhonguo7118.cn

C#:   public / protected / private / internal
来源：https://nb.zhonguo2118.cn

[G11] getter / setter
来源：https://ns.zhonguo8118.cn

Py:   @property 与 @x.setter
来源：https://rp.zhonguo5118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://zr.zhonguo6118.cn

JS:   get name() { return this._name; }
来源：https://iq.zhonguo3118.cn

TS:   get name(): string { return this._name; }
来源：https://xt.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://jt.zhonguo2118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://zo.zhonguo3118.cn

Ruby: attr_accessor :name
来源：https://vz.zhonguo4118.cn

C#:   public string Name { get; set; }
来源：https://ti.zhonguo7118.cn

[G12] 对象转字符串
来源：https://fu.zhonguo4118.cn

Py:   def __str__(self): return self.name
来源：https://mf.zhonguo4118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://wx.zhonguo4118.cn

JS:   toString() { return this.name; }
来源：https://pp.zhonguo2118.cn

TS:   toString(): string { return this.name; }
来源：https://ro.zhonguo4118.cn

Java: @Override public String toString() { return name; }
来源：https://es.zhonguo7118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://pt.zhonguo6118.cn

Ruby: def to_s; @name; end
来源：https://xr.zhonguo1118.cn

C#:   public override string ToString() => Name;
来源：https://by.zhonguo4118.cn

[G13] 判断对象类型
来源：https://vr.zhonguo1118.cn

Py:   isinstance(u, User)
来源：https://ax.zhonguo3118.cn

PHP:  $u instanceof User
来源：https://qe.zhonguo2118.cn

JS:   u instanceof User
来源：https://el.zhonguo6118.cn

TS:   u instanceof User
来源：https://pt.zhonguo4118.cn

Java: u instanceof User
来源：https://ob.zhonguo5118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://qd.zhonguo3118.cn

Ruby: u.is_a?(User)
来源：https://ok.zhonguo7118.cn

C#:   u is User
来源：https://ip.zhonguo3118.cn

[G14] 数据类 / record
来源：https://kn.zhonguo4118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://dl.zhonguo2118.cn

PHP:  // 用 readonly 属性模拟
来源：https://zb.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://dn.zhonguo8118.cn

TS:   type User = { name: string; age: number };
来源：https://pu.zhonguo5118.cn

Java: record User(String name, int age) {}
来源：https://aj.zhonguo5118.cn

Go:   type User struct { Name string; Age int }
来源：https://qf.zhonguo5118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://zs.zhonguo5118.cn

C#:   record User(string Name, int Age);
来源：https://eg.zhonguo8118.cn

[G15] 枚举
来源：https://pu.zhonguo1118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://qd.zhonguo3118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://ly.zhonguo2118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://gn.zhonguo1118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://dh.zhonguo7118.cn

Java: enum Color { RED, GREEN }
来源：https://hl.zhonguo1118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://ik.zhonguo4118.cn

Ruby: Color = %i[red green].freeze
来源：https://az.zhonguo6118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://sx.zhonguo4118.cn

[G16] 对象转数组 / 字典
来源：https://fc.zhonguo6118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ha.zhonguo6118.cn

PHP:  get_object_vars($obj);
来源：https://al.zhonguo4118.cn

JS:   Object.entries(obj)
来源：https://nm.zhonguo1118.cn

TS:   Object.entries(obj)
来源：https://iz.zhonguo1118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://yn.zhonguo1118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://xb.zhonguo5118.cn

Ruby: obj.instance_variables
来源：https://pw.zhonguo8118.cn

C#:   // 用反射或 System.Text.Json
来源：https://nj.zhonguo5118.cn

================================================================================
来源：https://mq.zhonguo1118.cn

H. 异常与错误处理
来源：https://mz.zhonguo8118.cn

================================================================================
来源：https://dc.zhonguo1118.cn

[H01] try / catch 基础
来源：https://ws.zhonguo4118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://ju.zhonguo3118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://go.zhonguo1118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://pt.zhonguo3118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://qz.zhonguo1118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://xy.zhonguo7118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://hn.zhonguo6118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://zd.zhonguo1118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://mo.zhonguo4118.cn

[H02] finally / ensure 收尾
来源：https://hv.zhonguo7118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://wo.zhonguo6118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://ku.zhonguo3118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://qc.zhonguo1118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://xb.zhonguo7118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://cf.zhonguo8118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://ji.zhonguo3118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://od.zhonguo6118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://zo.zhonguo6118.cn

[H03] 主动抛出异常
来源：https://zz.zhonguo5118.cn

Py:   raise ValueError("错误信息")
来源：https://pj.zhonguo6118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ob.zhonguo8118.cn

JS:   throw new Error("错误信息");
来源：https://ic.zhonguo5118.cn

TS:   throw new Error("错误信息");
来源：https://bz.zhonguo6118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://xj.zhonguo5118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://sd.zhonguo2118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ej.zhonguo7118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://cv.zhonguo2118.cn

[H04] 自定义异常类型
来源：https://xv.zhonguo6118.cn

Py:   class MyError(Exception): pass
来源：https://pi.zhonguo4118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://sf.zhonguo3118.cn

JS:   class MyError extends Error {}
来源：https://nj.zhonguo8118.cn

TS:   class MyError extends Error {}
来源：https://fk.zhonguo8118.cn

Java: class MyException extends RuntimeException {}
来源：https://fg.zhonguo8118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://qw.zhonguo8118.cn

Ruby: class MyError < StandardError; end
来源：https://gb.zhonguo4118.cn

C#:   class MyException : Exception {}
来源：https://oh.zhonguo7118.cn

[H05] 捕获特定类型
来源：https://kz.zhonguo5118.cn

Py:   except ValueError as e:
来源：https://gf.zhonguo8118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://xe.zhonguo4118.cn

JS:   if (e instanceof TypeError) {}
来源：https://uo.zhonguo1118.cn

TS:   if (e instanceof TypeError) {}
来源：https://yz.zhonguo5118.cn

Java: catch (IOException | SQLException e) {}
来源：https://yh.zhonguo2118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://ev.zhonguo5118.cn

Ruby: rescue ArgumentError => e
来源：https://py.zhonguo2118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://qy.zhonguo5118.cn

[H06] 可选值 / 空值安全访问
来源：https://zp.zhonguo6118.cn

Py:   value = d.get("k") or default
来源：https://ix.zhonguo5118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://sa.zhonguo2118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://vc.zhonguo5118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://zm.zhonguo8118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://fv.zhonguo8118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://jp.zhonguo6118.cn

Ruby: d&.dig(:a, :b)
来源：https://es.zhonguo7118.cn

C#:   obj?.A?.B ?? default
来源：https://mv.zhonguo4118.cn

[H07] 断言
来源：https://wf.zhonguo8118.cn

Py:   assert x > 0, "必须为正"
来源：https://ip.zhonguo6118.cn

PHP:  assert($x > 0);
来源：https://cf.zhonguo2118.cn

JS:   console.assert(x > 0);
来源：https://nj.zhonguo8118.cn

TS:   console.assert(x > 0);
来源：https://uo.zhonguo2118.cn

Java: assert x > 0 : "必须为正";
来源：https://al.zhonguo7118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://qu.zhonguo1118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://sy.zhonguo8118.cn

C#:   Debug.Assert(x > 0);
来源：https://uc.zhonguo8118.cn

[H08] 获取错误信息与堆栈
来源：https://lx.zhonguo4118.cn

Py:   str(e);  traceback.format_exc()
来源：https://us.zhonguo2118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://kh.zhonguo7118.cn

JS:   e.message;  e.stack
来源：https://ot.zhonguo1118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://yg.zhonguo8118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://fe.zhonguo8118.cn

Go:   err.Error()
来源：https://sk.zhonguo7118.cn

Ruby: e.message;  e.backtrace
来源：https://dz.zhonguo4118.cn

C#:   e.Message;  e.StackTrace
来源：https://wi.zhonguo3118.cn

[H09] 带错误码的异常
来源：https://ff.zhonguo7118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://ji.zhonguo2118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://uu.zhonguo1118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://ah.zhonguo2118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://cq.zhonguo1118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://yl.zhonguo5118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://be.zhonguo6118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://sz.zhonguo1118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://rb.zhonguo3118.cn

[H10] 资源自动释放
来源：https://ho.zhonguo8118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://wb.zhonguo5118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://yk.zhonguo5118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://ah.zhonguo1118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://xd.zhonguo5118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://ja.zhonguo7118.cn

Go:   defer f.Close()
来源：https://mg.zhonguo4118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://dy.zhonguo4118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://ls.zhonguo7118.cn

================================================================================
来源：https://vc.zhonguo5118.cn

I. 正则表达式
来源：https://be.zhonguo2118.cn

================================================================================
来源：https://va.zhonguo5118.cn

[I01] 判断是否匹配
来源：https://bk.zhonguo6118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://zs.zhonguo7118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://dg.zhonguo2118.cn

JS:   /\d+/.test(s)
来源：https://kt.zhonguo1118.cn

TS:   /\d+/.test(s)
来源：https://fw.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://bx.zhonguo4118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://ql.zhonguo5118.cn

Ruby: s.match?(/\d+/)
来源：https://rr.zhonguo1118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://jp.zhonguo3118.cn

[I02] 提取所有匹配
来源：https://pn.zhonguo6118.cn

Py:   re.findall(r"\d+", s)
来源：https://we.zhonguo5118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://vs.zhonguo6118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://ps.zhonguo7118.cn

TS:   s.match(/\d+/g)
来源：https://np.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://gg.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ra.zhonguo1118.cn

Ruby: s.scan(/\d+/)
来源：https://ky.zhonguo1118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://ye.zhonguo6118.cn

[I03] 提取捕获分组
来源：https://kz.zhonguo8118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://vc.zhonguo7118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://ia.zhonguo6118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://ch.zhonguo6118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://df.zhonguo3118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://pc.zhonguo5118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://kc.zhonguo5118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://vf.zhonguo5118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://zc.zhonguo6118.cn

[I04] 正则替换
来源：https://iu.zhonguo1118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://hz.zhonguo1118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://wo.zhonguo5118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://if.zhonguo6118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://yh.zhonguo7118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://vq.zhonguo6118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://jk.zhonguo2118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://ni.zhonguo2118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://ig.zhonguo1118.cn

[I05] 按正则拆分
来源：https://kp.zhonguo2118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://id.zhonguo8118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://jp.zhonguo5118.cn

JS:   s.split(/\s*,\s*/)
来源：https://bo.zhonguo5118.cn

TS:   s.split(/\s*,\s*/)
来源：https://uo.zhonguo4118.cn

Java: s.split("\\s*,\\s*")
来源：https://kp.zhonguo7118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://js.zhonguo8118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://jx.zhonguo2118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://yl.zhonguo2118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://sv.zhonguo2118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://ag.zhonguo3118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://xb.zhonguo2118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://xo.zhonguo4118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://fb.zhonguo2118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://kj.zhonguo1118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://do.zhonguo1118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://sd.zhonguo8118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://lm.zhonguo1118.cn

[I07] 忽略大小写与多行模式
来源：https://to.zhonguo2118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://pm.zhonguo4118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://ey.zhonguo6118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://ql.zhonguo3118.cn

TS:   /error/gim
来源：https://je.zhonguo7118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://if.zhonguo7118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://uh.zhonguo7118.cn

Ruby: s.scan(/error/i)
来源：https://fr.zhonguo2118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://dv.zhonguo3118.cn

[I08] 贪婪与非贪婪匹配
来源：https://cw.zhonguo2118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://ao.zhonguo1118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://qx.zhonguo3118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://gl.zhonguo1118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://iw.zhonguo3118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://ka.zhonguo6118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://fo.zhonguo6118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://xm.zhonguo4118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://uc.zhonguo1118.cn

================================================================================
来源：https://qx.zhonguo6118.cn

J. 日期与时间
来源：https://bf.zhonguo1118.cn

================================================================================
来源：https://tr.zhonguo2118.cn

[J01] 获取当前时间
来源：https://er.zhonguo1118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://oh.zhonguo8118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://ib.zhonguo2118.cn

JS:   new Date();  Date.now()
来源：https://rc.zhonguo5118.cn

TS:   new Date();  Date.now()
来源：https://dw.zhonguo7118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://lj.zhonguo3118.cn

Go:   time.Now()
来源：https://gr.zhonguo7118.cn

Ruby: Time.now
来源：https://wu.zhonguo1118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://cl.zhonguo2118.cn

[J02] 格式化输出
来源：https://qh.zhonguo7118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://bj.zhonguo5118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://tk.zhonguo3118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://et.zhonguo6118.cn

TS:   d.toISOString()
来源：https://yo.zhonguo6118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://dj.zhonguo7118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://nx.zhonguo4118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://yx.zhonguo7118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://xe.zhonguo4118.cn

[J03] 字符串解析为日期
来源：https://vw.zhonguo8118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://xe.zhonguo1118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://md.zhonguo7118.cn

JS:   new Date("2024-01-02")
来源：https://ja.zhonguo3118.cn

TS:   new Date("2024-01-02")
来源：https://fm.zhonguo5118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://zc.zhonguo7118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://br.zhonguo2118.cn

Ruby: Date.parse("2024-01-02")
来源：https://df.zhonguo5118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://cr.zhonguo3118.cn

[J04] 时间戳与日期互转
来源：https://kk.zhonguo5118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://uq.zhonguo7118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://nx.zhonguo3118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://bd.zhonguo8118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://gd.zhonguo7118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://zy.zhonguo4118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://pa.zhonguo3118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://bm.zhonguo8118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://nc.zhonguo8118.cn

[J05] 时间加减（加 7 天）
来源：https://kj.zhonguo6118.cn

Py:   now + timedelta(days=7)
来源：https://yw.zhonguo3118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://ed.zhonguo5118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://ad.zhonguo4118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://lm.zhonguo7118.cn

Java: LocalDate.now().plusDays(7)
来源：https://sa.zhonguo2118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://an.zhonguo1118.cn

Ruby: Time.now + 7 * 86400
来源：https://ib.zhonguo1118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://rp.zhonguo4118.cn

[J06] 计算两时间之差
来源：https://dy.zhonguo6118.cn

Py:   (end - start).total_seconds()
来源：https://yz.zhonguo5118.cn

PHP:  $end->diff($start)->days;
来源：https://xb.zhonguo3118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://lm.zhonguo8118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://ns.zhonguo6118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://ie.zhonguo3118.cn

Go:   end.Sub(start).Hours()
来源：https://gj.zhonguo8118.cn

Ruby: end - start                 # 返回秒数
来源：https://zk.zhonguo2118.cn

C#:   (end - start).TotalSeconds
来源：https://yj.zhonguo6118.cn

[J07] 比较两个日期
来源：https://nw.zhonguo6118.cn

Py:   d1 < d2;  d1 == d2
来源：https://yn.zhonguo1118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://kl.zhonguo2118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://kp.zhonguo3118.cn


<!-- 参考信息 -->