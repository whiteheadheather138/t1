代发 wailian999

C#:   Debug.Assert(x > 0);
来源：https://nm.zhonguo7118.cn

[H08] 获取错误信息与堆栈
来源：https://gp.zhonguo2118.cn

Py:   str(e);  traceback.format_exc()
来源：https://dp.zhonguo6118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://ob.zhonguo2118.cn

JS:   e.message;  e.stack
来源：https://ko.zhonguo8118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://xn.zhonguo8118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://gm.zhonguo6118.cn

Go:   err.Error()
来源：https://jd.zhonguo6118.cn

Ruby: e.message;  e.backtrace
来源：https://bb.zhonguo1118.cn

C#:   e.Message;  e.StackTrace
来源：https://zp.zhonguo2118.cn

[H09] 带错误码的异常
来源：https://us.zhonguo1118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://zn.zhonguo7118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://au.zhonguo1118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://hv.zhonguo8118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://jq.zhonguo3118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://im.zhonguo1118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://tx.zhonguo6118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://ve.zhonguo2118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://ju.zhonguo8118.cn

[H10] 资源自动释放
来源：https://dw.zhonguo8118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://cw.zhonguo4118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://kb.zhonguo6118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://mh.zhonguo4118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://ve.zhonguo3118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://uy.zhonguo1118.cn

Go:   defer f.Close()
来源：https://ns.zhonguo6118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://oi.zhonguo1118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://yq.zhonguo8118.cn

================================================================================
来源：https://gm.zhonguo8118.cn

I. 正则表达式
来源：https://lf.zhonguo8118.cn

================================================================================
来源：https://ei.zhonguo5118.cn

[I01] 判断是否匹配
来源：https://pm.zhonguo3118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://kc.zhonguo1118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://ki.zhonguo3118.cn

JS:   /\d+/.test(s)
来源：https://zl.zhonguo5118.cn

TS:   /\d+/.test(s)
来源：https://qq.zhonguo7118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://aq.zhonguo1118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://cb.zhonguo3118.cn

Ruby: s.match?(/\d+/)
来源：https://ex.zhonguo3118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://wj.zhonguo2118.cn

[I02] 提取所有匹配
来源：https://wt.zhonguo7118.cn

Py:   re.findall(r"\d+", s)
来源：https://pl.zhonguo2118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://ml.zhonguo5118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://ko.zhonguo2118.cn

TS:   s.match(/\d+/g)
来源：https://ab.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://la.zhonguo7118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ew.zhonguo5118.cn

Ruby: s.scan(/\d+/)
来源：https://gk.zhonguo6118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://jz.zhonguo5118.cn

[I03] 提取捕获分组
来源：https://mf.zhonguo8118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://nc.zhonguo8118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://gq.zhonguo1118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://ee.zhonguo2118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://xd.zhonguo6118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://se.zhonguo2118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://io.zhonguo5118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://ba.zhonguo4118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://fc.zhonguo2118.cn

[I04] 正则替换
来源：https://aq.zhonguo8118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://jq.zhonguo8118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://yu.zhonguo2118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://jy.zhonguo8118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://bh.zhonguo6118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://xa.zhonguo2118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://gk.zhonguo5118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://um.zhonguo8118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://dg.zhonguo4118.cn

[I05] 按正则拆分
来源：https://sb.zhonguo6118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://dg.zhonguo3118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://wb.zhonguo3118.cn

JS:   s.split(/\s*,\s*/)
来源：https://zq.zhonguo1118.cn

TS:   s.split(/\s*,\s*/)
来源：https://uk.zhonguo8118.cn

Java: s.split("\\s*,\\s*")
来源：https://qz.zhonguo3118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://yy.zhonguo4118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://ms.zhonguo2118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://cy.zhonguo6118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://sz.zhonguo2118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://ta.zhonguo8118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://ik.zhonguo2118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://zg.zhonguo3118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://sn.zhonguo4118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://kh.zhonguo8118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://nt.zhonguo8118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://cg.zhonguo3118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://dc.zhonguo5118.cn

[I07] 忽略大小写与多行模式
来源：https://ss.zhonguo8118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://jq.zhonguo7118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://es.zhonguo7118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://bx.zhonguo7118.cn

TS:   /error/gim
来源：https://ic.zhonguo2118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://dd.zhonguo1118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://ip.zhonguo2118.cn

Ruby: s.scan(/error/i)
来源：https://ev.zhonguo3118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://hq.zhonguo8118.cn

[I08] 贪婪与非贪婪匹配
来源：https://yq.zhonguo7118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://pg.zhonguo8118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://nk.zhonguo2118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://qn.zhonguo5118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://dl.zhonguo1118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://ct.zhonguo5118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://ty.zhonguo1118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://zu.zhonguo7118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://sj.zhonguo3118.cn

================================================================================
来源：https://bw.zhonguo3118.cn

J. 日期与时间
来源：https://kp.zhonguo6118.cn

================================================================================
来源：https://yo.zhonguo6118.cn

[J01] 获取当前时间
来源：https://mq.zhonguo8118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://vi.zhonguo4118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://ow.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://cq.zhonguo2118.cn

TS:   new Date();  Date.now()
来源：https://jf.zhonguo8118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://js.zhonguo1118.cn

Go:   time.Now()
来源：https://lu.zhonguo8118.cn

Ruby: Time.now
来源：https://wt.zhonguo4118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://al.zhonguo2118.cn

[J02] 格式化输出
来源：https://li.zhonguo1118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://of.zhonguo7118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://eb.zhonguo6118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://yl.zhonguo6118.cn

TS:   d.toISOString()
来源：https://hb.zhonguo4118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://mp.zhonguo8118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://ta.zhonguo3118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://je.zhonguo4118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://nb.zhonguo6118.cn

[J03] 字符串解析为日期
来源：https://oa.zhonguo6118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://dh.zhonguo6118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://rp.zhonguo7118.cn

JS:   new Date("2024-01-02")
来源：https://ks.zhonguo2118.cn

TS:   new Date("2024-01-02")
来源：https://tc.zhonguo6118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://lx.zhonguo3118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://iy.zhonguo7118.cn

Ruby: Date.parse("2024-01-02")
来源：https://mz.zhonguo5118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://rk.zhonguo8118.cn

[J04] 时间戳与日期互转
来源：https://pe.zhonguo6118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://vp.zhonguo7118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://mb.zhonguo1118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://xs.zhonguo1118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://lo.zhonguo1118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://gl.zhonguo3118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://dz.zhonguo6118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://gb.zhonguo2118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://pc.zhonguo2118.cn

[J05] 时间加减（加 7 天）
来源：https://ou.zhonguo2118.cn

Py:   now + timedelta(days=7)
来源：https://du.zhonguo4118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://yg.zhonguo3118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://sx.zhonguo8118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://xg.zhonguo4118.cn

Java: LocalDate.now().plusDays(7)
来源：https://su.zhonguo2118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://oj.zhonguo4118.cn

Ruby: Time.now + 7 * 86400
来源：https://bq.zhonguo6118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://nn.zhonguo5118.cn

[J06] 计算两时间之差
来源：https://li.zhonguo3118.cn

Py:   (end - start).total_seconds()
来源：https://kl.zhonguo8118.cn

PHP:  $end->diff($start)->days;
来源：https://dz.zhonguo8118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://vo.zhonguo7118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://xa.zhonguo8118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://oq.zhonguo1118.cn

Go:   end.Sub(start).Hours()
来源：https://ox.zhonguo3118.cn

Ruby: end - start                 # 返回秒数
来源：https://wt.zhonguo5118.cn

C#:   (end - start).TotalSeconds
来源：https://on.zhonguo6118.cn

[J07] 比较两个日期
来源：https://hs.zhonguo8118.cn

Py:   d1 < d2;  d1 == d2
来源：https://dy.zhonguo6118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://oq.zhonguo8118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://ug.zhonguo5118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://af.zhonguo6118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://yn.zhonguo4118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://kz.zhonguo7118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://mi.zhonguo8118.cn

C#:   d1 < d2;  d1 == d2
来源：https://fo.zhonguo4118.cn

[J08] 提取年月日与星期
来源：https://im.zhonguo3118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://ln.zhonguo3118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://ax.zhonguo4118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://aj.zhonguo2118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://yb.zhonguo7118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://mj.zhonguo4118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://el.zhonguo8118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://xz.zhonguo8118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://of.zhonguo3118.cn

[J09] 时区处理
来源：https://ss.zhonguo3118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://pw.zhonguo5118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://wz.zhonguo8118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://xv.zhonguo1118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://ch.zhonguo3118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://pv.zhonguo8118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://ak.zhonguo4118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://ae.zhonguo7118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://yi.zhonguo3118.cn

[J10] 取今天 / 本月第一天
来源：https://ft.zhonguo6118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://ap.zhonguo5118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://zn.zhonguo2118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://cg.zhonguo8118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://ke.zhonguo6118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://uk.zhonguo7118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://ew.zhonguo2118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://hc.zhonguo4118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://au.zhonguo3118.cn

================================================================================
来源：https://oq.zhonguo8118.cn

K. JSON 与序列化
来源：https://rm.zhonguo7118.cn

================================================================================
来源：https://pw.zhonguo2118.cn

[K01] 对象转 JSON 字符串
来源：https://hp.zhonguo6118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://fs.zhonguo4118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://qt.zhonguo2118.cn

JS:   JSON.stringify(obj)
来源：https://gt.zhonguo2118.cn

TS:   JSON.stringify(obj)
来源：https://vh.zhonguo1118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://gy.zhonguo1118.cn

Go:   json.Marshal(obj)
来源：https://dz.zhonguo5118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://cf.zhonguo2118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://jb.zhonguo5118.cn

[K02] JSON 字符串转对象
来源：https://ln.zhonguo6118.cn

Py:   json.loads(s)
来源：https://md.zhonguo4118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://ys.zhonguo6118.cn

JS:   JSON.parse(s)
来源：https://ik.zhonguo3118.cn

TS:   JSON.parse(s)
来源：https://og.zhonguo6118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://yn.zhonguo4118.cn

Go:   json.Unmarshal(data, &v)
来源：https://vg.zhonguo1118.cn

Ruby: JSON.parse(s)
来源：https://dq.zhonguo8118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://om.zhonguo7118.cn

[K03] JSON 美化输出（带缩进）
来源：https://px.zhonguo1118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://pj.zhonguo8118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://bl.zhonguo3118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://nx.zhonguo2118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://jh.zhonguo4118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://ka.zhonguo8118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://bb.zhonguo6118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://hy.zhonguo2118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://bk.zhonguo7118.cn

[K04] 读取 JSON 文件
来源：https://xt.zhonguo2118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://kz.zhonguo5118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://by.zhonguo2118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://mr.zhonguo8118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://bj.zhonguo1118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://tr.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://cf.zhonguo1118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://zk.zhonguo7118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://ye.zhonguo3118.cn

[K05] 深拷贝对象
来源：https://ia.zhonguo2118.cn

Py:   copy.deepcopy(obj)
来源：https://ls.zhonguo4118.cn

PHP:  unserialize(serialize($obj));
来源：https://li.zhonguo6118.cn

JS:   structuredClone(obj)
来源：https://tu.zhonguo7118.cn

TS:   structuredClone(obj)
来源：https://rm.zhonguo3118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://ru.zhonguo1118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://pw.zhonguo5118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://qu.zhonguo5118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://cv.zhonguo6118.cn

[K06] 解析 URL 查询串
来源：https://kg.zhonguo3118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://nt.zhonguo3118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://er.zhonguo3118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://yb.zhonguo5118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://rh.zhonguo1118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://qb.zhonguo6118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://es.zhonguo8118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://zc.zhonguo3118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://ke.zhonguo8118.cn

[K07] 进制转换
来源：https://gz.zhonguo4118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://xj.zhonguo5118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://cx.zhonguo1118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://lh.zhonguo5118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://hs.zhonguo5118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://ku.zhonguo7118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://bz.zhonguo1118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://sz.zhonguo1118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://is.zhonguo8118.cn

[K08] 二进制序列化（非 JSON）
来源：https://gh.zhonguo8118.cn

Py:   pickle.dumps(obj)
来源：https://ec.zhonguo3118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://zb.zhonguo4118.cn

JS:   v8.serialize(obj)        // Node
来源：https://bu.zhonguo7118.cn

TS:   v8.serialize(obj)        // Node
来源：https://vw.zhonguo4118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://vv.zhonguo8118.cn

Go:   encoding/gob
来源：https://rn.zhonguo6118.cn

Ruby: Marshal.dump(obj)
来源：https://lx.zhonguo3118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://zn.zhonguo6118.cn

================================================================================
来源：https://oe.zhonguo1118.cn

L. 网络请求
来源：https://gl.zhonguo4118.cn

================================================================================
来源：https://lu.zhonguo2118.cn

[L01] 发送 GET 请求
来源：https://ym.zhonguo1118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://sj.zhonguo6118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://xb.zhonguo6118.cn

JS:   await fetch(url)
来源：https://hu.zhonguo7118.cn

TS:   await fetch(url)
来源：https://px.zhonguo6118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://mr.zhonguo4118.cn

Go:   resp, err := http.Get(url)
来源：https://vr.zhonguo7118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://fd.zhonguo3118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://wx.zhonguo7118.cn

[L02] 发送 POST JSON
来源：https://zp.zhonguo4118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://hq.zhonguo5118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://cq.zhonguo8118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://dn.zhonguo7118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://mz.zhonguo3118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://rv.zhonguo6118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://rj.zhonguo6118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://pl.zhonguo7118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://go.zhonguo7118.cn

[L03] 设置自定义请求头
来源：https://sy.zhonguo7118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://kq.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://cs.zhonguo2118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://jw.zhonguo8118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://ut.zhonguo7118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://wr.zhonguo1118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://iq.zhonguo4118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://rh.zhonguo3118.cn


<!-- 参考信息 -->