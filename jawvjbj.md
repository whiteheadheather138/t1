代发 wailian999

Ruby: class MyError < StandardError; end
来源：https://sk.zhonguo7118.cn

C#:   class MyException : Exception {}
来源：https://lu.zhonguo2118.cn

[H05] 捕获特定类型
来源：https://md.zhonguo2118.cn

Py:   except ValueError as e:
来源：https://hn.zhonguo2118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://dm.zhonguo6118.cn

JS:   if (e instanceof TypeError) {}
来源：https://ti.zhonguo4118.cn

TS:   if (e instanceof TypeError) {}
来源：https://cx.zhonguo2118.cn

Java: catch (IOException | SQLException e) {}
来源：https://ru.zhonguo7118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://mi.zhonguo8118.cn

Ruby: rescue ArgumentError => e
来源：https://uj.zhonguo5118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://xd.zhonguo7118.cn

[H06] 可选值 / 空值安全访问
来源：https://iy.zhonguo7118.cn

Py:   value = d.get("k") or default
来源：https://kk.zhonguo5118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://df.zhonguo1118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://xw.zhonguo2118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://qq.zhonguo8118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://fy.zhonguo7118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://vt.zhonguo6118.cn

Ruby: d&.dig(:a, :b)
来源：https://by.zhonguo6118.cn

C#:   obj?.A?.B ?? default
来源：https://qe.zhonguo8118.cn

[H07] 断言
来源：https://oz.zhonguo5118.cn

Py:   assert x > 0, "必须为正"
来源：https://vc.zhonguo3118.cn

PHP:  assert($x > 0);
来源：https://ox.zhonguo7118.cn

JS:   console.assert(x > 0);
来源：https://zo.zhonguo8118.cn

TS:   console.assert(x > 0);
来源：https://jc.zhonguo5118.cn

Java: assert x > 0 : "必须为正";
来源：https://sf.zhonguo7118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://mx.zhonguo7118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://zt.zhonguo1118.cn

C#:   Debug.Assert(x > 0);
来源：https://fn.zhonguo4118.cn

[H08] 获取错误信息与堆栈
来源：https://ie.zhonguo5118.cn

Py:   str(e);  traceback.format_exc()
来源：https://mq.zhonguo1118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://ab.zhonguo8118.cn

JS:   e.message;  e.stack
来源：https://jd.zhonguo2118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://pi.zhonguo1118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://ff.zhonguo3118.cn

Go:   err.Error()
来源：https://kv.zhonguo6118.cn

Ruby: e.message;  e.backtrace
来源：https://oe.zhonguo6118.cn

C#:   e.Message;  e.StackTrace
来源：https://lh.zhonguo8118.cn

[H09] 带错误码的异常
来源：https://sd.zhonguo7118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://tg.zhonguo5118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://wc.zhonguo7118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://ig.zhonguo4118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://oa.zhonguo5118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://xr.zhonguo2118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://lr.zhonguo7118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://sd.zhonguo6118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://tq.zhonguo5118.cn

[H10] 资源自动释放
来源：https://eu.zhonguo7118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://kp.zhonguo6118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://gu.zhonguo4118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://qj.zhonguo7118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://ao.zhonguo2118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://xz.zhonguo7118.cn

Go:   defer f.Close()
来源：https://nj.zhonguo6118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://ge.zhonguo1118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://cf.zhonguo4118.cn

================================================================================
来源：https://rn.zhonguo5118.cn

I. 正则表达式
来源：https://sf.zhonguo7118.cn

================================================================================
来源：https://pg.zhonguo8118.cn

[I01] 判断是否匹配
来源：https://hz.zhonguo7118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://dp.zhonguo5118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://pl.zhonguo7118.cn

JS:   /\d+/.test(s)
来源：https://si.zhonguo3118.cn

TS:   /\d+/.test(s)
来源：https://hd.zhonguo2118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://wt.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://dd.zhonguo8118.cn

Ruby: s.match?(/\d+/)
来源：https://xc.zhonguo2118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://kv.zhonguo3118.cn

[I02] 提取所有匹配
来源：https://bl.zhonguo4118.cn

Py:   re.findall(r"\d+", s)
来源：https://id.zhonguo1118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://aw.zhonguo6118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://ci.zhonguo7118.cn

TS:   s.match(/\d+/g)
来源：https://fu.zhonguo3118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://ww.zhonguo6118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://gj.zhonguo2118.cn

Ruby: s.scan(/\d+/)
来源：https://rd.zhonguo4118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://aq.zhonguo3118.cn

[I03] 提取捕获分组
来源：https://yd.zhonguo7118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://nq.zhonguo2118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://ve.zhonguo4118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://oj.zhonguo7118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://of.zhonguo5118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://ua.zhonguo3118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://xa.zhonguo8118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://sd.zhonguo4118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://mo.zhonguo7118.cn

[I04] 正则替换
来源：https://pi.zhonguo4118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://da.zhonguo7118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://ga.zhonguo3118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://wg.zhonguo2118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://aa.zhonguo3118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://xg.zhonguo8118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://gx.zhonguo6118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://qe.zhonguo2118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://kw.zhonguo3118.cn

[I05] 按正则拆分
来源：https://nu.zhonguo7118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://yb.zhonguo8118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://nf.zhonguo6118.cn

JS:   s.split(/\s*,\s*/)
来源：https://pn.zhonguo8118.cn

TS:   s.split(/\s*,\s*/)
来源：https://xy.zhonguo6118.cn

Java: s.split("\\s*,\\s*")
来源：https://jx.zhonguo5118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://id.zhonguo4118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://bo.zhonguo1118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://ly.zhonguo5118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://xa.zhonguo4118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://dg.zhonguo2118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://df.zhonguo2118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://fh.zhonguo8118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://pa.zhonguo3118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://ia.zhonguo4118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://zz.zhonguo2118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://pn.zhonguo7118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://ye.zhonguo5118.cn

[I07] 忽略大小写与多行模式
来源：https://rv.zhonguo6118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://wd.zhonguo2118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://av.zhonguo2118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://qq.zhonguo8118.cn

TS:   /error/gim
来源：https://qz.zhonguo6118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://ra.zhonguo5118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://dr.zhonguo6118.cn

Ruby: s.scan(/error/i)
来源：https://xs.zhonguo4118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://yg.zhonguo1118.cn

[I08] 贪婪与非贪婪匹配
来源：https://ws.zhonguo1118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://fs.zhonguo2118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://nq.zhonguo4118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://iw.zhonguo8118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://sz.zhonguo3118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://jv.zhonguo2118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://qr.zhonguo8118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://kn.zhonguo4118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://ds.zhonguo7118.cn

================================================================================
来源：https://xj.zhonguo5118.cn

J. 日期与时间
来源：https://zy.zhonguo4118.cn

================================================================================
来源：https://xs.zhonguo8118.cn

[J01] 获取当前时间
来源：https://cz.zhonguo5118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://nq.zhonguo7118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://vm.zhonguo5118.cn

JS:   new Date();  Date.now()
来源：https://nc.zhonguo2118.cn

TS:   new Date();  Date.now()
来源：https://jk.zhonguo3118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://qk.zhonguo3118.cn

Go:   time.Now()
来源：https://gu.zhonguo1118.cn

Ruby: Time.now
来源：https://xg.zhonguo5118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://qn.zhonguo7118.cn

[J02] 格式化输出
来源：https://xv.zhonguo3118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://uh.zhonguo2118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://ck.zhonguo8118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://eu.zhonguo3118.cn

TS:   d.toISOString()
来源：https://gp.zhonguo7118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://sy.zhonguo2118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://kq.zhonguo7118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://yn.zhonguo5118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://nd.zhonguo4118.cn

[J03] 字符串解析为日期
来源：https://rk.zhonguo7118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://qh.zhonguo2118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://nb.zhonguo7118.cn

JS:   new Date("2024-01-02")
来源：https://hp.zhonguo1118.cn

TS:   new Date("2024-01-02")
来源：https://xo.zhonguo5118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://di.zhonguo5118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://xo.zhonguo2118.cn

Ruby: Date.parse("2024-01-02")
来源：https://vc.zhonguo8118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://ar.zhonguo4118.cn

[J04] 时间戳与日期互转
来源：https://ni.zhonguo8118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://hi.zhonguo2118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://rk.zhonguo6118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://wq.zhonguo5118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://wz.zhonguo6118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://oy.zhonguo4118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://xi.zhonguo2118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://lj.zhonguo1118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://km.zhonguo8118.cn

[J05] 时间加减（加 7 天）
来源：https://qv.zhonguo5118.cn

Py:   now + timedelta(days=7)
来源：https://yg.zhonguo2118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://ez.zhonguo4118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://bz.zhonguo1118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://db.zhonguo3118.cn

Java: LocalDate.now().plusDays(7)
来源：https://va.zhonguo4118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://oh.zhonguo1118.cn

Ruby: Time.now + 7 * 86400
来源：https://tg.zhonguo1118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://uy.zhonguo6118.cn

[J06] 计算两时间之差
来源：https://zn.zhonguo1118.cn

Py:   (end - start).total_seconds()
来源：https://cc.zhonguo4118.cn

PHP:  $end->diff($start)->days;
来源：https://uu.zhonguo1118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://xx.zhonguo6118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://hg.zhonguo4118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://fi.zhonguo3118.cn

Go:   end.Sub(start).Hours()
来源：https://wm.zhonguo6118.cn

Ruby: end - start                 # 返回秒数
来源：https://uk.zhonguo8118.cn

C#:   (end - start).TotalSeconds
来源：https://ir.zhonguo3118.cn

[J07] 比较两个日期
来源：https://qo.zhonguo5118.cn

Py:   d1 < d2;  d1 == d2
来源：https://qu.zhonguo3118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://uw.zhonguo3118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://qt.zhonguo7118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://qo.zhonguo1118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://nu.zhonguo3118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://eu.zhonguo7118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://nk.zhonguo6118.cn

C#:   d1 < d2;  d1 == d2
来源：https://bl.zhonguo7118.cn

[J08] 提取年月日与星期
来源：https://ys.zhonguo4118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://nk.zhonguo2118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://jm.zhonguo3118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://gs.zhonguo2118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://jg.zhonguo7118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://yb.zhonguo6118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://zp.zhonguo2118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://xt.zhonguo4118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://xt.zhonguo8118.cn

[J09] 时区处理
来源：https://py.zhonguo7118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://qo.zhonguo3118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://lm.zhonguo1118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://nd.zhonguo1118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://en.zhonguo7118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://eb.zhonguo3118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://hb.zhonguo3118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://ic.zhonguo3118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://oc.zhonguo8118.cn

[J10] 取今天 / 本月第一天
来源：https://ny.zhonguo4118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://gf.zhonguo1118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://xl.zhonguo2118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://lm.zhonguo5118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://jr.zhonguo6118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://ur.zhonguo6118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://pj.zhonguo5118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://hi.zhonguo1118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://ow.zhonguo8118.cn

================================================================================
来源：https://rm.zhonguo4118.cn

K. JSON 与序列化
来源：https://zs.zhonguo6118.cn

================================================================================
来源：https://of.zhonguo6118.cn

[K01] 对象转 JSON 字符串
来源：https://sj.zhonguo5118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://to.zhonguo4118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://pn.zhonguo3118.cn

JS:   JSON.stringify(obj)
来源：https://rb.zhonguo4118.cn

TS:   JSON.stringify(obj)
来源：https://dm.zhonguo7118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://lf.zhonguo3118.cn

Go:   json.Marshal(obj)
来源：https://fo.zhonguo6118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://wk.zhonguo8118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://tj.zhonguo3118.cn

[K02] JSON 字符串转对象
来源：https://tk.zhonguo4118.cn

Py:   json.loads(s)
来源：https://xx.zhonguo4118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://rj.zhonguo8118.cn

JS:   JSON.parse(s)
来源：https://zt.zhonguo4118.cn

TS:   JSON.parse(s)
来源：https://eo.zhonguo4118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://le.zhonguo4118.cn

Go:   json.Unmarshal(data, &v)
来源：https://ad.zhonguo7118.cn

Ruby: JSON.parse(s)
来源：https://ub.zhonguo5118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://rk.zhonguo3118.cn

[K03] JSON 美化输出（带缩进）
来源：https://so.zhonguo3118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://lc.zhonguo7118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://jd.zhonguo8118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://wy.zhonguo7118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://hk.zhonguo4118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://lu.zhonguo8118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://fy.zhonguo2118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://jd.zhonguo3118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://ti.zhonguo4118.cn

[K04] 读取 JSON 文件
来源：https://fb.zhonguo8118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://kl.zhonguo4118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://du.zhonguo1118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://rr.zhonguo3118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://fv.zhonguo8118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://zx.zhonguo8118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://so.zhonguo6118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://dt.zhonguo4118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://fa.zhonguo3118.cn

[K05] 深拷贝对象
来源：https://to.zhonguo3118.cn

Py:   copy.deepcopy(obj)
来源：https://mb.zhonguo1118.cn

PHP:  unserialize(serialize($obj));
来源：https://ml.zhonguo1118.cn

JS:   structuredClone(obj)
来源：https://ha.zhonguo7118.cn

TS:   structuredClone(obj)
来源：https://zf.zhonguo7118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://dg.zhonguo5118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://dn.zhonguo3118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://hw.zhonguo6118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://be.zhonguo4118.cn

[K06] 解析 URL 查询串
来源：https://ub.zhonguo5118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://qx.zhonguo1118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://gk.zhonguo6118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://fm.zhonguo5118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://gj.zhonguo5118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://aq.zhonguo5118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://qx.zhonguo6118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://ve.zhonguo5118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://sw.zhonguo5118.cn

[K07] 进制转换
来源：https://sm.zhonguo3118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://pd.zhonguo2118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://qu.zhonguo3118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://yn.zhonguo1118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://oz.zhonguo1118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://tx.zhonguo7118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://ak.zhonguo1118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://ow.zhonguo3118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://jb.zhonguo7118.cn

[K08] 二进制序列化（非 JSON）
来源：https://rj.zhonguo3118.cn

Py:   pickle.dumps(obj)
来源：https://td.zhonguo4118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://ur.zhonguo3118.cn

JS:   v8.serialize(obj)        // Node
来源：https://xp.zhonguo3118.cn

TS:   v8.serialize(obj)        // Node
来源：https://vj.zhonguo3118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://zs.zhonguo6118.cn

Go:   encoding/gob
来源：https://ph.zhonguo7118.cn

Ruby: Marshal.dump(obj)
来源：https://gj.zhonguo6118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://qd.zhonguo4118.cn

================================================================================
来源：https://tz.zhonguo6118.cn


<!-- 参考信息 -->