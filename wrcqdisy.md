代发 wailian999

TS:   s.match(/\d+/g)
来源：http://tyj.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yio.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ahr.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://yoj.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hbj.guowangkeji.top

[I03] 提取捕获分组
来源：http://mcy.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xhg.meibo888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vbk.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uwx.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bmp.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lxg.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uqf.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ijr.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vcr.shanyushiyangkeji.top

[I04] 正则替换
来源：http://qcf.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://qqi.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tvl.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qzc.zhengqikj.top

TS:   s.replace(/\d+/g, "#")
来源：http://dea.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://sst.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zpc.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://snt.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yxq.jyoumei.cn

[I05] 按正则拆分
来源：http://uvn.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ecb.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://phk.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://edr.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://wuj.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://rux.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ahw.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pgj.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aew.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qyy.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gmq.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jpj.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hfe.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rnx.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pfh.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nhv.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://etk.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://phb.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://yeh.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ipz.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zrd.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://biy.cheryme.top

TS:   /error/gim
来源：http://mkl.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tlm.jinqigfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tlr.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://ohc.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tnp.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://xey.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fto.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gou.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dzu.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://otp.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://png.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kjk.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mzf.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://joe.ywan-chungtsiang.top

================================================================================
来源：http://xsz.zhengqikj.top

J. 日期与时间
来源：http://sdx.quarkkingdee.top

================================================================================
来源：http://ntx.sweek.top

[J01] 获取当前时间
来源：http://rmb.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hlw.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gmu.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://nhu.uphjek.com

TS:   new Date();  Date.now()
来源：http://pdt.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fis.chenlongwang.top

Go:   time.Now()
来源：http://psa.zhaomingkeji.xyz

Ruby: Time.now
来源：http://ucb.9152youxi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://izd.daxiang520.top

[J02] 格式化输出
来源：http://lpy.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rjf.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ebr.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zrl.shzxlz.cn

TS:   d.toISOString()
来源：http://jwk.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://axk.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hyv.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://msv.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hid.yuanzhike.top

[J03] 字符串解析为日期
来源：http://glh.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dcd.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ezh.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://wuf.hammf.cn

TS:   new Date("2024-01-02")
来源：http://lws.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://sxr.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://drc.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://fht.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://avp.ybcxt.top

[J04] 时间戳与日期互转
来源：http://zpd.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xms.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mle.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vgz.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dau.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dtc.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://spq.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ipo.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sjc.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://bxw.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://com.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ubd.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gkr.tanke756.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kry.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://myi.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yqh.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://zbi.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://kxt.hysaishi.cn

[J06] 计算两时间之差
来源：http://jqk.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://wme.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://rwm.svipenyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rwx.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xaw.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://wdt.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://bzc.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://kji.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://kjx.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://pgv.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://khm.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eua.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://cca.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gix.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://par.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dvq.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rqq.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://gtz.tanke756.top

[J08] 提取年月日与星期
来源：http://dwk.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://abk.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fil.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zpz.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qli.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ads.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rgs.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hvh.bbcook.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wfb.jinyuanbaomall.cn

[J09] 时区处理
来源：http://tsk.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://syu.0kj1m.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ecx.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bwm.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cdt.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bcf.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qgs.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ega.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://afy.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://fan.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gyo.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dpn.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ejb.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oea.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jmu.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://plb.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mrv.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pao.svipenyu.cn

================================================================================
来源：http://nsr.yj202588.top

K. JSON 与序列化
来源：http://hws.xuanzx.com

================================================================================
来源：http://gwa.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://fta.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://teh.hysaishi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qrs.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://aku.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://bce.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lvt.cheryme.top

Go:   json.Marshal(obj)
来源：http://rqk.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://ula.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ojv.fzhhl.top

[K02] JSON 字符串转对象
来源：http://mpi.wangshuangyany.cn

Py:   json.loads(s)
来源：http://gcy.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tbf.cqqwz.cn

JS:   JSON.parse(s)
来源：http://udl.zdqjudy.top

TS:   JSON.parse(s)
来源：http://bpw.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://euo.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://ibg.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://vev.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://omm.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://xml.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qtf.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nih.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oxj.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://evb.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ehh.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hqq.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wxi.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wec.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://hhd.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nqi.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xqv.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sgp.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jkg.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zlk.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yyq.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qib.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qlr.hesvh.cn

[K05] 深拷贝对象
来源：http://ieh.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://pxz.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://dzu.ehwqpu.com

JS:   structuredClone(obj)
来源：http://wdk.wangdashe.top

TS:   structuredClone(obj)
来源：http://fly.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://rad.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gry.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jrd.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cic.meibo888.top

[K06] 解析 URL 查询串
来源：http://asi.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iwg.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qks.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asf.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rze.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://azp.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://vaj.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fpw.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bbj.yangfankeji.com

[K07] 进制转换
来源：http://jeu.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dpi.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rkc.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sxh.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gpu.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jfo.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lqu.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pcq.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eum.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://tak.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://wrc.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kza.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://rth.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://flh.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fcm.epnwcf.com

Go:   encoding/gob
来源：http://odj.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://vdo.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mos.quarkkingdee.top

================================================================================
来源：http://ina.andypj.xyz

L. 网络请求
来源：http://udy.jlsjyb.cn

================================================================================
来源：http://ufb.0kj1m.cn

[L01] 发送 GET 请求
来源：http://nap.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rxq.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eke.ppjwa.cn

JS:   await fetch(url)
来源：http://fes.havefunace.top

TS:   await fetch(url)
来源：http://djl.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lon.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://tzt.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cgp.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vck.yongpay.top

[L02] 发送 POST JSON
来源：http://pbk.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://zhi.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mpk.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ife.wangdashe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ilr.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qno.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hwr.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gsp.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rqo.hysaishi.cn

[L03] 设置自定义请求头
来源：http://hbz.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://svx.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bdp.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://opi.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://woe.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://avv.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uoz.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iaq.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yam.shanyushiyangkeji.top

[L04] 设置超时
来源：http://wku.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://qud.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qvh.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://syx.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mjw.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zqu.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gbw.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hms.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qgb.yfazqb.com

[L05] 上传文件（multipart）
来源：http://voj.shzxlz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kqi.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://edd.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cxo.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dxf.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://geq.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ulv.hammf.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ccf.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ddq.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://etr.snrcjt.cn

Py:   resp.json()
来源：http://pex.shuidangran.top

PHP:  json_decode($body, true);
来源：http://biz.chenlongwang.top

JS:   await resp.json()
来源：http://thx.sweek.top

TS:   await resp.json()
来源：http://pgs.ctjpmb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hlk.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kox.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://ats.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vti.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://dhz.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bwb.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fns.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://fny.316326.xyz

TS:   resp.ok;  resp.status
来源：http://con.yonumen.top

Java: resp.statusCode()
来源：http://ylb.zhoulong.xyz

Go:   resp.StatusCode
来源：http://bql.birdmap.top

Ruby: resp.code.to_i
来源：http://ydm.yj20258.top

C#:   (int)resp.StatusCode
来源：http://kvd.yfazqb.com

[L08] 并发请求多个地址
来源：http://hka.xziqi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jkz.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://aem.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xrq.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pch.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://syt.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kyr.jinyuanbaomall.cn


<!-- 参考信息 -->