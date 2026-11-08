代发 wailian999

JS:   get name() { return this._name; }
来源：https://hs.zhonguo8118.cn

TS:   get name(): string { return this._name; }
来源：https://zt.zhonguo5118.cn

Java: public String getName() { return name; }
来源：https://tn.zhonguo3118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://hn.zhonguo2118.cn

Ruby: attr_accessor :name
来源：https://fy.zhonguo6118.cn

C#:   public string Name { get; set; }
来源：https://wp.zhonguo2118.cn

[G12] 对象转字符串
来源：https://nd.zhonguo2118.cn

Py:   def __str__(self): return self.name
来源：https://ca.zhonguo1118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://vn.zhonguo5118.cn

JS:   toString() { return this.name; }
来源：https://jo.zhonguo7118.cn

TS:   toString(): string { return this.name; }
来源：https://bj.zhonguo5118.cn

Java: @Override public String toString() { return name; }
来源：https://ya.zhonguo2118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://cl.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://kl.zhonguo3118.cn

C#:   public override string ToString() => Name;
来源：https://er.zhonguo1118.cn

[G13] 判断对象类型
来源：https://bv.zhonguo8118.cn

Py:   isinstance(u, User)
来源：https://lx.zhonguo6118.cn

PHP:  $u instanceof User
来源：https://pb.zhonguo1118.cn

JS:   u instanceof User
来源：https://ia.zhonguo1118.cn

TS:   u instanceof User
来源：https://vz.zhonguo7118.cn

Java: u instanceof User
来源：https://pm.zhonguo5118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://bu.zhonguo7118.cn

Ruby: u.is_a?(User)
来源：https://lp.zhonguo6118.cn

C#:   u is User
来源：https://mm.zhonguo1118.cn

[G14] 数据类 / record
来源：https://te.zhonguo1118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://ag.zhonguo7118.cn

PHP:  // 用 readonly 属性模拟
来源：https://vr.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://qv.zhonguo8118.cn

TS:   type User = { name: string; age: number };
来源：https://gp.zhonguo1118.cn

Java: record User(String name, int age) {}
来源：https://ed.zhonguo4118.cn

Go:   type User struct { Name string; Age int }
来源：https://ii.zhonguo1118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://sk.zhonguo4118.cn

C#:   record User(string Name, int Age);
来源：https://sj.zhonguo1118.cn

[G15] 枚举
来源：https://tw.zhonguo2118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://ks.zhonguo6118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://po.zhonguo5118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://ag.zhonguo1118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://jq.zhonguo4118.cn

Java: enum Color { RED, GREEN }
来源：https://hm.zhonguo8118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://wt.zhonguo8118.cn

Ruby: Color = %i[red green].freeze
来源：https://qx.zhonguo5118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://du.zhonguo8118.cn

[G16] 对象转数组 / 字典
来源：https://sx.zhonguo8118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://tc.zhonguo4118.cn

PHP:  get_object_vars($obj);
来源：https://kp.zhonguo2118.cn

JS:   Object.entries(obj)
来源：https://qy.zhonguo8118.cn

TS:   Object.entries(obj)
来源：https://pr.zhonguo8118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://nn.zhonguo5118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://ab.zhonguo5118.cn

Ruby: obj.instance_variables
来源：https://op.zhonguo1118.cn

C#:   // 用反射或 System.Text.Json
来源：https://ku.zhonguo8118.cn

================================================================================
来源：https://do.zhonguo6118.cn

H. 异常与错误处理
来源：https://uj.zhonguo8118.cn

================================================================================
来源：https://lb.zhonguo7118.cn

[H01] try / catch 基础
来源：https://og.zhonguo8118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://au.zhonguo6118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://ct.zhonguo1118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://rk.zhonguo8118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://sr.zhonguo7118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://fo.zhonguo3118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://ok.zhonguo6118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://ll.zhonguo6118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://rg.zhonguo4118.cn

[H02] finally / ensure 收尾
来源：https://sv.zhonguo7118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://ta.zhonguo6118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://xj.zhonguo1118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://np.zhonguo2118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://so.zhonguo7118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://vn.zhonguo1118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://jm.zhonguo5118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://an.zhonguo5118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://mq.zhonguo3118.cn

[H03] 主动抛出异常
来源：https://xm.zhonguo2118.cn

Py:   raise ValueError("错误信息")
来源：https://mj.zhonguo8118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://wg.zhonguo8118.cn

JS:   throw new Error("错误信息");
来源：https://ni.zhonguo5118.cn

TS:   throw new Error("错误信息");
来源：https://sf.zhonguo6118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://nf.zhonguo6118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://wx.zhonguo6118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://in.zhonguo1118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://mb.zhonguo5118.cn

[H04] 自定义异常类型
来源：https://zb.zhonguo6118.cn

Py:   class MyError(Exception): pass
来源：https://pr.zhonguo6118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://vz.zhonguo5118.cn

JS:   class MyError extends Error {}
来源：https://ru.zhonguo7118.cn

TS:   class MyError extends Error {}
来源：https://dl.zhonguo8118.cn

Java: class MyException extends RuntimeException {}
来源：https://bb.zhonguo6118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://sa.zhonguo1118.cn

Ruby: class MyError < StandardError; end
来源：https://yl.zhonguo8118.cn

C#:   class MyException : Exception {}
来源：https://vc.zhonguo6118.cn

[H05] 捕获特定类型
来源：https://qq.zhonguo4118.cn

Py:   except ValueError as e:
来源：https://td.zhonguo2118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://sm.zhonguo4118.cn

JS:   if (e instanceof TypeError) {}
来源：https://kp.zhonguo2118.cn

TS:   if (e instanceof TypeError) {}
来源：https://rx.zhonguo6118.cn

Java: catch (IOException | SQLException e) {}
来源：https://sy.zhonguo3118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://vv.zhonguo6118.cn

Ruby: rescue ArgumentError => e
来源：https://ky.zhonguo1118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://zo.zhonguo2118.cn

[H06] 可选值 / 空值安全访问
来源：https://ca.zhonguo3118.cn

Py:   value = d.get("k") or default
来源：https://xf.zhonguo2118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://zs.zhonguo3118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://ln.zhonguo3118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://pv.zhonguo3118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://mz.zhonguo7118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://ak.zhonguo6118.cn

Ruby: d&.dig(:a, :b)
来源：https://nu.zhonguo3118.cn

C#:   obj?.A?.B ?? default
来源：https://dl.zhonguo3118.cn

[H07] 断言
来源：https://wv.zhonguo5118.cn

Py:   assert x > 0, "必须为正"
来源：https://bu.zhonguo7118.cn

PHP:  assert($x > 0);
来源：https://dz.zhonguo7118.cn

JS:   console.assert(x > 0);
来源：https://ip.zhonguo3118.cn

TS:   console.assert(x > 0);
来源：https://of.zhonguo8118.cn

Java: assert x > 0 : "必须为正";
来源：https://tv.zhonguo1118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://te.zhonguo1118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://nw.zhonguo5118.cn

C#:   Debug.Assert(x > 0);
来源：https://ka.zhonguo6118.cn

[H08] 获取错误信息与堆栈
来源：https://zf.zhonguo2118.cn

Py:   str(e);  traceback.format_exc()
来源：https://iu.zhonguo5118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://mg.zhonguo8118.cn

JS:   e.message;  e.stack
来源：https://oj.zhonguo5118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://yd.zhonguo6118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://wm.zhonguo4118.cn

Go:   err.Error()
来源：https://mr.zhonguo5118.cn

Ruby: e.message;  e.backtrace
来源：https://bc.zhonguo3118.cn

C#:   e.Message;  e.StackTrace
来源：https://bb.zhonguo3118.cn

[H09] 带错误码的异常
来源：https://dm.zhonguo4118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://oo.zhonguo2118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://iw.zhonguo1118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://rz.zhonguo1118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://ba.zhonguo7118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://ql.zhonguo3118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://mk.zhonguo8118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://lw.zhonguo6118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://md.zhonguo2118.cn

[H10] 资源自动释放
来源：https://ov.zhonguo8118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://wx.zhonguo6118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://go.zhonguo4118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://bj.zhonguo7118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://nv.zhonguo5118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://mp.zhonguo4118.cn

Go:   defer f.Close()
来源：https://rf.zhonguo1118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://xn.zhonguo3118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://qd.zhonguo4118.cn

================================================================================
来源：https://vs.zhonguo1118.cn

I. 正则表达式
来源：https://gu.zhonguo4118.cn

================================================================================
来源：https://jk.zhonguo2118.cn

[I01] 判断是否匹配
来源：https://zs.zhonguo1118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://fp.zhonguo8118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://xt.zhonguo5118.cn

JS:   /\d+/.test(s)
来源：https://iu.zhonguo2118.cn

TS:   /\d+/.test(s)
来源：https://dr.zhonguo5118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://uk.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://eg.zhonguo4118.cn

Ruby: s.match?(/\d+/)
来源：https://wg.zhonguo5118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://tc.zhonguo3118.cn

[I02] 提取所有匹配
来源：https://oc.zhonguo7118.cn

Py:   re.findall(r"\d+", s)
来源：https://zf.zhonguo1118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://uw.zhonguo2118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://vr.zhonguo6118.cn

TS:   s.match(/\d+/g)
来源：https://dc.zhonguo2118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://wu.zhonguo2118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://tt.zhonguo3118.cn

Ruby: s.scan(/\d+/)
来源：https://xb.zhonguo6118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://su.zhonguo1118.cn

[I03] 提取捕获分组
来源：https://jc.zhonguo6118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://wh.zhonguo8118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://ym.zhonguo2118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://zy.zhonguo1118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://tk.zhonguo2118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://zf.zhonguo7118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://ma.zhonguo7118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://ed.zhonguo7118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://dc.zhonguo5118.cn

[I04] 正则替换
来源：https://cu.zhonguo1118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://fi.zhonguo5118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://rx.zhonguo7118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://co.zhonguo8118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://mv.zhonguo3118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://ay.zhonguo1118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://kk.zhonguo3118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://ti.zhonguo4118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://ug.zhonguo8118.cn

[I05] 按正则拆分
来源：https://xb.zhonguo1118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://fs.zhonguo4118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://go.zhonguo5118.cn

JS:   s.split(/\s*,\s*/)
来源：https://gn.zhonguo8118.cn

TS:   s.split(/\s*,\s*/)
来源：https://da.zhonguo2118.cn

Java: s.split("\\s*,\\s*")
来源：https://yu.zhonguo4118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://is.zhonguo7118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://ks.zhonguo3118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://zq.zhonguo7118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://kp.zhonguo2118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://sb.zhonguo6118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://dr.zhonguo3118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://vv.zhonguo5118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://yb.zhonguo6118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://xc.zhonguo4118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://bd.zhonguo6118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://al.zhonguo8118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://xq.zhonguo4118.cn

[I07] 忽略大小写与多行模式
来源：https://vl.zhonguo5118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://un.zhonguo2118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://br.zhonguo5118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://hk.zhonguo3118.cn

TS:   /error/gim
来源：https://ns.zhonguo8118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://js.zhonguo3118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://cz.zhonguo8118.cn

Ruby: s.scan(/error/i)
来源：https://ec.zhonguo8118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://re.zhonguo8118.cn

[I08] 贪婪与非贪婪匹配
来源：https://lc.zhonguo4118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://yw.zhonguo7118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://qb.zhonguo5118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://dh.zhonguo4118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://zu.zhonguo4118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://eg.zhonguo2118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://ud.zhonguo6118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://zy.zhonguo6118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://an.zhonguo6118.cn

================================================================================
来源：https://gx.zhonguo2118.cn

J. 日期与时间
来源：https://yi.zhonguo5118.cn

================================================================================
来源：https://rm.zhonguo2118.cn

[J01] 获取当前时间
来源：https://qy.zhonguo3118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://tb.zhonguo8118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://mj.zhonguo8118.cn

JS:   new Date();  Date.now()
来源：https://fy.zhonguo3118.cn

TS:   new Date();  Date.now()
来源：https://yd.zhonguo8118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://io.zhonguo1118.cn

Go:   time.Now()
来源：https://up.zhonguo6118.cn

Ruby: Time.now
来源：https://ta.zhonguo2118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://og.zhonguo7118.cn

[J02] 格式化输出
来源：https://oq.zhonguo7118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://ov.zhonguo8118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://qk.zhonguo4118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://mp.zhonguo2118.cn

TS:   d.toISOString()
来源：https://jj.zhonguo5118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://zf.zhonguo3118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://uo.zhonguo7118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://ve.zhonguo8118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://ay.zhonguo3118.cn

[J03] 字符串解析为日期
来源：https://vl.zhonguo4118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://wo.zhonguo6118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://ve.zhonguo8118.cn

JS:   new Date("2024-01-02")
来源：https://sg.zhonguo8118.cn

TS:   new Date("2024-01-02")
来源：https://tb.zhonguo1118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://dh.zhonguo7118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://ad.zhonguo5118.cn

Ruby: Date.parse("2024-01-02")
来源：https://ry.zhonguo3118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://jw.zhonguo2118.cn

[J04] 时间戳与日期互转
来源：https://au.zhonguo1118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://xq.zhonguo8118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://xb.zhonguo1118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://cn.zhonguo5118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://tm.zhonguo4118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://xh.zhonguo3118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://qz.zhonguo1118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://ng.zhonguo4118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://vw.zhonguo7118.cn

[J05] 时间加减（加 7 天）
来源：https://ec.zhonguo3118.cn

Py:   now + timedelta(days=7)
来源：https://kl.zhonguo8118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://vg.zhonguo6118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://ja.zhonguo7118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://tm.zhonguo5118.cn

Java: LocalDate.now().plusDays(7)
来源：https://dm.zhonguo8118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://yf.zhonguo8118.cn

Ruby: Time.now + 7 * 86400
来源：https://ow.zhonguo7118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://nn.zhonguo8118.cn

[J06] 计算两时间之差
来源：https://do.zhonguo7118.cn

Py:   (end - start).total_seconds()
来源：https://rp.zhonguo8118.cn

PHP:  $end->diff($start)->days;
来源：https://vm.zhonguo3118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://ut.zhonguo2118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://cy.zhonguo6118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://ho.zhonguo2118.cn

Go:   end.Sub(start).Hours()
来源：https://ad.zhonguo3118.cn

Ruby: end - start                 # 返回秒数
来源：https://my.zhonguo5118.cn

C#:   (end - start).TotalSeconds
来源：https://ek.zhonguo2118.cn

[J07] 比较两个日期
来源：https://ye.zhonguo8118.cn

Py:   d1 < d2;  d1 == d2
来源：https://gv.zhonguo4118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://hl.zhonguo8118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://to.zhonguo4118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://cz.zhonguo7118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://ld.zhonguo3118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://hd.zhonguo7118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://ks.zhonguo5118.cn

C#:   d1 < d2;  d1 == d2
来源：https://hu.zhonguo6118.cn

[J08] 提取年月日与星期
来源：https://fc.zhonguo5118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://rf.zhonguo1118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://xt.zhonguo6118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://zy.zhonguo7118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://xx.zhonguo8118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://hr.zhonguo6118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://eh.zhonguo3118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://ep.zhonguo8118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://qd.zhonguo6118.cn

[J09] 时区处理
来源：https://rx.zhonguo4118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://mu.zhonguo7118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://gi.zhonguo2118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://eg.zhonguo8118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://tz.zhonguo5118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://ti.zhonguo2118.cn


<!-- 参考信息 -->