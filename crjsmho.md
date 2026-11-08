代发 wailian999

TS:   console.assert(x > 0);
来源：https://bf.zhonguo2118.cn

Java: assert x > 0 : "必须为正";
来源：https://oj.zhonguo8118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://ch.zhonguo3118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://xg.zhonguo8118.cn

C#:   Debug.Assert(x > 0);
来源：https://qy.zhonguo2118.cn

[H08] 获取错误信息与堆栈
来源：https://px.zhonguo4118.cn

Py:   str(e);  traceback.format_exc()
来源：https://wj.zhonguo4118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://wr.zhonguo1118.cn

JS:   e.message;  e.stack
来源：https://yt.zhonguo3118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://pl.zhonguo6118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://zf.zhonguo3118.cn

Go:   err.Error()
来源：https://ck.zhonguo6118.cn

Ruby: e.message;  e.backtrace
来源：https://oz.zhonguo2118.cn

C#:   e.Message;  e.StackTrace
来源：https://zi.zhonguo8118.cn

[H09] 带错误码的异常
来源：https://vb.zhonguo2118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://kb.zhonguo7118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://wb.zhonguo3118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://kz.zhonguo6118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://kd.zhonguo8118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://di.zhonguo5118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://ca.zhonguo6118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://ph.zhonguo8118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://ts.zhonguo1118.cn

[H10] 资源自动释放
来源：https://bk.zhonguo2118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://ey.zhonguo1118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://tl.zhonguo8118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://iw.zhonguo7118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://ru.zhonguo1118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://uf.zhonguo7118.cn

Go:   defer f.Close()
来源：https://xl.zhonguo8118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://ct.zhonguo8118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://sm.zhonguo5118.cn

================================================================================
来源：https://vo.zhonguo4118.cn

I. 正则表达式
来源：https://mq.zhonguo7118.cn

================================================================================
来源：https://za.zhonguo8118.cn

[I01] 判断是否匹配
来源：https://ku.zhonguo4118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://ef.zhonguo3118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://zp.zhonguo7118.cn

JS:   /\d+/.test(s)
来源：https://tt.zhonguo4118.cn

TS:   /\d+/.test(s)
来源：https://rk.zhonguo5118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://lx.zhonguo1118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://zm.zhonguo6118.cn

Ruby: s.match?(/\d+/)
来源：https://gl.zhonguo6118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://cg.zhonguo1118.cn

[I02] 提取所有匹配
来源：https://kz.zhonguo7118.cn

Py:   re.findall(r"\d+", s)
来源：https://xo.zhonguo8118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://pd.zhonguo2118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://ic.zhonguo8118.cn

TS:   s.match(/\d+/g)
来源：https://yp.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://fj.zhonguo2118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://qr.zhonguo2118.cn

Ruby: s.scan(/\d+/)
来源：https://bf.zhonguo6118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://vl.zhonguo8118.cn

[I03] 提取捕获分组
来源：https://mv.zhonguo7118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://xk.zhonguo2118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://ei.zhonguo1118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://ar.zhonguo2118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://qe.zhonguo7118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://tj.zhonguo8118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://zx.zhonguo2118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://aa.zhonguo1118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://ge.zhonguo2118.cn

[I04] 正则替换
来源：https://eo.zhonguo2118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://ds.zhonguo1118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://vj.zhonguo2118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://mv.zhonguo2118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://wh.zhonguo7118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://ot.zhonguo2118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://sk.zhonguo6118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://il.zhonguo4118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://zi.zhonguo5118.cn

[I05] 按正则拆分
来源：https://ts.zhonguo6118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://yp.zhonguo2118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://au.zhonguo5118.cn

JS:   s.split(/\s*,\s*/)
来源：https://uc.zhonguo2118.cn

TS:   s.split(/\s*,\s*/)
来源：https://tv.zhonguo3118.cn

Java: s.split("\\s*,\\s*")
来源：https://no.zhonguo1118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://mu.zhonguo2118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://gp.zhonguo3118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://sc.zhonguo3118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://ne.zhonguo6118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://fr.zhonguo1118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://fg.zhonguo4118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://zn.zhonguo3118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://uo.zhonguo2118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://tk.zhonguo3118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://hs.zhonguo8118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://ld.zhonguo6118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://cw.zhonguo2118.cn

[I07] 忽略大小写与多行模式
来源：https://ri.zhonguo8118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://dg.zhonguo6118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://fr.zhonguo2118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://fl.zhonguo3118.cn

TS:   /error/gim
来源：https://rd.zhonguo1118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://ru.zhonguo4118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://md.zhonguo1118.cn

Ruby: s.scan(/error/i)
来源：https://cv.zhonguo8118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://oc.zhonguo8118.cn

[I08] 贪婪与非贪婪匹配
来源：https://gl.zhonguo4118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://ba.zhonguo3118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://mq.zhonguo2118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://ia.zhonguo6118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://fm.zhonguo7118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://av.zhonguo5118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://bf.zhonguo2118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://xn.zhonguo7118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://mu.zhonguo4118.cn

================================================================================
来源：https://ge.zhonguo5118.cn

J. 日期与时间
来源：https://ts.zhonguo6118.cn

================================================================================
来源：https://ef.zhonguo8118.cn

[J01] 获取当前时间
来源：https://qg.zhonguo6118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://fw.zhonguo5118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://zc.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://pv.zhonguo6118.cn

TS:   new Date();  Date.now()
来源：https://ak.zhonguo2118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://ja.zhonguo7118.cn

Go:   time.Now()
来源：https://oa.zhonguo1118.cn

Ruby: Time.now
来源：https://qz.zhonguo1118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://zz.zhonguo2118.cn

[J02] 格式化输出
来源：https://kj.zhonguo1118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://ji.zhonguo4118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://zj.zhonguo1118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://ga.zhonguo1118.cn

TS:   d.toISOString()
来源：https://ee.zhonguo1118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://ek.zhonguo2118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://ql.zhonguo3118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://kh.zhonguo6118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://cn.zhonguo2118.cn

[J03] 字符串解析为日期
来源：https://tr.zhonguo7118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://jd.zhonguo4118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://mn.zhonguo8118.cn

JS:   new Date("2024-01-02")
来源：https://sb.zhonguo7118.cn

TS:   new Date("2024-01-02")
来源：https://bs.zhonguo8118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://wf.zhonguo6118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://ej.zhonguo1118.cn

Ruby: Date.parse("2024-01-02")
来源：https://ym.zhonguo1118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://tj.zhonguo5118.cn

[J04] 时间戳与日期互转
来源：https://ku.zhonguo5118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://is.zhonguo3118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://ol.zhonguo1118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://gd.zhonguo1118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://aa.zhonguo4118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://sm.zhonguo2118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://hu.zhonguo6118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://bn.zhonguo1118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://ih.zhonguo6118.cn

[J05] 时间加减（加 7 天）
来源：https://cg.zhonguo1118.cn

Py:   now + timedelta(days=7)
来源：https://pg.zhonguo4118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://qa.zhonguo7118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://ps.zhonguo8118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://mn.zhonguo7118.cn

Java: LocalDate.now().plusDays(7)
来源：https://dx.zhonguo4118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://jq.zhonguo5118.cn

Ruby: Time.now + 7 * 86400
来源：https://rg.zhonguo8118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://yq.zhonguo2118.cn

[J06] 计算两时间之差
来源：https://ss.zhonguo2118.cn

Py:   (end - start).total_seconds()
来源：https://qs.zhonguo2118.cn

PHP:  $end->diff($start)->days;
来源：https://oe.zhonguo8118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://lb.zhonguo4118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://ti.zhonguo7118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://xj.zhonguo2118.cn

Go:   end.Sub(start).Hours()
来源：https://db.zhonguo8118.cn

Ruby: end - start                 # 返回秒数
来源：https://us.zhonguo2118.cn

C#:   (end - start).TotalSeconds
来源：https://ys.zhonguo6118.cn

[J07] 比较两个日期
来源：https://da.zhonguo6118.cn

Py:   d1 < d2;  d1 == d2
来源：https://bu.zhonguo3118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://fe.zhonguo2118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://qa.zhonguo7118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://am.zhonguo8118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://nk.zhonguo2118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://wi.zhonguo3118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://we.zhonguo4118.cn

C#:   d1 < d2;  d1 == d2
来源：https://cu.zhonguo1118.cn

[J08] 提取年月日与星期
来源：https://od.zhonguo5118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://qo.zhonguo7118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://ny.zhonguo8118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://iw.zhonguo5118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://ju.zhonguo1118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://el.zhonguo5118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://nl.zhonguo2118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://ep.zhonguo3118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://cf.zhonguo7118.cn

[J09] 时区处理
来源：https://ur.zhonguo5118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://xq.zhonguo4118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://vz.zhonguo5118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://tj.zhonguo8118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://tj.zhonguo4118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://cb.zhonguo5118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://dx.zhonguo1118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://ut.zhonguo7118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://wd.zhonguo6118.cn

[J10] 取今天 / 本月第一天
来源：https://td.zhonguo1118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://at.zhonguo2118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://im.zhonguo1118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://dh.zhonguo4118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://xf.zhonguo7118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://uy.zhonguo2118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://va.zhonguo2118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://ur.zhonguo3118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://qa.zhonguo5118.cn

================================================================================
来源：https://ws.zhonguo2118.cn

K. JSON 与序列化
来源：https://ob.zhonguo4118.cn

================================================================================
来源：https://rk.zhonguo8118.cn

[K01] 对象转 JSON 字符串
来源：https://dv.zhonguo8118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://vr.zhonguo7118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://tr.zhonguo7118.cn

JS:   JSON.stringify(obj)
来源：https://ur.zhonguo4118.cn

TS:   JSON.stringify(obj)
来源：https://pw.zhonguo8118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://oo.zhonguo6118.cn

Go:   json.Marshal(obj)
来源：https://yd.zhonguo1118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://qr.zhonguo5118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://zi.zhonguo7118.cn

[K02] JSON 字符串转对象
来源：https://yn.zhonguo5118.cn

Py:   json.loads(s)
来源：https://tf.zhonguo8118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://md.zhonguo3118.cn

JS:   JSON.parse(s)
来源：https://ak.zhonguo8118.cn

TS:   JSON.parse(s)
来源：https://bm.zhonguo5118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://er.zhonguo4118.cn

Go:   json.Unmarshal(data, &v)
来源：https://vx.zhonguo1118.cn

Ruby: JSON.parse(s)
来源：https://xy.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://ua.zhonguo5118.cn

[K03] JSON 美化输出（带缩进）
来源：https://gd.zhonguo8118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://up.zhonguo6118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://ek.zhonguo6118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://gy.zhonguo8118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://gl.zhonguo5118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://wt.zhonguo4118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://lj.zhonguo1118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://bz.zhonguo6118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://uu.zhonguo3118.cn

[K04] 读取 JSON 文件
来源：https://fe.zhonguo4118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://hz.zhonguo6118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://yz.zhonguo4118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ys.zhonguo3118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://pp.zhonguo4118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://iy.zhonguo3118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://zf.zhonguo8118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://bw.zhonguo3118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://ud.zhonguo1118.cn

[K05] 深拷贝对象
来源：https://bx.zhonguo5118.cn

Py:   copy.deepcopy(obj)
来源：https://ws.zhonguo6118.cn

PHP:  unserialize(serialize($obj));
来源：https://wp.zhonguo4118.cn

JS:   structuredClone(obj)
来源：https://iy.zhonguo5118.cn

TS:   structuredClone(obj)
来源：https://ke.zhonguo4118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://ta.zhonguo5118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://zt.zhonguo1118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://zs.zhonguo7118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://xk.zhonguo3118.cn

[K06] 解析 URL 查询串
来源：https://az.zhonguo5118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://ny.zhonguo1118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://tv.zhonguo3118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://xf.zhonguo8118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://by.zhonguo3118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://wh.zhonguo7118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://cw.zhonguo3118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://yf.zhonguo2118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://ad.zhonguo6118.cn

[K07] 进制转换
来源：https://am.zhonguo6118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://aw.zhonguo1118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://bn.zhonguo3118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://zo.zhonguo4118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://zp.zhonguo1118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://qv.zhonguo6118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://ra.zhonguo8118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://pt.zhonguo1118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://ho.zhonguo6118.cn

[K08] 二进制序列化（非 JSON）
来源：https://at.zhonguo6118.cn

Py:   pickle.dumps(obj)
来源：https://yg.zhonguo4118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://kv.zhonguo2118.cn

JS:   v8.serialize(obj)        // Node
来源：https://kb.zhonguo8118.cn

TS:   v8.serialize(obj)        // Node
来源：https://dw.zhonguo8118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://od.zhonguo5118.cn

Go:   encoding/gob
来源：https://xr.zhonguo6118.cn

Ruby: Marshal.dump(obj)
来源：https://tj.zhonguo1118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://gh.zhonguo2118.cn

================================================================================
来源：https://vs.zhonguo2118.cn

L. 网络请求
来源：https://ec.zhonguo8118.cn

================================================================================
来源：https://ia.zhonguo5118.cn

[L01] 发送 GET 请求
来源：https://rf.zhonguo8118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://uo.zhonguo7118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://dn.zhonguo3118.cn

JS:   await fetch(url)
来源：https://gi.zhonguo2118.cn

TS:   await fetch(url)
来源：https://ez.zhonguo2118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://gw.zhonguo5118.cn

Go:   resp, err := http.Get(url)
来源：https://ho.zhonguo6118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://hd.zhonguo2118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://wg.zhonguo6118.cn

[L02] 发送 POST JSON
来源：https://wv.zhonguo6118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://uv.zhonguo4118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://pc.zhonguo3118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://ke.zhonguo2118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://pk.zhonguo2118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://cd.zhonguo8118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://oe.zhonguo2118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://ox.zhonguo5118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://yz.zhonguo4118.cn

[L03] 设置自定义请求头
来源：https://aq.zhonguo1118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://lx.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://nh.zhonguo6118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://re.zhonguo7118.cn


<!-- 参考信息 -->