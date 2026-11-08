代发 wailian999

TS:   throw new Error("错误信息");
来源：https://fw.zhonguo3118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://sh.zhonguo4118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://gh.zhonguo3118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://kv.zhonguo1118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://fu.zhonguo2118.cn

[H04] 自定义异常类型
来源：https://vi.zhonguo7118.cn

Py:   class MyError(Exception): pass
来源：https://mo.zhonguo5118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://rt.zhonguo4118.cn

JS:   class MyError extends Error {}
来源：https://sm.zhonguo2118.cn

TS:   class MyError extends Error {}
来源：https://dw.zhonguo2118.cn

Java: class MyException extends RuntimeException {}
来源：https://bc.zhonguo2118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://rx.zhonguo6118.cn

Ruby: class MyError < StandardError; end
来源：https://vp.zhonguo1118.cn

C#:   class MyException : Exception {}
来源：https://ks.zhonguo4118.cn

[H05] 捕获特定类型
来源：https://oq.zhonguo8118.cn

Py:   except ValueError as e:
来源：https://ue.zhonguo2118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://zf.zhonguo4118.cn

JS:   if (e instanceof TypeError) {}
来源：https://ec.zhonguo8118.cn

TS:   if (e instanceof TypeError) {}
来源：https://xe.zhonguo2118.cn

Java: catch (IOException | SQLException e) {}
来源：https://iz.zhonguo4118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://fc.zhonguo8118.cn

Ruby: rescue ArgumentError => e
来源：https://bf.zhonguo6118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://pb.zhonguo6118.cn

[H06] 可选值 / 空值安全访问
来源：https://ud.zhonguo6118.cn

Py:   value = d.get("k") or default
来源：https://yf.zhonguo5118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://ug.zhonguo8118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://pe.zhonguo5118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://kw.zhonguo2118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://ct.zhonguo8118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://ox.zhonguo4118.cn

Ruby: d&.dig(:a, :b)
来源：https://qb.zhonguo3118.cn

C#:   obj?.A?.B ?? default
来源：https://eh.zhonguo2118.cn

[H07] 断言
来源：https://jf.zhonguo4118.cn

Py:   assert x > 0, "必须为正"
来源：https://cg.zhonguo5118.cn

PHP:  assert($x > 0);
来源：https://gl.zhonguo4118.cn

JS:   console.assert(x > 0);
来源：https://rk.zhonguo1118.cn

TS:   console.assert(x > 0);
来源：https://xy.zhonguo4118.cn

Java: assert x > 0 : "必须为正";
来源：https://mi.zhonguo5118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://tn.zhonguo2118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://mm.zhonguo3118.cn

C#:   Debug.Assert(x > 0);
来源：https://xl.zhonguo8118.cn

[H08] 获取错误信息与堆栈
来源：https://br.zhonguo6118.cn

Py:   str(e);  traceback.format_exc()
来源：https://fv.zhonguo7118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://wi.zhonguo4118.cn

JS:   e.message;  e.stack
来源：https://xz.zhonguo6118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://gk.zhonguo2118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://cp.zhonguo8118.cn

Go:   err.Error()
来源：https://ga.zhonguo4118.cn

Ruby: e.message;  e.backtrace
来源：https://xi.zhonguo4118.cn

C#:   e.Message;  e.StackTrace
来源：https://dz.zhonguo3118.cn

[H09] 带错误码的异常
来源：https://pi.zhonguo4118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://jc.zhonguo8118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://yw.zhonguo5118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://xm.zhonguo1118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://jc.zhonguo8118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://zv.zhonguo7118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://hq.zhonguo2118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://cn.zhonguo8118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://wy.zhonguo5118.cn

[H10] 资源自动释放
来源：https://ez.zhonguo2118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://cq.zhonguo7118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://fl.zhonguo2118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://nd.zhonguo6118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://gr.zhonguo5118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://xt.zhonguo3118.cn

Go:   defer f.Close()
来源：https://sm.zhonguo8118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://jy.zhonguo3118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://rp.zhonguo3118.cn

================================================================================
来源：https://ae.zhonguo2118.cn

I. 正则表达式
来源：https://xv.zhonguo2118.cn

================================================================================
来源：https://fq.zhonguo5118.cn

[I01] 判断是否匹配
来源：https://ii.zhonguo4118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://ef.zhonguo4118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://cm.zhonguo8118.cn

JS:   /\d+/.test(s)
来源：https://dm.zhonguo8118.cn

TS:   /\d+/.test(s)
来源：https://qb.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://dw.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://as.zhonguo8118.cn

Ruby: s.match?(/\d+/)
来源：https://fc.zhonguo3118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://pl.zhonguo2118.cn

[I02] 提取所有匹配
来源：https://ni.zhonguo2118.cn

Py:   re.findall(r"\d+", s)
来源：https://qu.zhonguo5118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://np.zhonguo7118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://xa.zhonguo6118.cn

TS:   s.match(/\d+/g)
来源：https://fi.zhonguo7118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://mx.zhonguo7118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ir.zhonguo4118.cn

Ruby: s.scan(/\d+/)
来源：https://lo.zhonguo3118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://dd.zhonguo3118.cn

[I03] 提取捕获分组
来源：https://ry.zhonguo7118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://xe.zhonguo3118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://bc.zhonguo4118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://tr.zhonguo3118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://sx.zhonguo7118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://js.zhonguo8118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://di.zhonguo7118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://te.zhonguo1118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://hs.zhonguo4118.cn

[I04] 正则替换
来源：https://au.zhonguo5118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://lr.zhonguo4118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://lg.zhonguo2118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://tg.zhonguo8118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://go.zhonguo8118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://sk.zhonguo1118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://fh.zhonguo5118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://zv.zhonguo1118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://nm.zhonguo4118.cn

[I05] 按正则拆分
来源：https://ip.zhonguo3118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://he.zhonguo1118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://yz.zhonguo8118.cn

JS:   s.split(/\s*,\s*/)
来源：https://ho.zhonguo3118.cn

TS:   s.split(/\s*,\s*/)
来源：https://fh.zhonguo4118.cn

Java: s.split("\\s*,\\s*")
来源：https://rp.zhonguo6118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://hr.zhonguo2118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://nq.zhonguo2118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://li.zhonguo1118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://ew.zhonguo3118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://yt.zhonguo1118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://rv.zhonguo1118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://zc.zhonguo5118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://xs.zhonguo3118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://is.zhonguo8118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://xd.zhonguo6118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://lj.zhonguo6118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://zo.zhonguo3118.cn

[I07] 忽略大小写与多行模式
来源：https://nx.zhonguo7118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://ii.zhonguo8118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://je.zhonguo1118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://jo.zhonguo2118.cn

TS:   /error/gim
来源：https://yn.zhonguo8118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://de.zhonguo2118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://vv.zhonguo8118.cn

Ruby: s.scan(/error/i)
来源：https://wk.zhonguo6118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://li.zhonguo1118.cn

[I08] 贪婪与非贪婪匹配
来源：https://cg.zhonguo5118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://yr.zhonguo1118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://ri.zhonguo3118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://qp.zhonguo6118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://hc.zhonguo4118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://rs.zhonguo7118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://zb.zhonguo2118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://wh.zhonguo8118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://xd.zhonguo4118.cn

================================================================================
来源：https://qq.zhonguo6118.cn

J. 日期与时间
来源：https://bh.zhonguo6118.cn

================================================================================
来源：https://gr.zhonguo6118.cn

[J01] 获取当前时间
来源：https://li.zhonguo7118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://pl.zhonguo1118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://qm.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://qd.zhonguo4118.cn

TS:   new Date();  Date.now()
来源：https://nn.zhonguo8118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://ag.zhonguo1118.cn

Go:   time.Now()
来源：https://md.zhonguo3118.cn

Ruby: Time.now
来源：https://so.zhonguo8118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://ym.zhonguo7118.cn

[J02] 格式化输出
来源：https://pj.zhonguo2118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://dj.zhonguo8118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://ek.zhonguo1118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://gl.zhonguo6118.cn

TS:   d.toISOString()
来源：https://yn.zhonguo8118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://qn.zhonguo1118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://qt.zhonguo4118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://dt.zhonguo3118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://ve.zhonguo8118.cn

[J03] 字符串解析为日期
来源：https://ch.zhonguo7118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://mg.zhonguo5118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://wn.zhonguo8118.cn

JS:   new Date("2024-01-02")
来源：https://yf.zhonguo3118.cn

TS:   new Date("2024-01-02")
来源：https://xb.zhonguo1118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://nl.zhonguo4118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://nd.zhonguo2118.cn

Ruby: Date.parse("2024-01-02")
来源：https://dw.zhonguo5118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://cn.zhonguo3118.cn

[J04] 时间戳与日期互转
来源：https://ow.zhonguo5118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://ol.zhonguo1118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://ff.zhonguo3118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://rr.zhonguo5118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://na.zhonguo5118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://fm.zhonguo2118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://cb.zhonguo7118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://er.zhonguo1118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://xh.zhonguo6118.cn

[J05] 时间加减（加 7 天）
来源：https://ju.zhonguo4118.cn

Py:   now + timedelta(days=7)
来源：https://uo.zhonguo2118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://gr.zhonguo8118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://pw.zhonguo7118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://lo.zhonguo8118.cn

Java: LocalDate.now().plusDays(7)
来源：https://ph.zhonguo8118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://xp.zhonguo3118.cn

Ruby: Time.now + 7 * 86400
来源：https://mm.zhonguo5118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://qq.zhonguo7118.cn

[J06] 计算两时间之差
来源：https://sy.zhonguo5118.cn

Py:   (end - start).total_seconds()
来源：https://he.zhonguo7118.cn

PHP:  $end->diff($start)->days;
来源：https://mj.zhonguo2118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://vl.zhonguo7118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://ej.zhonguo3118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://zl.zhonguo8118.cn

Go:   end.Sub(start).Hours()
来源：https://wj.zhonguo4118.cn

Ruby: end - start                 # 返回秒数
来源：https://ky.zhonguo3118.cn

C#:   (end - start).TotalSeconds
来源：https://zy.zhonguo1118.cn

[J07] 比较两个日期
来源：https://am.zhonguo6118.cn

Py:   d1 < d2;  d1 == d2
来源：https://ze.zhonguo2118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://qc.zhonguo1118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://ly.zhonguo6118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://ga.zhonguo3118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://kl.zhonguo8118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://ox.zhonguo5118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://rm.zhonguo1118.cn

C#:   d1 < d2;  d1 == d2
来源：https://mw.zhonguo2118.cn

[J08] 提取年月日与星期
来源：https://wg.zhonguo1118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://hd.zhonguo7118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://ha.zhonguo7118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://zm.zhonguo3118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://uh.zhonguo6118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://gs.zhonguo2118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://oa.zhonguo5118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://gc.zhonguo1118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://pk.zhonguo1118.cn

[J09] 时区处理
来源：https://hs.zhonguo1118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://fm.zhonguo4118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://kn.zhonguo3118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://wo.zhonguo1118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://ku.zhonguo2118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://vr.zhonguo8118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://cd.zhonguo3118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://hh.zhonguo5118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://uu.zhonguo2118.cn

[J10] 取今天 / 本月第一天
来源：https://lt.zhonguo7118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://br.zhonguo6118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://pe.zhonguo5118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://ja.zhonguo5118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://kl.zhonguo1118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://lh.zhonguo4118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://th.zhonguo8118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://pi.zhonguo3118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://cy.zhonguo8118.cn

================================================================================
来源：https://wj.zhonguo1118.cn

K. JSON 与序列化
来源：https://ib.zhonguo8118.cn

================================================================================
来源：https://kl.zhonguo2118.cn

[K01] 对象转 JSON 字符串
来源：https://cg.zhonguo7118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://zg.zhonguo8118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://gd.zhonguo4118.cn

JS:   JSON.stringify(obj)
来源：https://cb.zhonguo4118.cn

TS:   JSON.stringify(obj)
来源：https://ql.zhonguo1118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://jk.zhonguo8118.cn

Go:   json.Marshal(obj)
来源：https://gt.zhonguo3118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://dc.zhonguo1118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://wk.zhonguo5118.cn

[K02] JSON 字符串转对象
来源：https://gy.zhonguo7118.cn

Py:   json.loads(s)
来源：https://on.zhonguo6118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://ab.zhonguo3118.cn

JS:   JSON.parse(s)
来源：https://gp.zhonguo3118.cn

TS:   JSON.parse(s)
来源：https://oo.zhonguo4118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://ev.zhonguo6118.cn

Go:   json.Unmarshal(data, &v)
来源：https://lj.zhonguo8118.cn

Ruby: JSON.parse(s)
来源：https://zp.zhonguo4118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://ri.zhonguo1118.cn

[K03] JSON 美化输出（带缩进）
来源：https://we.zhonguo6118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://vt.zhonguo8118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://to.zhonguo6118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://rv.zhonguo3118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://xr.zhonguo3118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://yv.zhonguo4118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://ue.zhonguo2118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://zq.zhonguo5118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://pc.zhonguo2118.cn

[K04] 读取 JSON 文件
来源：https://kt.zhonguo2118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://qy.zhonguo7118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://er.zhonguo2118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://si.zhonguo4118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ls.zhonguo6118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://dz.zhonguo3118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://fu.zhonguo4118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://ah.zhonguo3118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://tc.zhonguo5118.cn

[K05] 深拷贝对象
来源：https://cp.zhonguo3118.cn

Py:   copy.deepcopy(obj)
来源：https://wi.zhonguo8118.cn

PHP:  unserialize(serialize($obj));
来源：https://un.zhonguo1118.cn

JS:   structuredClone(obj)
来源：https://oe.zhonguo1118.cn

TS:   structuredClone(obj)
来源：https://cv.zhonguo1118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://ux.zhonguo6118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://ci.zhonguo4118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://kh.zhonguo5118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://ii.zhonguo2118.cn

[K06] 解析 URL 查询串
来源：https://iv.zhonguo6118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://sc.zhonguo6118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://vy.zhonguo4118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://gi.zhonguo6118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://ii.zhonguo1118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://kp.zhonguo5118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://vu.zhonguo8118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://es.zhonguo5118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://pb.zhonguo3118.cn

[K07] 进制转换
来源：https://os.zhonguo1118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://cx.zhonguo7118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://ew.zhonguo5118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://tj.zhonguo3118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://ro.zhonguo2118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://zo.zhonguo3118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://yh.zhonguo1118.cn


<!-- 参考信息 -->