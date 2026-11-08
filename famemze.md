代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：https://zv.zhonguo7118.cn

Ruby: def self.f; end
来源：https://ad.zhonguo8118.cn

C#:   public static void F() {}
来源：https://et.zhonguo8118.cn

[G09] 接口 / 抽象类
来源：https://sr.zhonguo2118.cn

Py:   from abc import ABC, abstractmethod
来源：https://bs.zhonguo3118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://el.zhonguo3118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://rf.zhonguo5118.cn

TS:   interface Shape { area(): number; }
来源：https://je.zhonguo2118.cn

Java: interface Shape { double area(); }
来源：https://id.zhonguo8118.cn

Go:   type Shape interface { Area() float64 }
来源：https://rz.zhonguo7118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://vg.zhonguo8118.cn

C#:   interface IShape { double Area(); }
来源：https://sz.zhonguo2118.cn

[G10] 访问控制
来源：https://qr.zhonguo6118.cn

Py:   约定 _protected / __private（不强制）
来源：https://ks.zhonguo1118.cn

PHP:  public / protected / private
来源：https://dp.zhonguo8118.cn

JS:   #private 字段；其余公开
来源：https://dt.zhonguo3118.cn

TS:   public / protected / private
来源：https://cp.zhonguo2118.cn

Java: public / protected / private / 默认包级
来源：https://fn.zhonguo3118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://up.zhonguo6118.cn

Ruby: public / protected / private
来源：https://fu.zhonguo8118.cn

C#:   public / protected / private / internal
来源：https://bp.zhonguo4118.cn

[G11] getter / setter
来源：https://jp.zhonguo6118.cn

Py:   @property 与 @x.setter
来源：https://op.zhonguo4118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://wn.zhonguo3118.cn

JS:   get name() { return this._name; }
来源：https://qj.zhonguo1118.cn

TS:   get name(): string { return this._name; }
来源：https://hz.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://or.zhonguo1118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://fy.zhonguo4118.cn

Ruby: attr_accessor :name
来源：https://py.zhonguo7118.cn

C#:   public string Name { get; set; }
来源：https://pu.zhonguo2118.cn

[G12] 对象转字符串
来源：https://ox.zhonguo1118.cn

Py:   def __str__(self): return self.name
来源：https://zr.zhonguo2118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ru.zhonguo5118.cn

JS:   toString() { return this.name; }
来源：https://nn.zhonguo2118.cn

TS:   toString(): string { return this.name; }
来源：https://qk.zhonguo7118.cn

Java: @Override public String toString() { return name; }
来源：https://qn.zhonguo8118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://mg.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://cg.zhonguo3118.cn

C#:   public override string ToString() => Name;
来源：https://lo.zhonguo2118.cn

[G13] 判断对象类型
来源：https://hf.zhonguo6118.cn

Py:   isinstance(u, User)
来源：https://bg.zhonguo5118.cn

PHP:  $u instanceof User
来源：https://sz.zhonguo5118.cn

JS:   u instanceof User
来源：https://af.zhonguo1118.cn

TS:   u instanceof User
来源：https://yq.zhonguo5118.cn

Java: u instanceof User
来源：https://go.zhonguo3118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ip.zhonguo2118.cn

Ruby: u.is_a?(User)
来源：https://pr.zhonguo7118.cn

C#:   u is User
来源：https://ay.zhonguo2118.cn

[G14] 数据类 / record
来源：https://th.zhonguo8118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://lh.zhonguo8118.cn

PHP:  // 用 readonly 属性模拟
来源：https://mu.zhonguo6118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://au.zhonguo3118.cn

TS:   type User = { name: string; age: number };
来源：https://re.zhonguo2118.cn

Java: record User(String name, int age) {}
来源：https://yo.zhonguo4118.cn

Go:   type User struct { Name string; Age int }
来源：https://ua.zhonguo1118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://cw.zhonguo8118.cn

C#:   record User(string Name, int Age);
来源：https://ru.zhonguo6118.cn

[G15] 枚举
来源：https://tm.zhonguo6118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://ln.zhonguo6118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://nb.zhonguo5118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://mf.zhonguo2118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://oz.zhonguo3118.cn

Java: enum Color { RED, GREEN }
来源：https://uj.zhonguo7118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://bh.zhonguo5118.cn

Ruby: Color = %i[red green].freeze
来源：https://ul.zhonguo4118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://rg.zhonguo2118.cn

[G16] 对象转数组 / 字典
来源：https://tw.zhonguo1118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://au.zhonguo4118.cn

PHP:  get_object_vars($obj);
来源：https://ne.zhonguo5118.cn

JS:   Object.entries(obj)
来源：https://gd.zhonguo7118.cn

TS:   Object.entries(obj)
来源：https://pk.zhonguo1118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://sk.zhonguo2118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://hj.zhonguo5118.cn

Ruby: obj.instance_variables
来源：https://mz.zhonguo1118.cn

C#:   // 用反射或 System.Text.Json
来源：https://nt.zhonguo5118.cn

================================================================================
来源：https://qf.zhonguo3118.cn

H. 异常与错误处理
来源：https://tg.zhonguo8118.cn

================================================================================
来源：https://bu.zhonguo8118.cn

[H01] try / catch 基础
来源：https://ub.zhonguo2118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://ft.zhonguo7118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://nm.zhonguo3118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://px.zhonguo7118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://sm.zhonguo8118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://lz.zhonguo5118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://ls.zhonguo3118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://oa.zhonguo4118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://og.zhonguo3118.cn

[H02] finally / ensure 收尾
来源：https://wb.zhonguo1118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://fd.zhonguo7118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://io.zhonguo7118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://oy.zhonguo1118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://ro.zhonguo6118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://ik.zhonguo8118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://st.zhonguo7118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://zt.zhonguo8118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://zd.zhonguo6118.cn

[H03] 主动抛出异常
来源：https://ie.zhonguo7118.cn

Py:   raise ValueError("错误信息")
来源：https://mg.zhonguo3118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://pw.zhonguo7118.cn

JS:   throw new Error("错误信息");
来源：https://na.zhonguo2118.cn

TS:   throw new Error("错误信息");
来源：https://ra.zhonguo8118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://zb.zhonguo7118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://vs.zhonguo1118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ba.zhonguo6118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://vi.zhonguo3118.cn

[H04] 自定义异常类型
来源：https://mu.zhonguo1118.cn

Py:   class MyError(Exception): pass
来源：https://xp.zhonguo8118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://ia.zhonguo8118.cn

JS:   class MyError extends Error {}
来源：https://hm.zhonguo2118.cn

TS:   class MyError extends Error {}
来源：https://ea.zhonguo2118.cn

Java: class MyException extends RuntimeException {}
来源：https://iq.zhonguo6118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://un.zhonguo7118.cn

Ruby: class MyError < StandardError; end
来源：https://qe.zhonguo2118.cn

C#:   class MyException : Exception {}
来源：https://fy.zhonguo7118.cn

[H05] 捕获特定类型
来源：https://no.zhonguo8118.cn

Py:   except ValueError as e:
来源：https://zh.zhonguo3118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://qs.zhonguo3118.cn

JS:   if (e instanceof TypeError) {}
来源：https://xn.zhonguo2118.cn

TS:   if (e instanceof TypeError) {}
来源：https://hn.zhonguo6118.cn

Java: catch (IOException | SQLException e) {}
来源：https://gi.zhonguo6118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://gu.zhonguo3118.cn

Ruby: rescue ArgumentError => e
来源：https://yz.zhonguo6118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://ts.zhonguo1118.cn

[H06] 可选值 / 空值安全访问
来源：https://bo.zhonguo7118.cn

Py:   value = d.get("k") or default
来源：https://ud.zhonguo2118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://gg.zhonguo2118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://tx.zhonguo2118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://se.zhonguo8118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://au.zhonguo5118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://cj.zhonguo1118.cn

Ruby: d&.dig(:a, :b)
来源：https://nn.zhonguo4118.cn

C#:   obj?.A?.B ?? default
来源：https://da.zhonguo2118.cn

[H07] 断言
来源：https://zu.zhonguo8118.cn

Py:   assert x > 0, "必须为正"
来源：https://ok.zhonguo2118.cn

PHP:  assert($x > 0);
来源：https://bh.zhonguo7118.cn

JS:   console.assert(x > 0);
来源：https://bz.zhonguo1118.cn

TS:   console.assert(x > 0);
来源：https://rb.zhonguo1118.cn

Java: assert x > 0 : "必须为正";
来源：https://xr.zhonguo8118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://lf.zhonguo3118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://cg.zhonguo5118.cn

C#:   Debug.Assert(x > 0);
来源：https://ly.zhonguo7118.cn

[H08] 获取错误信息与堆栈
来源：https://zu.zhonguo4118.cn

Py:   str(e);  traceback.format_exc()
来源：https://jm.zhonguo2118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://pq.zhonguo5118.cn

JS:   e.message;  e.stack
来源：https://ju.zhonguo1118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://fj.zhonguo5118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://uk.zhonguo7118.cn

Go:   err.Error()
来源：https://oh.zhonguo8118.cn

Ruby: e.message;  e.backtrace
来源：https://fp.zhonguo4118.cn

C#:   e.Message;  e.StackTrace
来源：https://hk.zhonguo5118.cn

[H09] 带错误码的异常
来源：https://ma.zhonguo3118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://rg.zhonguo8118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://zd.zhonguo3118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://fv.zhonguo7118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://vp.zhonguo4118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://km.zhonguo4118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://mp.zhonguo8118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://qi.zhonguo6118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://pa.zhonguo1118.cn

[H10] 资源自动释放
来源：https://ip.zhonguo3118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://tq.zhonguo2118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://ro.zhonguo2118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://yd.zhonguo6118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://kc.zhonguo2118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://yu.zhonguo1118.cn

Go:   defer f.Close()
来源：https://wt.zhonguo7118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://gg.zhonguo6118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://uc.zhonguo2118.cn

================================================================================
来源：https://wk.zhonguo1118.cn

I. 正则表达式
来源：https://rq.zhonguo4118.cn

================================================================================
来源：https://lg.zhonguo7118.cn

[I01] 判断是否匹配
来源：https://um.zhonguo5118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://ks.zhonguo7118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://gv.zhonguo6118.cn

JS:   /\d+/.test(s)
来源：https://dm.zhonguo8118.cn

TS:   /\d+/.test(s)
来源：https://ot.zhonguo2118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://zy.zhonguo7118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://xf.zhonguo6118.cn

Ruby: s.match?(/\d+/)
来源：https://qg.zhonguo7118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://xb.zhonguo3118.cn

[I02] 提取所有匹配
来源：https://zm.zhonguo8118.cn

Py:   re.findall(r"\d+", s)
来源：https://lz.zhonguo5118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://op.zhonguo4118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://jb.zhonguo1118.cn

TS:   s.match(/\d+/g)
来源：https://wd.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://fg.zhonguo1118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://wl.zhonguo7118.cn

Ruby: s.scan(/\d+/)
来源：https://ia.zhonguo2118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://gk.zhonguo5118.cn

[I03] 提取捕获分组
来源：https://tc.zhonguo8118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://st.zhonguo8118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://vw.zhonguo5118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://gz.zhonguo1118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://bj.zhonguo8118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://hr.zhonguo5118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://vk.zhonguo8118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://dw.zhonguo1118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://sp.zhonguo3118.cn

[I04] 正则替换
来源：https://wj.zhonguo8118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://oi.zhonguo5118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://yw.zhonguo5118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://jb.zhonguo2118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://ts.zhonguo4118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://qv.zhonguo5118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://fg.zhonguo3118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://qj.zhonguo6118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://ik.zhonguo8118.cn

[I05] 按正则拆分
来源：https://qe.zhonguo4118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://op.zhonguo6118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://tp.zhonguo7118.cn

JS:   s.split(/\s*,\s*/)
来源：https://dq.zhonguo8118.cn

TS:   s.split(/\s*,\s*/)
来源：https://rn.zhonguo1118.cn

Java: s.split("\\s*,\\s*")
来源：https://tv.zhonguo8118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://jq.zhonguo1118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://ad.zhonguo8118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://na.zhonguo7118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://by.zhonguo8118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://hx.zhonguo4118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://ip.zhonguo7118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://xx.zhonguo1118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://qv.zhonguo2118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://vi.zhonguo3118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://hn.zhonguo7118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://oq.zhonguo7118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://sq.zhonguo8118.cn

[I07] 忽略大小写与多行模式
来源：https://tj.zhonguo7118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://uy.zhonguo8118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://uz.zhonguo2118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://tf.zhonguo6118.cn

TS:   /error/gim
来源：https://ze.zhonguo2118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://pe.zhonguo4118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://fq.zhonguo6118.cn

Ruby: s.scan(/error/i)
来源：https://kg.zhonguo8118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://be.zhonguo3118.cn

[I08] 贪婪与非贪婪匹配
来源：https://yu.zhonguo3118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://qu.zhonguo4118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://lf.zhonguo2118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://it.zhonguo1118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://jw.zhonguo4118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://pg.zhonguo5118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://gt.zhonguo7118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://gh.zhonguo5118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://cc.zhonguo1118.cn

================================================================================
来源：https://fj.zhonguo1118.cn

J. 日期与时间
来源：https://nv.zhonguo1118.cn

================================================================================
来源：https://xd.zhonguo4118.cn

[J01] 获取当前时间
来源：https://vr.zhonguo6118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://wk.zhonguo8118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://yz.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://ij.zhonguo7118.cn

TS:   new Date();  Date.now()
来源：https://pc.zhonguo2118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://ey.zhonguo4118.cn

Go:   time.Now()
来源：https://jk.zhonguo5118.cn

Ruby: Time.now
来源：https://hv.zhonguo6118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://xk.zhonguo2118.cn

[J02] 格式化输出
来源：https://ze.zhonguo1118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://oh.zhonguo5118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://mz.zhonguo1118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://vx.zhonguo4118.cn

TS:   d.toISOString()
来源：https://ba.zhonguo5118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://gg.zhonguo3118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://az.zhonguo5118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://fk.zhonguo2118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://ss.zhonguo2118.cn

[J03] 字符串解析为日期
来源：https://hg.zhonguo7118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://xg.zhonguo1118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://gt.zhonguo5118.cn

JS:   new Date("2024-01-02")
来源：https://hv.zhonguo1118.cn

TS:   new Date("2024-01-02")
来源：https://st.zhonguo2118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://xt.zhonguo7118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://qh.zhonguo4118.cn

Ruby: Date.parse("2024-01-02")
来源：https://yj.zhonguo1118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://uo.zhonguo2118.cn

[J04] 时间戳与日期互转
来源：https://oh.zhonguo3118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://rc.zhonguo6118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://my.zhonguo3118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://qy.zhonguo6118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://fc.zhonguo8118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://gg.zhonguo1118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://xg.zhonguo1118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://uq.zhonguo6118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://yf.zhonguo8118.cn

[J05] 时间加减（加 7 天）
来源：https://ox.zhonguo1118.cn

Py:   now + timedelta(days=7)
来源：https://nk.zhonguo5118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://hu.zhonguo6118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://oz.zhonguo1118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://dn.zhonguo3118.cn

Java: LocalDate.now().plusDays(7)
来源：https://km.zhonguo8118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://od.zhonguo1118.cn

Ruby: Time.now + 7 * 86400
来源：https://tc.zhonguo7118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://wr.zhonguo1118.cn

[J06] 计算两时间之差
来源：https://nd.zhonguo7118.cn

Py:   (end - start).total_seconds()
来源：https://bm.zhonguo4118.cn

PHP:  $end->diff($start)->days;
来源：https://wu.zhonguo4118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://ic.zhonguo1118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://oz.zhonguo6118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://ih.zhonguo7118.cn

Go:   end.Sub(start).Hours()
来源：https://jl.zhonguo6118.cn

Ruby: end - start                 # 返回秒数
来源：https://tt.zhonguo2118.cn

C#:   (end - start).TotalSeconds
来源：https://ki.zhonguo7118.cn


<!-- 参考信息 -->