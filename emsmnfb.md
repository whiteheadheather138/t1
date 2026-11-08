代发 wailian999

[I02] 提取所有匹配
来源：https://bp.zhonguo5118.cn

Py:   re.findall(r"\d+", s)
来源：https://vm.zhonguo3118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://jy.zhonguo7118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://yn.zhonguo2118.cn

TS:   s.match(/\d+/g)
来源：https://eq.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://ix.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://pe.zhonguo4118.cn

Ruby: s.scan(/\d+/)
来源：https://pk.zhonguo8118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://kk.zhonguo3118.cn

[I03] 提取捕获分组
来源：https://sd.zhonguo4118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://yc.zhonguo6118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://yv.zhonguo8118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://dd.zhonguo6118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://kd.zhonguo4118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://nf.zhonguo8118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://rr.zhonguo7118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://yj.zhonguo4118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://lq.zhonguo4118.cn

[I04] 正则替换
来源：https://pi.zhonguo6118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://mv.zhonguo6118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://nw.zhonguo2118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://ju.zhonguo6118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://ut.zhonguo7118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://hq.zhonguo7118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://uq.zhonguo5118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://bl.zhonguo4118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://fd.zhonguo3118.cn

[I05] 按正则拆分
来源：https://sa.zhonguo4118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://lx.zhonguo2118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://ca.zhonguo3118.cn

JS:   s.split(/\s*,\s*/)
来源：https://hw.zhonguo7118.cn

TS:   s.split(/\s*,\s*/)
来源：https://fi.zhonguo8118.cn

Java: s.split("\\s*,\\s*")
来源：https://ef.zhonguo3118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://nn.zhonguo1118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://fm.zhonguo6118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://ic.zhonguo3118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://qa.zhonguo8118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://gi.zhonguo6118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://yz.zhonguo1118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://hb.zhonguo1118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://dq.zhonguo1118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://ka.zhonguo3118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://af.zhonguo1118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://fk.zhonguo2118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://uz.zhonguo2118.cn

[I07] 忽略大小写与多行模式
来源：https://eb.zhonguo6118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://qw.zhonguo5118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://oy.zhonguo6118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://oj.zhonguo3118.cn

TS:   /error/gim
来源：https://qm.zhonguo1118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://nt.zhonguo8118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://ln.zhonguo4118.cn

Ruby: s.scan(/error/i)
来源：https://kl.zhonguo7118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://om.zhonguo6118.cn

[I08] 贪婪与非贪婪匹配
来源：https://ku.zhonguo4118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://rh.zhonguo2118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://qs.zhonguo1118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://wq.zhonguo4118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://he.zhonguo3118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://vh.zhonguo8118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://pf.zhonguo7118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://zn.zhonguo7118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://tt.zhonguo6118.cn

================================================================================
来源：https://zk.zhonguo6118.cn

J. 日期与时间
来源：https://il.zhonguo6118.cn

================================================================================
来源：https://qt.zhonguo4118.cn

[J01] 获取当前时间
来源：https://pk.zhonguo2118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://vz.zhonguo8118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://ty.zhonguo2118.cn

JS:   new Date();  Date.now()
来源：https://fq.zhonguo7118.cn

TS:   new Date();  Date.now()
来源：https://ty.zhonguo5118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://lu.zhonguo5118.cn

Go:   time.Now()
来源：https://fc.zhonguo5118.cn

Ruby: Time.now
来源：https://ta.zhonguo7118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://qd.zhonguo2118.cn

[J02] 格式化输出
来源：https://hk.zhonguo2118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://lr.zhonguo7118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://ow.zhonguo2118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://ve.zhonguo7118.cn

TS:   d.toISOString()
来源：https://xw.zhonguo3118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://yy.zhonguo4118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://ac.zhonguo7118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://jf.zhonguo7118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://jm.zhonguo2118.cn

[J03] 字符串解析为日期
来源：https://gp.zhonguo7118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://ej.zhonguo7118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://oj.zhonguo2118.cn

JS:   new Date("2024-01-02")
来源：https://ei.zhonguo8118.cn

TS:   new Date("2024-01-02")
来源：https://kc.zhonguo4118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://kv.zhonguo1118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://ik.zhonguo2118.cn

Ruby: Date.parse("2024-01-02")
来源：https://rp.zhonguo2118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://cs.zhonguo3118.cn

[J04] 时间戳与日期互转
来源：https://jf.zhonguo3118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://sg.zhonguo6118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://tz.zhonguo2118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://jq.zhonguo4118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://si.zhonguo1118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://ic.zhonguo5118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://pu.zhonguo5118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://kt.zhonguo5118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://ul.zhonguo6118.cn

[J05] 时间加减（加 7 天）
来源：https://lh.zhonguo3118.cn

Py:   now + timedelta(days=7)
来源：https://ea.zhonguo4118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://hk.zhonguo5118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://zt.zhonguo5118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://zo.zhonguo3118.cn

Java: LocalDate.now().plusDays(7)
来源：https://yj.zhonguo6118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://wv.zhonguo6118.cn

Ruby: Time.now + 7 * 86400
来源：https://hu.zhonguo5118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://wv.zhonguo1118.cn

[J06] 计算两时间之差
来源：https://ms.zhonguo8118.cn

Py:   (end - start).total_seconds()
来源：https://bk.zhonguo3118.cn

PHP:  $end->diff($start)->days;
来源：https://jd.zhonguo2118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://au.zhonguo3118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://px.zhonguo3118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://xx.zhonguo3118.cn

Go:   end.Sub(start).Hours()
来源：https://vg.zhonguo2118.cn

Ruby: end - start                 # 返回秒数
来源：https://ac.zhonguo1118.cn

C#:   (end - start).TotalSeconds
来源：https://gv.zhonguo1118.cn

[J07] 比较两个日期
来源：https://wa.zhonguo1118.cn

Py:   d1 < d2;  d1 == d2
来源：https://lo.zhonguo5118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://ij.zhonguo4118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://yh.zhonguo6118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://zl.zhonguo6118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://qf.zhonguo2118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://pw.zhonguo7118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://ht.zhonguo2118.cn

C#:   d1 < d2;  d1 == d2
来源：https://rr.zhonguo4118.cn

[J08] 提取年月日与星期
来源：https://ew.zhonguo3118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://qh.zhonguo3118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://ah.zhonguo6118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://bq.zhonguo1118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://si.zhonguo1118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://qi.zhonguo1118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://ua.zhonguo8118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://xf.zhonguo1118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://hc.zhonguo7118.cn

[J09] 时区处理
来源：https://mw.zhonguo4118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://bx.zhonguo8118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://zb.zhonguo1118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://ey.zhonguo5118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://kr.zhonguo3118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://qx.zhonguo1118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://yg.zhonguo4118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://mr.zhonguo4118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://mz.zhonguo4118.cn

[J10] 取今天 / 本月第一天
来源：https://dy.zhonguo7118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://zs.zhonguo2118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://cr.zhonguo3118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://ar.zhonguo3118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://vs.zhonguo5118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://ix.zhonguo8118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://wn.zhonguo5118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://om.zhonguo5118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://jt.zhonguo4118.cn

================================================================================
来源：https://oi.zhonguo7118.cn

K. JSON 与序列化
来源：https://ih.zhonguo4118.cn

================================================================================
来源：https://ba.zhonguo4118.cn

[K01] 对象转 JSON 字符串
来源：https://aq.zhonguo5118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://vv.zhonguo3118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://jv.zhonguo6118.cn

JS:   JSON.stringify(obj)
来源：https://xr.zhonguo8118.cn

TS:   JSON.stringify(obj)
来源：https://hs.zhonguo6118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://ny.zhonguo2118.cn

Go:   json.Marshal(obj)
来源：https://jd.zhonguo2118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://gc.zhonguo8118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://qd.zhonguo6118.cn

[K02] JSON 字符串转对象
来源：https://cf.zhonguo6118.cn

Py:   json.loads(s)
来源：https://bd.zhonguo2118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://es.zhonguo3118.cn

JS:   JSON.parse(s)
来源：https://zn.zhonguo7118.cn

TS:   JSON.parse(s)
来源：https://ia.zhonguo7118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://lw.zhonguo4118.cn

Go:   json.Unmarshal(data, &v)
来源：https://xo.zhonguo5118.cn

Ruby: JSON.parse(s)
来源：https://mj.zhonguo6118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://js.zhonguo5118.cn

[K03] JSON 美化输出（带缩进）
来源：https://fv.zhonguo7118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://xt.zhonguo5118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://pc.zhonguo3118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://vd.zhonguo7118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://fm.zhonguo3118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://fg.zhonguo7118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://gv.zhonguo8118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://nx.zhonguo5118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://dn.zhonguo2118.cn

[K04] 读取 JSON 文件
来源：https://gh.zhonguo3118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://ma.zhonguo2118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://iw.zhonguo3118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://pm.zhonguo5118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://yh.zhonguo4118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://zp.zhonguo2118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://rb.zhonguo1118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://yo.zhonguo8118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://tz.zhonguo5118.cn

[K05] 深拷贝对象
来源：https://xy.zhonguo8118.cn

Py:   copy.deepcopy(obj)
来源：https://ee.zhonguo5118.cn

PHP:  unserialize(serialize($obj));
来源：https://qi.zhonguo8118.cn

JS:   structuredClone(obj)
来源：https://pm.zhonguo7118.cn

TS:   structuredClone(obj)
来源：https://pw.zhonguo3118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://qv.zhonguo3118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://xk.zhonguo4118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://bf.zhonguo7118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://pu.zhonguo6118.cn

[K06] 解析 URL 查询串
来源：https://ng.zhonguo4118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://wr.zhonguo4118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://jx.zhonguo2118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://tl.zhonguo4118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://qe.zhonguo4118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://nf.zhonguo8118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://hf.zhonguo7118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://zb.zhonguo4118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://fy.zhonguo8118.cn

[K07] 进制转换
来源：https://ip.zhonguo3118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://bp.zhonguo3118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://ts.zhonguo1118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://gq.zhonguo1118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://oj.zhonguo4118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://jl.zhonguo4118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://gw.zhonguo7118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://pf.zhonguo6118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://bv.zhonguo5118.cn

[K08] 二进制序列化（非 JSON）
来源：https://du.zhonguo4118.cn

Py:   pickle.dumps(obj)
来源：https://uu.zhonguo8118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://od.zhonguo4118.cn

JS:   v8.serialize(obj)        // Node
来源：https://qq.zhonguo3118.cn

TS:   v8.serialize(obj)        // Node
来源：https://ap.zhonguo3118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://xs.zhonguo5118.cn

Go:   encoding/gob
来源：https://xz.zhonguo7118.cn

Ruby: Marshal.dump(obj)
来源：https://ko.zhonguo7118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://pq.zhonguo5118.cn

================================================================================
来源：https://py.zhonguo3118.cn

L. 网络请求
来源：https://ej.zhonguo3118.cn

================================================================================
来源：https://lm.zhonguo8118.cn

[L01] 发送 GET 请求
来源：https://qg.zhonguo8118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://lc.zhonguo1118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://pp.zhonguo3118.cn

JS:   await fetch(url)
来源：https://qv.zhonguo5118.cn

TS:   await fetch(url)
来源：https://jb.zhonguo4118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://ou.zhonguo1118.cn

Go:   resp, err := http.Get(url)
来源：https://fs.zhonguo4118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://dk.zhonguo3118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://wo.zhonguo4118.cn

[L02] 发送 POST JSON
来源：https://bb.zhonguo3118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://kx.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://gp.zhonguo8118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://je.zhonguo8118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://th.zhonguo2118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://di.zhonguo8118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://yw.zhonguo7118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://fe.zhonguo3118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://zl.zhonguo3118.cn

[L03] 设置自定义请求头
来源：https://um.zhonguo3118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://pb.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://wb.zhonguo8118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://le.zhonguo7118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://hg.zhonguo8118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://qv.zhonguo3118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://zp.zhonguo3118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://kn.zhonguo5118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://fh.zhonguo2118.cn

[L04] 设置超时
来源：https://mv.zhonguo4118.cn

Py:   requests.get(url, timeout=5)
来源：https://tn.zhonguo4118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://vy.zhonguo5118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://qs.zhonguo1118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://pq.zhonguo6118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://cr.zhonguo3118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://rc.zhonguo6118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://mg.zhonguo5118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://oc.zhonguo2118.cn

[L05] 上传文件（multipart）
来源：https://sv.zhonguo3118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://fp.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://cs.zhonguo8118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://st.zhonguo2118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://xd.zhonguo3118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://ug.zhonguo7118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://gi.zhonguo5118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://dg.zhonguo2118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://gt.zhonguo5118.cn

[L06] 解析响应为 JSON
来源：https://wv.zhonguo7118.cn

Py:   resp.json()
来源：https://cp.zhonguo3118.cn

PHP:  json_decode($body, true);
来源：https://kw.zhonguo6118.cn

JS:   await resp.json()
来源：https://qu.zhonguo3118.cn

TS:   await resp.json()
来源：https://gf.zhonguo8118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://nn.zhonguo6118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://jm.zhonguo8118.cn

Ruby: JSON.parse(resp.body)
来源：https://nv.zhonguo6118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://ok.zhonguo5118.cn

[L07] 处理 HTTP 状态码
来源：https://fi.zhonguo1118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://tw.zhonguo5118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://ra.zhonguo2118.cn

JS:   resp.ok;  resp.status
来源：https://ps.zhonguo3118.cn

TS:   resp.ok;  resp.status
来源：https://xn.zhonguo5118.cn

Java: resp.statusCode()
来源：https://lt.zhonguo5118.cn

Go:   resp.StatusCode
来源：https://gu.zhonguo4118.cn

Ruby: resp.code.to_i
来源：https://cn.zhonguo8118.cn

C#:   (int)resp.StatusCode
来源：https://wp.zhonguo6118.cn

[L08] 并发请求多个地址
来源：https://gc.zhonguo1118.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：https://dw.zhonguo8118.cn

PHP:  curl_multi_init() 系列
来源：https://hr.zhonguo3118.cn


<!-- 参考信息 -->