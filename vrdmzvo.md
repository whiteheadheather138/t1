代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：https://oz.zhonguo3118.cn

Ruby: def to_s; @name; end
来源：https://nt.zhonguo6118.cn

C#:   public override string ToString() => Name;
来源：https://or.zhonguo6118.cn

[G13] 判断对象类型
来源：https://oa.zhonguo7118.cn

Py:   isinstance(u, User)
来源：https://dd.zhonguo5118.cn

PHP:  $u instanceof User
来源：https://ku.zhonguo4118.cn

JS:   u instanceof User
来源：https://qi.zhonguo1118.cn

TS:   u instanceof User
来源：https://ws.zhonguo4118.cn

Java: u instanceof User
来源：https://aw.zhonguo7118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://am.zhonguo2118.cn

Ruby: u.is_a?(User)
来源：https://mw.zhonguo2118.cn

C#:   u is User
来源：https://sy.zhonguo5118.cn

[G14] 数据类 / record
来源：https://mj.zhonguo8118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://yr.zhonguo4118.cn

PHP:  // 用 readonly 属性模拟
来源：https://ww.zhonguo8118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://cm.zhonguo1118.cn

TS:   type User = { name: string; age: number };
来源：https://wd.zhonguo1118.cn

Java: record User(String name, int age) {}
来源：https://kv.zhonguo4118.cn

Go:   type User struct { Name string; Age int }
来源：https://pw.zhonguo2118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://yw.zhonguo7118.cn

C#:   record User(string Name, int Age);
来源：https://jm.zhonguo3118.cn

[G15] 枚举
来源：https://dx.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://fj.zhonguo2118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://ka.zhonguo7118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://vo.zhonguo8118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://qo.zhonguo7118.cn

Java: enum Color { RED, GREEN }
来源：https://sx.zhonguo4118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://hr.zhonguo2118.cn

Ruby: Color = %i[red green].freeze
来源：https://ql.zhonguo4118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://zc.zhonguo3118.cn

[G16] 对象转数组 / 字典
来源：https://ph.zhonguo4118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://nm.zhonguo1118.cn

PHP:  get_object_vars($obj);
来源：https://xm.zhonguo3118.cn

JS:   Object.entries(obj)
来源：https://zt.zhonguo7118.cn

TS:   Object.entries(obj)
来源：https://ca.zhonguo7118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://vd.zhonguo1118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://du.zhonguo2118.cn

Ruby: obj.instance_variables
来源：https://yx.zhonguo8118.cn

C#:   // 用反射或 System.Text.Json
来源：https://ll.zhonguo6118.cn

================================================================================
来源：https://bb.zhonguo2118.cn

H. 异常与错误处理
来源：https://jz.zhonguo8118.cn

================================================================================
来源：https://pp.zhonguo5118.cn

[H01] try / catch 基础
来源：https://zs.zhonguo3118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://uk.zhonguo1118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://ai.zhonguo3118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://zw.zhonguo6118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://ww.zhonguo2118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://ti.zhonguo6118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://yi.zhonguo6118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://mj.zhonguo4118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://qq.zhonguo4118.cn

[H02] finally / ensure 收尾
来源：https://mi.zhonguo5118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://yw.zhonguo4118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://rz.zhonguo7118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://mr.zhonguo2118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://co.zhonguo1118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://rf.zhonguo1118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://ov.zhonguo4118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://oi.zhonguo8118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://ly.zhonguo2118.cn

[H03] 主动抛出异常
来源：https://ff.zhonguo7118.cn

Py:   raise ValueError("错误信息")
来源：https://nb.zhonguo5118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ar.zhonguo1118.cn

JS:   throw new Error("错误信息");
来源：https://zw.zhonguo5118.cn

TS:   throw new Error("错误信息");
来源：https://vk.zhonguo4118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://gr.zhonguo7118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://ru.zhonguo7118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://jh.zhonguo6118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://mw.zhonguo5118.cn

[H04] 自定义异常类型
来源：https://xz.zhonguo7118.cn

Py:   class MyError(Exception): pass
来源：https://ak.zhonguo5118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://wf.zhonguo2118.cn

JS:   class MyError extends Error {}
来源：https://xc.zhonguo5118.cn

TS:   class MyError extends Error {}
来源：https://mo.zhonguo8118.cn

Java: class MyException extends RuntimeException {}
来源：https://ir.zhonguo6118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://uq.zhonguo3118.cn

Ruby: class MyError < StandardError; end
来源：https://au.zhonguo6118.cn

C#:   class MyException : Exception {}
来源：https://ba.zhonguo4118.cn

[H05] 捕获特定类型
来源：https://rc.zhonguo3118.cn

Py:   except ValueError as e:
来源：https://vd.zhonguo3118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://px.zhonguo6118.cn

JS:   if (e instanceof TypeError) {}
来源：https://bv.zhonguo3118.cn

TS:   if (e instanceof TypeError) {}
来源：https://vg.zhonguo5118.cn

Java: catch (IOException | SQLException e) {}
来源：https://ml.zhonguo6118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://qz.zhonguo2118.cn

Ruby: rescue ArgumentError => e
来源：https://xn.zhonguo5118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://uf.zhonguo8118.cn

[H06] 可选值 / 空值安全访问
来源：https://ad.zhonguo2118.cn

Py:   value = d.get("k") or default
来源：https://ux.zhonguo7118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://nq.zhonguo3118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://gr.zhonguo2118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://we.zhonguo6118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://tg.zhonguo4118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://qn.zhonguo5118.cn

Ruby: d&.dig(:a, :b)
来源：https://zg.zhonguo4118.cn

C#:   obj?.A?.B ?? default
来源：https://na.zhonguo2118.cn

[H07] 断言
来源：https://rq.zhonguo2118.cn

Py:   assert x > 0, "必须为正"
来源：https://jr.zhonguo4118.cn

PHP:  assert($x > 0);
来源：https://io.zhonguo3118.cn

JS:   console.assert(x > 0);
来源：https://yb.zhonguo7118.cn

TS:   console.assert(x > 0);
来源：https://nj.zhonguo5118.cn

Java: assert x > 0 : "必须为正";
来源：https://kf.zhonguo6118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://ur.zhonguo3118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://jh.zhonguo3118.cn

C#:   Debug.Assert(x > 0);
来源：https://pz.zhonguo6118.cn

[H08] 获取错误信息与堆栈
来源：https://oh.zhonguo4118.cn

Py:   str(e);  traceback.format_exc()
来源：https://mo.zhonguo5118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://gz.zhonguo6118.cn

JS:   e.message;  e.stack
来源：https://xb.zhonguo6118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://zj.zhonguo2118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://tw.zhonguo4118.cn

Go:   err.Error()
来源：https://aj.zhonguo5118.cn

Ruby: e.message;  e.backtrace
来源：https://sz.zhonguo8118.cn

C#:   e.Message;  e.StackTrace
来源：https://lk.zhonguo8118.cn

[H09] 带错误码的异常
来源：https://fe.zhonguo5118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://po.zhonguo6118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://mt.zhonguo7118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://la.zhonguo2118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://hn.zhonguo2118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://nz.zhonguo7118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://gw.zhonguo2118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://cv.zhonguo1118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://ck.zhonguo7118.cn

[H10] 资源自动释放
来源：https://vz.zhonguo6118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://hf.zhonguo3118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://qe.zhonguo6118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://bw.zhonguo7118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://hl.zhonguo7118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://gx.zhonguo6118.cn

Go:   defer f.Close()
来源：https://qo.zhonguo3118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://ky.zhonguo1118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://lx.zhonguo1118.cn

================================================================================
来源：https://pd.zhonguo5118.cn

I. 正则表达式
来源：https://jm.zhonguo1118.cn

================================================================================
来源：https://tb.zhonguo8118.cn

[I01] 判断是否匹配
来源：https://qs.zhonguo1118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://zu.zhonguo6118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://mf.zhonguo5118.cn

JS:   /\d+/.test(s)
来源：https://gz.zhonguo1118.cn

TS:   /\d+/.test(s)
来源：https://ij.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://yv.zhonguo3118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://fz.zhonguo2118.cn

Ruby: s.match?(/\d+/)
来源：https://vb.zhonguo5118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://te.zhonguo7118.cn

[I02] 提取所有匹配
来源：https://kr.zhonguo3118.cn

Py:   re.findall(r"\d+", s)
来源：https://mo.zhonguo6118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://pv.zhonguo7118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://qr.zhonguo2118.cn

TS:   s.match(/\d+/g)
来源：https://ck.zhonguo3118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://cl.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://pj.zhonguo6118.cn

Ruby: s.scan(/\d+/)
来源：https://ax.zhonguo5118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://cd.zhonguo8118.cn

[I03] 提取捕获分组
来源：https://hr.zhonguo4118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://go.zhonguo6118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://fd.zhonguo3118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://qt.zhonguo2118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://sz.zhonguo2118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://oo.zhonguo5118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://ne.zhonguo8118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://ct.zhonguo6118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://wt.zhonguo3118.cn

[I04] 正则替换
来源：https://ff.zhonguo5118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://dh.zhonguo1118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://dt.zhonguo8118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://sa.zhonguo2118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://uw.zhonguo4118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://is.zhonguo5118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://zo.zhonguo7118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://tx.zhonguo6118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://ma.zhonguo8118.cn

[I05] 按正则拆分
来源：https://qp.zhonguo1118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://ll.zhonguo5118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://ll.zhonguo3118.cn

JS:   s.split(/\s*,\s*/)
来源：https://cg.zhonguo6118.cn

TS:   s.split(/\s*,\s*/)
来源：https://hy.zhonguo6118.cn

Java: s.split("\\s*,\\s*")
来源：https://mh.zhonguo6118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://dc.zhonguo7118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://mu.zhonguo2118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://ua.zhonguo5118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://ok.zhonguo3118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://gw.zhonguo7118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://bc.zhonguo5118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://vl.zhonguo8118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://la.zhonguo4118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://nw.zhonguo4118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://on.zhonguo4118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://qs.zhonguo6118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://fb.zhonguo2118.cn

[I07] 忽略大小写与多行模式
来源：https://qs.zhonguo7118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://up.zhonguo7118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://wq.zhonguo8118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://sw.zhonguo7118.cn

TS:   /error/gim
来源：https://da.zhonguo6118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://ax.zhonguo7118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://kv.zhonguo3118.cn

Ruby: s.scan(/error/i)
来源：https://pa.zhonguo2118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://ap.zhonguo3118.cn

[I08] 贪婪与非贪婪匹配
来源：https://vk.zhonguo8118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://ew.zhonguo1118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://sg.zhonguo4118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://np.zhonguo4118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://qe.zhonguo2118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://gy.zhonguo4118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://rw.zhonguo5118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://gg.zhonguo8118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://ft.zhonguo5118.cn

================================================================================
来源：https://ni.zhonguo6118.cn

J. 日期与时间
来源：https://qi.zhonguo4118.cn

================================================================================
来源：https://dx.zhonguo4118.cn

[J01] 获取当前时间
来源：https://wd.zhonguo2118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://wq.zhonguo5118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://ps.zhonguo7118.cn

JS:   new Date();  Date.now()
来源：https://od.zhonguo5118.cn

TS:   new Date();  Date.now()
来源：https://ft.zhonguo3118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://rr.zhonguo2118.cn

Go:   time.Now()
来源：https://ml.zhonguo3118.cn

Ruby: Time.now
来源：https://et.zhonguo4118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://nm.zhonguo7118.cn

[J02] 格式化输出
来源：https://mt.zhonguo3118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://yr.zhonguo3118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://zv.zhonguo6118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://jm.zhonguo5118.cn

TS:   d.toISOString()
来源：https://zj.zhonguo4118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://fs.zhonguo7118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://da.zhonguo3118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://di.zhonguo4118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://mh.zhonguo4118.cn

[J03] 字符串解析为日期
来源：https://ml.zhonguo7118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://kn.zhonguo8118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://lb.zhonguo4118.cn

JS:   new Date("2024-01-02")
来源：https://lu.zhonguo7118.cn

TS:   new Date("2024-01-02")
来源：https://ys.zhonguo5118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://rj.zhonguo3118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://sq.zhonguo7118.cn

Ruby: Date.parse("2024-01-02")
来源：https://sd.zhonguo4118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://ea.zhonguo8118.cn

[J04] 时间戳与日期互转
来源：https://oh.zhonguo8118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://al.zhonguo1118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://ik.zhonguo3118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://jx.zhonguo1118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://wm.zhonguo8118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://fa.zhonguo1118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://ws.zhonguo6118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://mp.zhonguo5118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://qd.zhonguo6118.cn

[J05] 时间加减（加 7 天）
来源：https://zu.zhonguo5118.cn

Py:   now + timedelta(days=7)
来源：https://bc.zhonguo4118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://xj.zhonguo2118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://nl.zhonguo7118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://ws.zhonguo3118.cn

Java: LocalDate.now().plusDays(7)
来源：https://rk.zhonguo3118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://wa.zhonguo4118.cn

Ruby: Time.now + 7 * 86400
来源：https://rl.zhonguo4118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://nb.zhonguo2118.cn

[J06] 计算两时间之差
来源：https://ft.zhonguo6118.cn

Py:   (end - start).total_seconds()
来源：https://iu.zhonguo2118.cn

PHP:  $end->diff($start)->days;
来源：https://hc.zhonguo3118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://mk.zhonguo6118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://bq.zhonguo5118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://sp.zhonguo7118.cn

Go:   end.Sub(start).Hours()
来源：https://pn.zhonguo6118.cn

Ruby: end - start                 # 返回秒数
来源：https://kx.zhonguo7118.cn

C#:   (end - start).TotalSeconds
来源：https://ic.zhonguo6118.cn

[J07] 比较两个日期
来源：https://kh.zhonguo2118.cn

Py:   d1 < d2;  d1 == d2
来源：https://xe.zhonguo8118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://vi.zhonguo8118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://hk.zhonguo2118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://xw.zhonguo5118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://uz.zhonguo2118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://lg.zhonguo6118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://ix.zhonguo4118.cn

C#:   d1 < d2;  d1 == d2
来源：https://av.zhonguo6118.cn

[J08] 提取年月日与星期
来源：https://xm.zhonguo3118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://vm.zhonguo4118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://zk.zhonguo6118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://hj.zhonguo4118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://rz.zhonguo5118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://tt.zhonguo5118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://tu.zhonguo5118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://tu.zhonguo5118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://ns.zhonguo3118.cn

[J09] 时区处理
来源：https://ml.zhonguo4118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://cn.zhonguo8118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://lu.zhonguo5118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://xx.zhonguo4118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://md.zhonguo5118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://nn.zhonguo4118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://pq.zhonguo8118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://tj.zhonguo8118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://sq.zhonguo5118.cn

[J10] 取今天 / 本月第一天
来源：https://ou.zhonguo8118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://nr.zhonguo7118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://ip.zhonguo4118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://bp.zhonguo5118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://xq.zhonguo7118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://ye.zhonguo2118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://nd.zhonguo7118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://yz.zhonguo8118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://kq.zhonguo5118.cn


<!-- 参考信息 -->