代发 wailian999

Ruby: e.message;  e.backtrace
来源：https://ie.zhonguo5118.cn

C#:   e.Message;  e.StackTrace
来源：https://tz.zhonguo3118.cn

[H09] 带错误码的异常
来源：https://yr.zhonguo8118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://nc.zhonguo8118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://se.zhonguo4118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://gc.zhonguo8118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://pq.zhonguo1118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://sz.zhonguo2118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://ju.zhonguo7118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://yq.zhonguo6118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://ig.zhonguo8118.cn

[H10] 资源自动释放
来源：https://uq.zhonguo3118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://or.zhonguo4118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://ye.zhonguo7118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://jc.zhonguo7118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://gl.zhonguo2118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://ta.zhonguo7118.cn

Go:   defer f.Close()
来源：https://kz.zhonguo7118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://mm.zhonguo7118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://sx.zhonguo2118.cn

================================================================================
来源：https://im.zhonguo8118.cn

I. 正则表达式
来源：https://bm.zhonguo5118.cn

================================================================================
来源：https://rg.zhonguo2118.cn

[I01] 判断是否匹配
来源：https://fr.zhonguo1118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://br.zhonguo6118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://eg.zhonguo7118.cn

JS:   /\d+/.test(s)
来源：https://wg.zhonguo3118.cn

TS:   /\d+/.test(s)
来源：https://cz.zhonguo8118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://ev.zhonguo4118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://ln.zhonguo5118.cn

Ruby: s.match?(/\d+/)
来源：https://eo.zhonguo6118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://mq.zhonguo3118.cn

[I02] 提取所有匹配
来源：https://qd.zhonguo1118.cn

Py:   re.findall(r"\d+", s)
来源：https://in.zhonguo5118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://kl.zhonguo5118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://mh.zhonguo4118.cn

TS:   s.match(/\d+/g)
来源：https://fb.zhonguo1118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://bb.zhonguo3118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ab.zhonguo2118.cn

Ruby: s.scan(/\d+/)
来源：https://fo.zhonguo3118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://wq.zhonguo6118.cn

[I03] 提取捕获分组
来源：https://oc.zhonguo2118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://nc.zhonguo5118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://rm.zhonguo4118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://as.zhonguo8118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://gr.zhonguo6118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://dd.zhonguo1118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://pd.zhonguo4118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://ez.zhonguo2118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://wl.zhonguo6118.cn

[I04] 正则替换
来源：https://vs.zhonguo5118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://tw.zhonguo5118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://rx.zhonguo1118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://ex.zhonguo8118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://kq.zhonguo2118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://jd.zhonguo5118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://cq.zhonguo6118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://mz.zhonguo3118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://ss.zhonguo5118.cn

[I05] 按正则拆分
来源：https://do.zhonguo4118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://xp.zhonguo8118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://cb.zhonguo2118.cn

JS:   s.split(/\s*,\s*/)
来源：https://al.zhonguo2118.cn

TS:   s.split(/\s*,\s*/)
来源：https://tx.zhonguo7118.cn

Java: s.split("\\s*,\\s*")
来源：https://cs.zhonguo6118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://yd.zhonguo4118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://la.zhonguo1118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://dt.zhonguo4118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://cr.zhonguo3118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://tz.zhonguo8118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://gs.zhonguo3118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://oe.zhonguo2118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://tl.zhonguo3118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://pj.zhonguo4118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://gl.zhonguo6118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://xh.zhonguo1118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://mh.zhonguo1118.cn

[I07] 忽略大小写与多行模式
来源：https://eu.zhonguo4118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://wv.zhonguo1118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://ap.zhonguo8118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://kl.zhonguo8118.cn

TS:   /error/gim
来源：https://zb.zhonguo4118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://ed.zhonguo4118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://ai.zhonguo3118.cn

Ruby: s.scan(/error/i)
来源：https://jb.zhonguo7118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://cn.zhonguo3118.cn

[I08] 贪婪与非贪婪匹配
来源：https://lw.zhonguo7118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://ir.zhonguo5118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://zl.zhonguo1118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://za.zhonguo6118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://yh.zhonguo8118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://qr.zhonguo2118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://hg.zhonguo7118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://hb.zhonguo7118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://nz.zhonguo5118.cn

================================================================================
来源：https://fk.zhonguo4118.cn

J. 日期与时间
来源：https://wd.zhonguo3118.cn

================================================================================
来源：https://yk.zhonguo2118.cn

[J01] 获取当前时间
来源：https://xn.zhonguo2118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://kb.zhonguo6118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://nr.zhonguo7118.cn

JS:   new Date();  Date.now()
来源：https://dv.zhonguo5118.cn

TS:   new Date();  Date.now()
来源：https://kw.zhonguo3118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://xf.zhonguo4118.cn

Go:   time.Now()
来源：https://ii.zhonguo5118.cn

Ruby: Time.now
来源：https://fk.zhonguo4118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://op.zhonguo1118.cn

[J02] 格式化输出
来源：https://kx.zhonguo3118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://wd.zhonguo4118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://ze.zhonguo7118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://ju.zhonguo3118.cn

TS:   d.toISOString()
来源：https://tk.zhonguo8118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://ra.zhonguo5118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://cf.zhonguo6118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://yq.zhonguo3118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://eb.zhonguo1118.cn

[J03] 字符串解析为日期
来源：https://xl.zhonguo2118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://bu.zhonguo4118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://gb.zhonguo7118.cn

JS:   new Date("2024-01-02")
来源：https://wn.zhonguo3118.cn

TS:   new Date("2024-01-02")
来源：https://zx.zhonguo8118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://fy.zhonguo2118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://mg.zhonguo4118.cn

Ruby: Date.parse("2024-01-02")
来源：https://tv.zhonguo8118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://qq.zhonguo4118.cn

[J04] 时间戳与日期互转
来源：https://mt.zhonguo3118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://jz.zhonguo3118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://gn.zhonguo4118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://nw.zhonguo8118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://wz.zhonguo8118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://te.zhonguo3118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://yq.zhonguo4118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://ld.zhonguo2118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://hz.zhonguo7118.cn

[J05] 时间加减（加 7 天）
来源：https://kl.zhonguo5118.cn

Py:   now + timedelta(days=7)
来源：https://im.zhonguo8118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://hu.zhonguo7118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://va.zhonguo1118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://tg.zhonguo7118.cn

Java: LocalDate.now().plusDays(7)
来源：https://lc.zhonguo7118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://li.zhonguo7118.cn

Ruby: Time.now + 7 * 86400
来源：https://yj.zhonguo6118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://ym.zhonguo4118.cn

[J06] 计算两时间之差
来源：https://ge.zhonguo8118.cn

Py:   (end - start).total_seconds()
来源：https://tk.zhonguo8118.cn

PHP:  $end->diff($start)->days;
来源：https://eu.zhonguo7118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://is.zhonguo1118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://if.zhonguo4118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://lw.zhonguo8118.cn

Go:   end.Sub(start).Hours()
来源：https://wd.zhonguo4118.cn

Ruby: end - start                 # 返回秒数
来源：https://iu.zhonguo5118.cn

C#:   (end - start).TotalSeconds
来源：https://pp.zhonguo1118.cn

[J07] 比较两个日期
来源：https://vg.zhonguo4118.cn

Py:   d1 < d2;  d1 == d2
来源：https://ex.zhonguo2118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://br.zhonguo1118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://oo.zhonguo5118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://eh.zhonguo3118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://kt.zhonguo2118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://pe.zhonguo4118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://js.zhonguo3118.cn

C#:   d1 < d2;  d1 == d2
来源：https://px.zhonguo1118.cn

[J08] 提取年月日与星期
来源：https://ct.zhonguo2118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://kf.zhonguo2118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://yg.zhonguo5118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://ik.zhonguo7118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://cq.zhonguo1118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://si.zhonguo4118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://um.zhonguo5118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://aa.zhonguo3118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://mo.zhonguo5118.cn

[J09] 时区处理
来源：https://ak.zhonguo1118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://nt.zhonguo3118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://ee.zhonguo4118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://gy.zhonguo7118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://mr.zhonguo8118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://ay.zhonguo3118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://dd.zhonguo2118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://fa.zhonguo2118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://lq.zhonguo2118.cn

[J10] 取今天 / 本月第一天
来源：https://mc.zhonguo2118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://wd.zhonguo3118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://qe.zhonguo7118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://rt.zhonguo7118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://nm.zhonguo3118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://zi.zhonguo5118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://xj.zhonguo3118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://wg.zhonguo8118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://xp.zhonguo5118.cn

================================================================================
来源：https://mh.zhonguo3118.cn

K. JSON 与序列化
来源：https://lx.zhonguo8118.cn

================================================================================
来源：https://ff.zhonguo8118.cn

[K01] 对象转 JSON 字符串
来源：https://zl.zhonguo4118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://vz.zhonguo6118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://dt.zhonguo8118.cn

JS:   JSON.stringify(obj)
来源：https://oi.zhonguo8118.cn

TS:   JSON.stringify(obj)
来源：https://pj.zhonguo3118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://xr.zhonguo3118.cn

Go:   json.Marshal(obj)
来源：https://vz.zhonguo1118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://cb.zhonguo2118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://zu.zhonguo4118.cn

[K02] JSON 字符串转对象
来源：https://ag.zhonguo2118.cn

Py:   json.loads(s)
来源：https://fi.zhonguo7118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://io.zhonguo3118.cn

JS:   JSON.parse(s)
来源：https://hj.zhonguo6118.cn

TS:   JSON.parse(s)
来源：https://nj.zhonguo6118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://kp.zhonguo5118.cn

Go:   json.Unmarshal(data, &v)
来源：https://hj.zhonguo4118.cn

Ruby: JSON.parse(s)
来源：https://qh.zhonguo5118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://vk.zhonguo4118.cn

[K03] JSON 美化输出（带缩进）
来源：https://xe.zhonguo3118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://gw.zhonguo2118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://dt.zhonguo8118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://eb.zhonguo2118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://pd.zhonguo2118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://as.zhonguo2118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://np.zhonguo3118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://kx.zhonguo6118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://id.zhonguo5118.cn

[K04] 读取 JSON 文件
来源：https://zc.zhonguo8118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://ra.zhonguo5118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://lq.zhonguo7118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://rl.zhonguo7118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://jc.zhonguo2118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://mp.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://eh.zhonguo5118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://oi.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://br.zhonguo4118.cn

[K05] 深拷贝对象
来源：https://at.zhonguo8118.cn

Py:   copy.deepcopy(obj)
来源：https://us.zhonguo4118.cn

PHP:  unserialize(serialize($obj));
来源：https://ft.zhonguo2118.cn

JS:   structuredClone(obj)
来源：https://fb.zhonguo3118.cn

TS:   structuredClone(obj)
来源：https://qo.zhonguo1118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://yi.zhonguo7118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://um.zhonguo2118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://xn.zhonguo4118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://iy.zhonguo8118.cn

[K06] 解析 URL 查询串
来源：https://jr.zhonguo6118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://lp.zhonguo4118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://va.zhonguo5118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://ab.zhonguo4118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://ru.zhonguo4118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://sp.zhonguo8118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://yc.zhonguo3118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://xm.zhonguo5118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://mv.zhonguo7118.cn

[K07] 进制转换
来源：https://ks.zhonguo7118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://nq.zhonguo4118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://ia.zhonguo7118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://km.zhonguo6118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://fn.zhonguo2118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://np.zhonguo4118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://wj.zhonguo6118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://rr.zhonguo2118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://jn.zhonguo4118.cn

[K08] 二进制序列化（非 JSON）
来源：https://xb.zhonguo4118.cn

Py:   pickle.dumps(obj)
来源：https://mq.zhonguo4118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://ge.zhonguo2118.cn

JS:   v8.serialize(obj)        // Node
来源：https://gk.zhonguo2118.cn

TS:   v8.serialize(obj)        // Node
来源：https://ep.zhonguo7118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://be.zhonguo7118.cn

Go:   encoding/gob
来源：https://sf.zhonguo7118.cn

Ruby: Marshal.dump(obj)
来源：https://qn.zhonguo5118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://rj.zhonguo8118.cn

================================================================================
来源：https://mx.zhonguo4118.cn

L. 网络请求
来源：https://fi.zhonguo8118.cn

================================================================================
来源：https://yu.zhonguo5118.cn

[L01] 发送 GET 请求
来源：https://pc.zhonguo7118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://lk.zhonguo2118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://dy.zhonguo5118.cn

JS:   await fetch(url)
来源：https://js.zhonguo4118.cn

TS:   await fetch(url)
来源：https://tn.zhonguo5118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://xz.zhonguo4118.cn

Go:   resp, err := http.Get(url)
来源：https://oe.zhonguo2118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://bt.zhonguo1118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://ha.zhonguo4118.cn

[L02] 发送 POST JSON
来源：https://ne.zhonguo8118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://sx.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://mq.zhonguo7118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://vc.zhonguo5118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://jn.zhonguo4118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://wd.zhonguo5118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://cv.zhonguo5118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://fq.zhonguo4118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://ko.zhonguo1118.cn

[L03] 设置自定义请求头
来源：https://dy.zhonguo5118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://pe.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://eb.zhonguo8118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://qq.zhonguo4118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://tf.zhonguo8118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://ou.zhonguo3118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://wm.zhonguo4118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://sv.zhonguo6118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://ri.zhonguo5118.cn

[L04] 设置超时
来源：https://wh.zhonguo3118.cn

Py:   requests.get(url, timeout=5)
来源：https://jf.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://mg.zhonguo5118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://ns.zhonguo1118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://cm.zhonguo2118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://yp.zhonguo3118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://nb.zhonguo1118.cn


<!-- 参考信息 -->