代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://roi.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ggp.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://psm.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://loc.gaohongyu789.top

[I02] 提取所有匹配
来源：http://saf.tanke756.top

Py:   re.findall(r"\d+", s)
来源：http://wkc.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ccq.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bst.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://owc.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wzv.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fnl.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://tgk.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xdz.9152youxi.cn

[I03] 提取捕获分组
来源：http://anb.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://saf.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bvv.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tnn.ybcxt.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ifc.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://evh.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xgx.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rzh.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jaf.sufxvd.cn

[I04] 正则替换
来源：http://xsv.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jwo.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qds.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://kab.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ljq.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://spr.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kyq.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iqp.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://smk.yonumen.top

[I05] 按正则拆分
来源：http://jwp.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ksr.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vdv.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://nzp.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://afm.bbcook.cn

Java: s.split("\\s*,\\s*")
来源：http://ymx.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hwj.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://ymg.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ihm.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nrs.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gnw.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ktd.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dnq.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qtr.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://drc.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vpm.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pio.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eku.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://zue.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pmq.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iyi.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jcr.xylfe.cn

TS:   /error/gim
来源：http://kke.nanxinkj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xuc.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bul.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://lzp.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yvv.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://ecn.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ikc.yuxming.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vxc.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dux.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://otr.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xss.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ofk.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vut.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://any.hongshengwenyu.top

================================================================================
来源：http://zom.yvedp.cn

J. 日期与时间
来源：http://jlj.jqgufenzy.top

================================================================================
来源：http://eaj.tianlin.xyz

[J01] 获取当前时间
来源：http://wya.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tii.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qdu.nwbrower.top

JS:   new Date();  Date.now()
来源：http://foc.c1oappe.top

TS:   new Date();  Date.now()
来源：http://yqi.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fif.yj20258888.top

Go:   time.Now()
来源：http://uri.yuxming.cn

Ruby: Time.now
来源：http://rfh.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gwz.sysykeji.top

[J02] 格式化输出
来源：http://lwn.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jsz.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gkn.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mlv.jinqigfzy.top

TS:   d.toISOString()
来源：http://yjz.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wcg.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://krs.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vvm.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uwi.meibo888.top

[J03] 字符串解析为日期
来源：http://zel.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bya.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://srm.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://ffb.yongpay.top

TS:   new Date("2024-01-02")
来源：http://hbh.yangfankeji.com

Java: LocalDate.parse("2024-01-02")
来源：http://ijf.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ytu.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://lxm.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gni.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://aro.hywenlv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nyc.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bpm.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://npo.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zxo.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jwa.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vnt.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vdi.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lam.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://ssh.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://feq.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ori.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dwg.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sck.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://cci.ehwqpu.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://egp.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://lld.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://csh.iojbl.cn

[J06] 计算两时间之差
来源：http://lnk.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://ski.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://lab.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gde.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rqg.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nay.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://cqy.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://yhg.mhx1999.top

C#:   (end - start).TotalSeconds
来源：http://qtr.gaohongyu789.top

[J07] 比较两个日期
来源：http://fov.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://hxq.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://unt.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://efv.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://vhx.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jrc.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qxf.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://mtr.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://lgh.hcnkem.com

[J08] 提取年月日与星期
来源：http://vhh.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dns.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qbo.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nqw.jinqigufen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://plb.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dug.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xao.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ift.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jin.yueranfly.top

[J09] 时区处理
来源：http://mqx.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nbg.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gax.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rrm.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bmx.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mae.hysaishi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://axo.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mvw.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://spa.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://hfm.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fpv.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xmf.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fam.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://akq.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pjn.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dhb.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hvm.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mwt.yj202588.top

================================================================================
来源：http://ejr.hysaishi.cn

K. JSON 与序列化
来源：http://nas.tianlin.xyz

================================================================================
来源：http://dky.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://qfz.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wzd.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ent.nwbrower.top

JS:   JSON.stringify(obj)
来源：http://bja.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://jga.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jgl.tanke756.top

Go:   json.Marshal(obj)
来源：http://dva.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://wup.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ypa.cucudq.cn

[K02] JSON 字符串转对象
来源：http://idv.bbcook.cn

Py:   json.loads(s)
来源：http://itp.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://krn.vehdjk.com

JS:   JSON.parse(s)
来源：http://spf.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://ciq.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ogi.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://xcf.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://dlc.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ezy.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://pjp.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fse.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xkt.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gsr.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jbc.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jjv.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xxn.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://wch.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xgc.ybcxt.top

[K04] 读取 JSON 文件
来源：http://myl.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hrj.yfazqb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gyy.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tmz.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mzk.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qyo.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qyy.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qsu.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lub.daxiang520.top

[K05] 深拷贝对象
来源：http://fgh.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://kqz.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://nxo.yuxming.cn

JS:   structuredClone(obj)
来源：http://jfz.chenzaomai.com

TS:   structuredClone(obj)
来源：http://ogz.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bqy.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ehx.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://msn.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ojl.smart0.xyz

[K06] 解析 URL 查询串
来源：http://rdp.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yvn.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://chx.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tuq.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gdw.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tje.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xyd.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://szt.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fhi.shanyushiyangkeji.top

[K07] 进制转换
来源：http://arj.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://egy.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wwq.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bwj.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rta.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nba.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nok.yvedp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ugo.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iuz.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://qic.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://mku.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tft.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://ilt.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://lha.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qeg.ehwqpu.com

Go:   encoding/gob
来源：http://dfn.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://fbv.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rby.zycfv.cn

================================================================================
来源：http://sll.xuanzx.com

L. 网络请求
来源：http://dvz.quarkkingdee.top

================================================================================
来源：http://pnm.yfazqb.com

[L01] 发送 GET 请求
来源：http://wjh.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ghv.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ujo.hnxiangtu.top

JS:   await fetch(url)
来源：http://uos.aibaodan.cn

TS:   await fetch(url)
来源：http://jer.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fcf.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://hok.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://moz.nwbrower.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://crg.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://dta.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://ndt.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kbt.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://igx.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://llj.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://est.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ozm.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hzb.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tio.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://tau.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kfw.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sin.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zxl.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eye.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jyv.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bas.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mef.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hzx.dianchejie.cn

[L04] 设置超时
来源：http://jqi.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://omo.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jri.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qdh.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://non.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bhx.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qtx.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://evc.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gwd.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://czs.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ugb.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ukh.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fuu.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://haz.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kpi.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tfe.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mav.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gox.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://xcp.jqgufenzy.top

Py:   resp.json()
来源：http://llv.birdmap.top

PHP:  json_decode($body, true);
来源：http://yvv.snrcjt.cn

JS:   await resp.json()
来源：http://mmg.feifeiyinyue.top

TS:   await resp.json()
来源：http://cyn.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gur.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cpu.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://kjp.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vjp.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://zkr.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jpm.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jnj.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://yza.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://gwc.fehbvm.com

Java: resp.statusCode()
来源：http://zcl.fktsv.cn

Go:   resp.StatusCode
来源：http://msu.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://xgy.chenlongwang.top


<!-- 参考信息 -->