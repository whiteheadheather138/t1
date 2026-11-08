代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://oz.zhonguo8118.cn

JS:   if (e instanceof TypeError) {}
来源：https://xd.zhonguo1118.cn

TS:   if (e instanceof TypeError) {}
来源：https://ee.zhonguo2118.cn

Java: catch (IOException | SQLException e) {}
来源：https://uy.zhonguo4118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://cs.zhonguo6118.cn

Ruby: rescue ArgumentError => e
来源：https://zm.zhonguo5118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://tl.zhonguo6118.cn

[H06] 可选值 / 空值安全访问
来源：https://pv.zhonguo5118.cn

Py:   value = d.get("k") or default
来源：https://ol.zhonguo2118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://ci.zhonguo2118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://vf.zhonguo6118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://gy.zhonguo1118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://dk.zhonguo5118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://fh.zhonguo6118.cn

Ruby: d&.dig(:a, :b)
来源：https://qv.zhonguo5118.cn

C#:   obj?.A?.B ?? default
来源：https://hk.zhonguo4118.cn

[H07] 断言
来源：https://ui.zhonguo4118.cn

Py:   assert x > 0, "必须为正"
来源：https://gu.zhonguo3118.cn

PHP:  assert($x > 0);
来源：https://kr.zhonguo1118.cn

JS:   console.assert(x > 0);
来源：https://mv.zhonguo2118.cn

TS:   console.assert(x > 0);
来源：https://og.zhonguo7118.cn

Java: assert x > 0 : "必须为正";
来源：https://tq.zhonguo3118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://gv.zhonguo8118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://ut.zhonguo2118.cn

C#:   Debug.Assert(x > 0);
来源：https://ou.zhonguo4118.cn

[H08] 获取错误信息与堆栈
来源：https://ep.zhonguo5118.cn

Py:   str(e);  traceback.format_exc()
来源：https://yz.zhonguo3118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://st.zhonguo3118.cn

JS:   e.message;  e.stack
来源：https://po.zhonguo8118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://ta.zhonguo3118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://wq.zhonguo4118.cn

Go:   err.Error()
来源：https://ys.zhonguo6118.cn

Ruby: e.message;  e.backtrace
来源：https://nw.zhonguo1118.cn

C#:   e.Message;  e.StackTrace
来源：https://ug.zhonguo6118.cn

[H09] 带错误码的异常
来源：https://zp.zhonguo1118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://rw.zhonguo8118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://wh.zhonguo8118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://ba.zhonguo5118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://hf.zhonguo5118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://op.zhonguo1118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://jw.zhonguo3118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://em.zhonguo2118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://mg.zhonguo2118.cn

[H10] 资源自动释放
来源：https://rm.zhonguo2118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://is.zhonguo8118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://ni.zhonguo1118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://fr.zhonguo5118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://mf.zhonguo6118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://as.zhonguo4118.cn

Go:   defer f.Close()
来源：https://at.zhonguo6118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://xg.zhonguo8118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://vn.zhonguo5118.cn

================================================================================
来源：https://mf.zhonguo1118.cn

I. 正则表达式
来源：https://ph.zhonguo3118.cn

================================================================================
来源：https://pv.zhonguo1118.cn

[I01] 判断是否匹配
来源：https://db.zhonguo6118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://gf.zhonguo3118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://bm.zhonguo5118.cn

JS:   /\d+/.test(s)
来源：https://yc.zhonguo8118.cn

TS:   /\d+/.test(s)
来源：https://kr.zhonguo5118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://uv.zhonguo4118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://ws.zhonguo1118.cn

Ruby: s.match?(/\d+/)
来源：https://iw.zhonguo5118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://gp.zhonguo8118.cn

[I02] 提取所有匹配
来源：https://hu.zhonguo6118.cn

Py:   re.findall(r"\d+", s)
来源：https://qf.zhonguo5118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://cv.zhonguo1118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://jm.zhonguo3118.cn

TS:   s.match(/\d+/g)
来源：https://ju.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://ya.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://sn.zhonguo2118.cn

Ruby: s.scan(/\d+/)
来源：https://is.zhonguo6118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://hq.zhonguo5118.cn

[I03] 提取捕获分组
来源：https://ux.zhonguo5118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://mr.zhonguo3118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://br.zhonguo8118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://cn.zhonguo2118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://mi.zhonguo7118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://ik.zhonguo7118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://rt.zhonguo4118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://av.zhonguo1118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://ms.zhonguo7118.cn

[I04] 正则替换
来源：https://ax.zhonguo1118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://an.zhonguo1118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://qr.zhonguo4118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://qg.zhonguo4118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://xv.zhonguo3118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://dz.zhonguo3118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://hx.zhonguo2118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://ce.zhonguo1118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://qj.zhonguo6118.cn

[I05] 按正则拆分
来源：https://la.zhonguo5118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://dy.zhonguo2118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://je.zhonguo3118.cn

JS:   s.split(/\s*,\s*/)
来源：https://zy.zhonguo1118.cn

TS:   s.split(/\s*,\s*/)
来源：https://sv.zhonguo4118.cn

Java: s.split("\\s*,\\s*")
来源：https://fy.zhonguo1118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://ve.zhonguo3118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://gr.zhonguo7118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://ne.zhonguo8118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://pd.zhonguo1118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://ye.zhonguo5118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://wh.zhonguo4118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://ja.zhonguo8118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://bk.zhonguo5118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://cq.zhonguo4118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://ef.zhonguo3118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://de.zhonguo5118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://fv.zhonguo6118.cn

[I07] 忽略大小写与多行模式
来源：https://eh.zhonguo5118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://av.zhonguo6118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://fu.zhonguo2118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://ww.zhonguo1118.cn

TS:   /error/gim
来源：https://pz.zhonguo7118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://sx.zhonguo3118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://bk.zhonguo1118.cn

Ruby: s.scan(/error/i)
来源：https://up.zhonguo2118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://tt.zhonguo8118.cn

[I08] 贪婪与非贪婪匹配
来源：https://iw.zhonguo5118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://gr.zhonguo2118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://tz.zhonguo7118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://rv.zhonguo5118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://el.zhonguo3118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://pw.zhonguo3118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://lw.zhonguo4118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://sk.zhonguo1118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://zo.zhonguo8118.cn

================================================================================
来源：https://av.zhonguo5118.cn

J. 日期与时间
来源：https://jz.zhonguo8118.cn

================================================================================
来源：https://bn.zhonguo4118.cn

[J01] 获取当前时间
来源：https://jr.zhonguo6118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://su.zhonguo7118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://ih.zhonguo2118.cn

JS:   new Date();  Date.now()
来源：https://ct.zhonguo7118.cn

TS:   new Date();  Date.now()
来源：https://gf.zhonguo7118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://vp.zhonguo4118.cn

Go:   time.Now()
来源：https://rh.zhonguo5118.cn

Ruby: Time.now
来源：https://uv.zhonguo1118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://df.zhonguo2118.cn

[J02] 格式化输出
来源：https://ir.zhonguo7118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://it.zhonguo5118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://so.zhonguo2118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://hk.zhonguo1118.cn

TS:   d.toISOString()
来源：https://na.zhonguo2118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://gg.zhonguo4118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://bh.zhonguo4118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://qt.zhonguo1118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://er.zhonguo1118.cn

[J03] 字符串解析为日期
来源：https://xd.zhonguo7118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://fq.zhonguo4118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://du.zhonguo4118.cn

JS:   new Date("2024-01-02")
来源：https://kz.zhonguo5118.cn

TS:   new Date("2024-01-02")
来源：https://zs.zhonguo7118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://tr.zhonguo5118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://cg.zhonguo7118.cn

Ruby: Date.parse("2024-01-02")
来源：https://re.zhonguo8118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://bz.zhonguo3118.cn

[J04] 时间戳与日期互转
来源：https://nc.zhonguo5118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://oy.zhonguo3118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://xq.zhonguo1118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://vr.zhonguo5118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://vz.zhonguo6118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://jj.zhonguo6118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://lj.zhonguo3118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://rs.zhonguo4118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://oj.zhonguo5118.cn

[J05] 时间加减（加 7 天）
来源：https://ne.zhonguo6118.cn

Py:   now + timedelta(days=7)
来源：https://xy.zhonguo5118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://yt.zhonguo3118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://js.zhonguo8118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://dn.zhonguo2118.cn

Java: LocalDate.now().plusDays(7)
来源：https://en.zhonguo2118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://bd.zhonguo8118.cn

Ruby: Time.now + 7 * 86400
来源：https://ro.zhonguo5118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://xf.zhonguo8118.cn

[J06] 计算两时间之差
来源：https://en.zhonguo8118.cn

Py:   (end - start).total_seconds()
来源：https://wn.zhonguo2118.cn

PHP:  $end->diff($start)->days;
来源：https://zq.zhonguo4118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://mq.zhonguo6118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://as.zhonguo3118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://qn.zhonguo7118.cn

Go:   end.Sub(start).Hours()
来源：https://et.zhonguo8118.cn

Ruby: end - start                 # 返回秒数
来源：https://rj.zhonguo7118.cn

C#:   (end - start).TotalSeconds
来源：https://rd.zhonguo6118.cn

[J07] 比较两个日期
来源：https://pg.zhonguo5118.cn

Py:   d1 < d2;  d1 == d2
来源：https://up.zhonguo7118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://ep.zhonguo7118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://wp.zhonguo7118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://ac.zhonguo1118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://bb.zhonguo1118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://se.zhonguo3118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://vy.zhonguo3118.cn

C#:   d1 < d2;  d1 == d2
来源：https://xf.zhonguo5118.cn

[J08] 提取年月日与星期
来源：https://ak.zhonguo6118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://bb.zhonguo8118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://jx.zhonguo2118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://zk.zhonguo8118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://oj.zhonguo4118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://wq.zhonguo5118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://iz.zhonguo4118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://jr.zhonguo7118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://jf.zhonguo2118.cn

[J09] 时区处理
来源：https://ky.zhonguo4118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://zw.zhonguo1118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://kx.zhonguo3118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://cy.zhonguo6118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://ml.zhonguo3118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://nz.zhonguo4118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://hb.zhonguo2118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://xa.zhonguo8118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://na.zhonguo1118.cn

[J10] 取今天 / 本月第一天
来源：https://zr.zhonguo1118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://ou.zhonguo7118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://xr.zhonguo8118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://nc.zhonguo6118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://wu.zhonguo4118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://qb.zhonguo6118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://vg.zhonguo1118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://js.zhonguo5118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://hh.zhonguo1118.cn

================================================================================
来源：https://nv.zhonguo6118.cn

K. JSON 与序列化
来源：https://ik.zhonguo7118.cn

================================================================================
来源：https://za.zhonguo7118.cn

[K01] 对象转 JSON 字符串
来源：https://mn.zhonguo3118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://zn.zhonguo7118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://ah.zhonguo4118.cn

JS:   JSON.stringify(obj)
来源：https://yg.zhonguo4118.cn

TS:   JSON.stringify(obj)
来源：https://fw.zhonguo8118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://iu.zhonguo6118.cn

Go:   json.Marshal(obj)
来源：https://bv.zhonguo8118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://if.zhonguo6118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://rg.zhonguo3118.cn

[K02] JSON 字符串转对象
来源：https://dk.zhonguo6118.cn

Py:   json.loads(s)
来源：https://ik.zhonguo1118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://nt.zhonguo7118.cn

JS:   JSON.parse(s)
来源：https://dt.zhonguo7118.cn

TS:   JSON.parse(s)
来源：https://wt.zhonguo8118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://hz.zhonguo7118.cn

Go:   json.Unmarshal(data, &v)
来源：https://nz.zhonguo8118.cn

Ruby: JSON.parse(s)
来源：https://ls.zhonguo8118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://du.zhonguo4118.cn

[K03] JSON 美化输出（带缩进）
来源：https://gv.zhonguo6118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://yt.zhonguo6118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://xx.zhonguo5118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://wy.zhonguo4118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://oq.zhonguo4118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://wm.zhonguo5118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://at.zhonguo8118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://kj.zhonguo3118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://xt.zhonguo8118.cn

[K04] 读取 JSON 文件
来源：https://od.zhonguo4118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://cx.zhonguo5118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://fk.zhonguo8118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://uj.zhonguo4118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ve.zhonguo5118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://nv.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://af.zhonguo6118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://ws.zhonguo4118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://nb.zhonguo4118.cn

[K05] 深拷贝对象
来源：https://va.zhonguo7118.cn

Py:   copy.deepcopy(obj)
来源：https://jo.zhonguo4118.cn

PHP:  unserialize(serialize($obj));
来源：https://qq.zhonguo1118.cn

JS:   structuredClone(obj)
来源：https://xp.zhonguo5118.cn

TS:   structuredClone(obj)
来源：https://tx.zhonguo8118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://xx.zhonguo3118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://ei.zhonguo2118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://mc.zhonguo5118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://ym.zhonguo7118.cn

[K06] 解析 URL 查询串
来源：https://xo.zhonguo4118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://mx.zhonguo5118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://xz.zhonguo3118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://ii.zhonguo7118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://nu.zhonguo6118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://wk.zhonguo5118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://qb.zhonguo4118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://mi.zhonguo3118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://gm.zhonguo7118.cn

[K07] 进制转换
来源：https://jp.zhonguo8118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://df.zhonguo3118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://hk.zhonguo5118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://yb.zhonguo7118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://xk.zhonguo6118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://tb.zhonguo1118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://mi.zhonguo4118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://zv.zhonguo7118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://fe.zhonguo7118.cn

[K08] 二进制序列化（非 JSON）
来源：https://gf.zhonguo1118.cn

Py:   pickle.dumps(obj)
来源：https://oy.zhonguo7118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://vf.zhonguo6118.cn

JS:   v8.serialize(obj)        // Node
来源：https://iw.zhonguo8118.cn

TS:   v8.serialize(obj)        // Node
来源：https://dg.zhonguo4118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://da.zhonguo4118.cn

Go:   encoding/gob
来源：https://ny.zhonguo7118.cn

Ruby: Marshal.dump(obj)
来源：https://fr.zhonguo5118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://rx.zhonguo6118.cn

================================================================================
来源：https://vu.zhonguo3118.cn

L. 网络请求
来源：https://ox.zhonguo5118.cn

================================================================================
来源：https://cm.zhonguo4118.cn

[L01] 发送 GET 请求
来源：https://cy.zhonguo7118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://wk.zhonguo3118.cn


<!-- 参考信息 -->