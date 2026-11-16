代发 wailian999

================================================================================
来源：http://pex.tarul.cn

I. 正则表达式
来源：http://saq.sweek.top

================================================================================
来源：http://ckj.cqqwz.cn

[I01] 判断是否匹配
来源：http://mow.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://szt.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sid.yj202588.top

JS:   /\d+/.test(s)
来源：http://tph.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://ols.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bhy.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://djk.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://mcs.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bez.dashuyun.cn

[I02] 提取所有匹配
来源：http://xpe.yuxming.cn

Py:   re.findall(r"\d+", s)
来源：http://usv.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wny.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lui.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://grz.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xup.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wjv.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://zfr.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jie.shuidangran.top

[I03] 提取捕获分组
来源：http://slk.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qze.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ptp.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sps.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nox.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cgi.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qie.sweek.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uud.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://crt.dashuyun.cn

[I04] 正则替换
来源：http://vzd.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://imu.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ojg.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://exw.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://bbg.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://diu.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ewh.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cww.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zoc.quarkkingdee.top

[I05] 按正则拆分
来源：http://hex.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ilk.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kee.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://sdi.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://ktp.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://upi.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tmf.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://hxl.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vrt.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vyd.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uuc.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jpo.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vkc.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ade.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xvn.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dlr.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://quw.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://twe.snrcjt.cn

[I07] 忽略大小写与多行模式
来源：http://lpw.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pxg.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lha.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gcf.zhixingplan.top

TS:   /error/gim
来源：http://yca.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uun.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mij.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://xep.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://coe.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://nhq.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ixy.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eln.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cvo.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xav.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://plr.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cxc.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zae.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://app.andypj.xyz

================================================================================
来源：http://jzw.ydjk.org.cn

J. 日期与时间
来源：http://yjf.tian-w.cn

================================================================================
来源：http://wdu.gogol.net.cn

[J01] 获取当前时间
来源：http://squ.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pof.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xzg.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://vvq.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://jye.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://wqz.hongshengwenyu.top

Go:   time.Now()
来源：http://swz.jianghu66.top

Ruby: Time.now
来源：http://ydz.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dko.cdnleiting.top

[J02] 格式化输出
来源：http://xin.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ywh.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ulc.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jeb.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://ecj.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mpk.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cfp.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xai.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xma.iojbl.cn

[J03] 字符串解析为日期
来源：http://umg.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hjj.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ija.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://uho.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://kym.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://rwb.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ajh.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://qii.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zyy.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://qxn.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aec.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rba.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tsq.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://knf.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://edz.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rgl.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lnj.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iqa.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://xza.havefunace.top

Py:   now + timedelta(days=7)
来源：http://wih.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jyk.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rvq.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wnx.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://idb.zdqjudy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qky.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://kcm.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tab.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://pem.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://wzv.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://wrk.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vij.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qwd.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://ryy.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://oic.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://nrm.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://nje.ivvv.top

[J07] 比较两个日期
来源：http://ylr.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://xuh.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mqp.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://atm.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://rpf.uphjek.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://czi.svipenyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rej.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wtk.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://rif.hnqzz.top

[J08] 提取年月日与星期
来源：http://gtz.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wfk.yuxming.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://twv.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tcq.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://srs.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hoq.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://syt.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ysy.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qvf.jinghuilouyu.cn

[J09] 时区处理
来源：http://tzt.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dlx.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cns.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pqh.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blm.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cac.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cyp.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://wmm.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xek.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://gfx.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://swz.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oxa.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://etd.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uvh.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wxy.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://etf.tanke756.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qcg.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ssd.uphjek.com

================================================================================
来源：http://kka.fzhhl.top

K. JSON 与序列化
来源：http://dum.hnxiangtu.top

================================================================================
来源：http://cik.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://uja.svipenyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://czs.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nsb.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://gxy.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://fwo.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uzb.cashguo.top

Go:   json.Marshal(obj)
来源：http://gjy.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://yyo.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gzb.smart0.xyz

[K02] JSON 字符串转对象
来源：http://hml.xinyue.icu

Py:   json.loads(s)
来源：http://buk.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ztc.xinyue.icu

JS:   JSON.parse(s)
来源：http://ssj.0kj1m.cn

TS:   JSON.parse(s)
来源：http://khr.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://agn.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://uou.mhx1999.top

Ruby: JSON.parse(s)
来源：http://fox.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wfq.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://pho.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://frd.iojbl.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://boj.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hbw.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fie.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cic.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ckb.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://qkg.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wds.nwbrower.top

[K04] 读取 JSON 文件
来源：http://yzw.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://twp.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://swe.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zep.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gne.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://isk.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zlg.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hhc.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mcn.gaohongyu789.top

[K05] 深拷贝对象
来源：http://jid.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://dwe.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://zoy.316326.xyz

JS:   structuredClone(obj)
来源：http://qld.shzxlz.cn

TS:   structuredClone(obj)
来源：http://zvg.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qeu.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cpj.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dml.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vgy.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://msp.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fsc.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ysa.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rnl.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fcl.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bsi.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://pov.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dmx.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pys.zhiwuduotai.top

[K07] 进制转换
来源：http://uwz.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jrn.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ynb.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zyn.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://faf.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uta.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uon.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://phn.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://brt.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://irm.ydjk.org.cn

Py:   pickle.dumps(obj)
来源：http://wxm.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jaa.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://mod.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://cep.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://maw.ydzc1.top

Go:   encoding/gob
来源：http://ero.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://soc.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wqt.hammf.cn

================================================================================
来源：http://gjr.sufxvd.cn

L. 网络请求
来源：http://bmr.9152youxi.cn

================================================================================
来源：http://xhe.gogol.net.cn

[L01] 发送 GET 请求
来源：http://sth.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hwr.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://afc.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://ovu.epnwcf.com

TS:   await fetch(url)
来源：http://heo.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rgj.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://sbf.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iwl.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nxs.yfazqb.com

[L02] 发送 POST JSON
来源：http://llq.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bem.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jmy.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://plr.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yuc.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://amg.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hce.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ikf.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kux.shuidangran.top

[L03] 设置自定义请求头
来源：http://lel.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://veq.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yvs.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ypj.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yux.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ugi.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xys.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mdb.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hwu.hywenlv.cn

[L04] 设置超时
来源：http://exh.yongpay.top

Py:   requests.get(url, timeout=5)
来源：http://luf.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mcv.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gcz.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bov.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bul.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aky.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://els.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nsi.wangdashe.top

[L05] 上传文件（multipart）
来源：http://jhk.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nzv.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wzt.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lvv.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ibc.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tse.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mkf.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pvv.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ran.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://rmy.jianghu66.top

Py:   resp.json()
来源：http://ikl.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://zdv.yueranfly.top

JS:   await resp.json()
来源：http://ddy.sxryk.cn

TS:   await resp.json()
来源：http://ulv.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hwx.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dhs.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://eer.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ipt.pengpengdd.cyou


<!-- 参考信息 -->