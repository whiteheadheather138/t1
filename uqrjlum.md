代发 wailian999

JS:   get name() { return this._name; }
来源：https://wi.zhonguo8118.cn

TS:   get name(): string { return this._name; }
来源：https://ns.zhonguo6118.cn

Java: public String getName() { return name; }
来源：https://ts.zhonguo7118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://sh.zhonguo7118.cn

Ruby: attr_accessor :name
来源：https://jd.zhonguo6118.cn

C#:   public string Name { get; set; }
来源：https://wj.zhonguo3118.cn

[G12] 对象转字符串
来源：https://up.zhonguo1118.cn

Py:   def __str__(self): return self.name
来源：https://lh.zhonguo5118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://cf.zhonguo2118.cn

JS:   toString() { return this.name; }
来源：https://ws.zhonguo5118.cn

TS:   toString(): string { return this.name; }
来源：https://vg.zhonguo6118.cn

Java: @Override public String toString() { return name; }
来源：https://rc.zhonguo1118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://pg.zhonguo1118.cn

Ruby: def to_s; @name; end
来源：https://fz.zhonguo6118.cn

C#:   public override string ToString() => Name;
来源：https://ay.zhonguo3118.cn

[G13] 判断对象类型
来源：https://uh.zhonguo6118.cn

Py:   isinstance(u, User)
来源：https://pj.zhonguo6118.cn

PHP:  $u instanceof User
来源：https://fc.zhonguo3118.cn

JS:   u instanceof User
来源：https://fa.zhonguo3118.cn

TS:   u instanceof User
来源：https://zq.zhonguo5118.cn

Java: u instanceof User
来源：https://wb.zhonguo1118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://gj.zhonguo7118.cn

Ruby: u.is_a?(User)
来源：https://an.zhonguo1118.cn

C#:   u is User
来源：https://hk.zhonguo5118.cn

[G14] 数据类 / record
来源：https://za.zhonguo3118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://mi.zhonguo2118.cn

PHP:  // 用 readonly 属性模拟
来源：https://vs.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://lt.zhonguo8118.cn

TS:   type User = { name: string; age: number };
来源：https://bz.zhonguo5118.cn

Java: record User(String name, int age) {}
来源：https://lu.zhonguo8118.cn

Go:   type User struct { Name string; Age int }
来源：https://xc.zhonguo3118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://oy.zhonguo5118.cn

C#:   record User(string Name, int Age);
来源：https://ts.zhonguo7118.cn

[G15] 枚举
来源：https://ud.zhonguo7118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://vq.zhonguo7118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://ma.zhonguo1118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://bc.zhonguo4118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://ca.zhonguo5118.cn

Java: enum Color { RED, GREEN }
来源：https://ck.zhonguo8118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://yi.zhonguo5118.cn

Ruby: Color = %i[red green].freeze
来源：https://lv.zhonguo5118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://wf.zhonguo4118.cn

[G16] 对象转数组 / 字典
来源：https://oh.zhonguo5118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://xx.zhonguo3118.cn

PHP:  get_object_vars($obj);
来源：https://tf.zhonguo4118.cn

JS:   Object.entries(obj)
来源：https://xm.zhonguo2118.cn

TS:   Object.entries(obj)
来源：https://ip.zhonguo6118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://iw.zhonguo4118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://wb.zhonguo3118.cn

Ruby: obj.instance_variables
来源：https://db.zhonguo7118.cn

C#:   // 用反射或 System.Text.Json
来源：https://rk.zhonguo3118.cn

================================================================================
来源：https://dh.zhonguo4118.cn

H. 异常与错误处理
来源：https://wz.zhonguo4118.cn

================================================================================
来源：https://kp.zhonguo5118.cn

[H01] try / catch 基础
来源：https://cv.zhonguo1118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://kx.zhonguo3118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://ts.zhonguo2118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://ng.zhonguo4118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://yq.zhonguo5118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://ny.zhonguo1118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://xt.zhonguo4118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://nv.zhonguo4118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://ks.zhonguo5118.cn

[H02] finally / ensure 收尾
来源：https://gg.zhonguo4118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://bo.zhonguo1118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://hl.zhonguo3118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://ox.zhonguo1118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://me.zhonguo8118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://ch.zhonguo2118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://ny.zhonguo6118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://vr.zhonguo6118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://lg.zhonguo8118.cn

[H03] 主动抛出异常
来源：https://aq.zhonguo5118.cn

Py:   raise ValueError("错误信息")
来源：https://nb.zhonguo4118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ae.zhonguo8118.cn

JS:   throw new Error("错误信息");
来源：https://no.zhonguo2118.cn

TS:   throw new Error("错误信息");
来源：https://bq.zhonguo1118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://dt.zhonguo2118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://hc.zhonguo8118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ne.zhonguo7118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://sz.zhonguo7118.cn

[H04] 自定义异常类型
来源：https://af.zhonguo6118.cn

Py:   class MyError(Exception): pass
来源：https://ca.zhonguo1118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://kc.zhonguo8118.cn

JS:   class MyError extends Error {}
来源：https://qy.zhonguo3118.cn

TS:   class MyError extends Error {}
来源：https://zs.zhonguo6118.cn

Java: class MyException extends RuntimeException {}
来源：https://se.zhonguo8118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://ra.zhonguo7118.cn

Ruby: class MyError < StandardError; end
来源：https://rp.zhonguo2118.cn

C#:   class MyException : Exception {}
来源：https://gf.zhonguo3118.cn

[H05] 捕获特定类型
来源：https://ht.zhonguo5118.cn

Py:   except ValueError as e:
来源：https://ly.zhonguo1118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://tx.zhonguo8118.cn

JS:   if (e instanceof TypeError) {}
来源：https://ih.zhonguo5118.cn

TS:   if (e instanceof TypeError) {}
来源：https://pe.zhonguo7118.cn

Java: catch (IOException | SQLException e) {}
来源：https://wz.zhonguo6118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://vr.zhonguo4118.cn

Ruby: rescue ArgumentError => e
来源：https://bw.zhonguo3118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://zo.zhonguo7118.cn

[H06] 可选值 / 空值安全访问
来源：https://gi.zhonguo8118.cn

Py:   value = d.get("k") or default
来源：https://tb.zhonguo1118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://qa.zhonguo2118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://bi.zhonguo4118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://rb.zhonguo2118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://rj.zhonguo1118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://pw.zhonguo5118.cn

Ruby: d&.dig(:a, :b)
来源：https://tx.zhonguo3118.cn

C#:   obj?.A?.B ?? default
来源：https://if.zhonguo8118.cn

[H07] 断言
来源：https://eo.zhonguo7118.cn

Py:   assert x > 0, "必须为正"
来源：https://jl.zhonguo8118.cn

PHP:  assert($x > 0);
来源：https://oi.zhonguo3118.cn

JS:   console.assert(x > 0);
来源：https://oq.zhonguo4118.cn

TS:   console.assert(x > 0);
来源：https://el.zhonguo7118.cn

Java: assert x > 0 : "必须为正";
来源：https://ci.zhonguo7118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://mj.zhonguo6118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://aj.zhonguo4118.cn

C#:   Debug.Assert(x > 0);
来源：https://lw.zhonguo3118.cn

[H08] 获取错误信息与堆栈
来源：https://ly.zhonguo5118.cn

Py:   str(e);  traceback.format_exc()
来源：https://rs.zhonguo6118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://qa.zhonguo1118.cn

JS:   e.message;  e.stack
来源：https://yr.zhonguo6118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://dy.zhonguo1118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://rv.zhonguo8118.cn

Go:   err.Error()
来源：https://qv.zhonguo6118.cn

Ruby: e.message;  e.backtrace
来源：https://qz.zhonguo3118.cn

C#:   e.Message;  e.StackTrace
来源：https://dy.zhonguo6118.cn

[H09] 带错误码的异常
来源：https://es.zhonguo2118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://gs.zhonguo5118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://mr.zhonguo3118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://hp.zhonguo7118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://pt.zhonguo6118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://ui.zhonguo1118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://bb.zhonguo6118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://za.zhonguo1118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://gu.zhonguo8118.cn

[H10] 资源自动释放
来源：https://pv.zhonguo7118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://wd.zhonguo1118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://rb.zhonguo3118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://mb.zhonguo4118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://ua.zhonguo1118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://hl.zhonguo6118.cn

Go:   defer f.Close()
来源：https://hs.zhonguo6118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://oz.zhonguo4118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://xv.zhonguo5118.cn

================================================================================
来源：https://jn.zhonguo2118.cn

I. 正则表达式
来源：https://rs.zhonguo3118.cn

================================================================================
来源：https://qt.zhonguo7118.cn

[I01] 判断是否匹配
来源：https://id.zhonguo1118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://ov.zhonguo1118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://us.zhonguo8118.cn

JS:   /\d+/.test(s)
来源：https://wh.zhonguo2118.cn

TS:   /\d+/.test(s)
来源：https://ke.zhonguo7118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://xm.zhonguo7118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://yg.zhonguo7118.cn

Ruby: s.match?(/\d+/)
来源：https://xd.zhonguo4118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://le.zhonguo7118.cn

[I02] 提取所有匹配
来源：https://qm.zhonguo4118.cn

Py:   re.findall(r"\d+", s)
来源：https://sd.zhonguo6118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://qb.zhonguo3118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://sf.zhonguo5118.cn

TS:   s.match(/\d+/g)
来源：https://uy.zhonguo7118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://hm.zhonguo6118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ot.zhonguo6118.cn

Ruby: s.scan(/\d+/)
来源：https://up.zhonguo1118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://kx.zhonguo8118.cn

[I03] 提取捕获分组
来源：https://kt.zhonguo4118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://dq.zhonguo1118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://qg.zhonguo1118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://oz.zhonguo8118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://wg.zhonguo2118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://xz.zhonguo4118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://im.zhonguo2118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://tx.zhonguo5118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://ip.zhonguo4118.cn

[I04] 正则替换
来源：https://mw.zhonguo8118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://yb.zhonguo3118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://cs.zhonguo8118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://gv.zhonguo1118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://mj.zhonguo6118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://yd.zhonguo3118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://ir.zhonguo1118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://es.zhonguo6118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://pa.zhonguo4118.cn

[I05] 按正则拆分
来源：https://ht.zhonguo5118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://dg.zhonguo6118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://cj.zhonguo7118.cn

JS:   s.split(/\s*,\s*/)
来源：https://ju.zhonguo2118.cn

TS:   s.split(/\s*,\s*/)
来源：https://tw.zhonguo6118.cn

Java: s.split("\\s*,\\s*")
来源：https://br.zhonguo6118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://nf.zhonguo8118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://ul.zhonguo6118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://yp.zhonguo6118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://lu.zhonguo5118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://dt.zhonguo6118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://ky.zhonguo5118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://sr.zhonguo8118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://xc.zhonguo3118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://hh.zhonguo2118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://ea.zhonguo6118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://tu.zhonguo8118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://dh.zhonguo6118.cn

[I07] 忽略大小写与多行模式
来源：https://ao.zhonguo1118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://uk.zhonguo7118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://hp.zhonguo6118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://it.zhonguo2118.cn

TS:   /error/gim
来源：https://qr.zhonguo2118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://is.zhonguo8118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://fb.zhonguo5118.cn

Ruby: s.scan(/error/i)
来源：https://dk.zhonguo5118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://ju.zhonguo8118.cn

[I08] 贪婪与非贪婪匹配
来源：https://os.zhonguo5118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://nd.zhonguo2118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://pp.zhonguo2118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://gk.zhonguo2118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://lf.zhonguo2118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://lx.zhonguo7118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://yz.zhonguo2118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://df.zhonguo3118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://qc.zhonguo7118.cn

================================================================================
来源：https://wu.zhonguo7118.cn

J. 日期与时间
来源：https://yc.zhonguo2118.cn

================================================================================
来源：https://cn.zhonguo7118.cn

[J01] 获取当前时间
来源：https://uy.zhonguo2118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://ub.zhonguo8118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://ak.zhonguo5118.cn

JS:   new Date();  Date.now()
来源：https://sw.zhonguo7118.cn

TS:   new Date();  Date.now()
来源：https://av.zhonguo7118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://qk.zhonguo6118.cn

Go:   time.Now()
来源：https://in.zhonguo3118.cn

Ruby: Time.now
来源：https://hz.zhonguo2118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://jj.zhonguo7118.cn

[J02] 格式化输出
来源：https://wd.zhonguo1118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://db.zhonguo5118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://xx.zhonguo7118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://nt.zhonguo7118.cn

TS:   d.toISOString()
来源：https://dk.zhonguo2118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://sb.zhonguo4118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://df.zhonguo5118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://dw.zhonguo5118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://tp.zhonguo6118.cn

[J03] 字符串解析为日期
来源：https://rv.zhonguo6118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://jv.zhonguo4118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://zh.zhonguo4118.cn

JS:   new Date("2024-01-02")
来源：https://bw.zhonguo7118.cn

TS:   new Date("2024-01-02")
来源：https://zl.zhonguo8118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://kd.zhonguo7118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://pf.zhonguo8118.cn

Ruby: Date.parse("2024-01-02")
来源：https://ct.zhonguo5118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://ak.zhonguo1118.cn

[J04] 时间戳与日期互转
来源：https://dt.zhonguo7118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://ev.zhonguo7118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://gg.zhonguo2118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://hg.zhonguo3118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://cu.zhonguo7118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://yo.zhonguo4118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://zx.zhonguo3118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://wz.zhonguo3118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://cr.zhonguo7118.cn

[J05] 时间加减（加 7 天）
来源：https://wp.zhonguo8118.cn

Py:   now + timedelta(days=7)
来源：https://zy.zhonguo7118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://dt.zhonguo8118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://oh.zhonguo3118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://rl.zhonguo4118.cn

Java: LocalDate.now().plusDays(7)
来源：https://js.zhonguo4118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://wb.zhonguo3118.cn

Ruby: Time.now + 7 * 86400
来源：https://vi.zhonguo2118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://kp.zhonguo2118.cn

[J06] 计算两时间之差
来源：https://ht.zhonguo1118.cn

Py:   (end - start).total_seconds()
来源：https://vh.zhonguo7118.cn

PHP:  $end->diff($start)->days;
来源：https://rv.zhonguo1118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://rp.zhonguo3118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://cg.zhonguo2118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://te.zhonguo5118.cn

Go:   end.Sub(start).Hours()
来源：https://ko.zhonguo6118.cn

Ruby: end - start                 # 返回秒数
来源：https://gj.zhonguo2118.cn

C#:   (end - start).TotalSeconds
来源：https://vm.zhonguo4118.cn

[J07] 比较两个日期
来源：https://xe.zhonguo3118.cn

Py:   d1 < d2;  d1 == d2
来源：https://dz.zhonguo8118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://hj.zhonguo1118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://qc.zhonguo2118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://hd.zhonguo4118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://ew.zhonguo2118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://ua.zhonguo5118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://zw.zhonguo7118.cn

C#:   d1 < d2;  d1 == d2
来源：https://nn.zhonguo6118.cn

[J08] 提取年月日与星期
来源：https://zi.zhonguo1118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://qc.zhonguo2118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://jt.zhonguo4118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://xc.zhonguo4118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://wz.zhonguo3118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://gp.zhonguo2118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://nc.zhonguo2118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://ss.zhonguo6118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://ce.zhonguo4118.cn

[J09] 时区处理
来源：https://ly.zhonguo5118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://di.zhonguo7118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://an.zhonguo3118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://ke.zhonguo7118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://cq.zhonguo7118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://ej.zhonguo4118.cn


<!-- 参考信息 -->