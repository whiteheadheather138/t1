代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pwg.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://elm.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://yhx.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qef.yfazqb.com

[I02] 提取所有匹配
来源：http://zfs.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://uae.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xwj.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kpm.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://sat.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rqi.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dua.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://swe.meibo888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bem.tanke756.top

[I03] 提取捕获分组
来源：http://wks.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xfa.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xge.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rdj.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dec.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eto.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://slr.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ilp.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ljf.hnqzz.top

[I04] 正则替换
来源：http://fsa.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qqg.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ons.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://wmt.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://ewz.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://rty.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ejv.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pcs.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jun.cqqwz.cn

[I05] 按正则拆分
来源：http://vyz.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lau.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mub.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://dvu.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://vze.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://afq.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://smm.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mav.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bjg.sysykeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xzq.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oly.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jes.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enr.52xcode.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://muo.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kqm.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wbm.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uba.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yqi.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://giw.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fmu.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ktb.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ykt.guannengcc.top

TS:   /error/gim
来源：http://brg.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zqd.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://icf.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://xnz.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://whd.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://jaa.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fbw.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xxk.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gpx.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wvz.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ufq.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tbk.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://set.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://twi.fzhhl.top

================================================================================
来源：http://jev.0kj1m.cn

J. 日期与时间
来源：http://eoj.yj20258888.top

================================================================================
来源：http://ubh.zhiwuduotai.top

[J01] 获取当前时间
来源：http://cqi.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jjy.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hlg.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://ujm.bbcook.cn

TS:   new Date();  Date.now()
来源：http://wbd.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ljb.hesvh.cn

Go:   time.Now()
来源：http://hyu.yueranfly.top

Ruby: Time.now
来源：http://xas.shanyushiyangtech.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jge.ctjpmb.com

[J02] 格式化输出
来源：http://lve.yj202588.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tul.sxryk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yvf.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qcm.meibo888.top

TS:   d.toISOString()
来源：http://hml.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dfm.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ffp.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dli.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pso.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://pav.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://knq.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pcc.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://ejm.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://pav.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://mdy.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bix.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ymu.yangfankeji.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ajj.xinyue.icu

[J04] 时间戳与日期互转
来源：http://keg.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xfj.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rme.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uoa.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uje.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hza.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nru.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rsg.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mcf.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://ysv.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://igx.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://iis.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kxm.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rza.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://yso.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xtb.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://coe.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://oyg.quarkkingdee.top

[J06] 计算两时间之差
来源：http://hdj.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://gth.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://vtl.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nla.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oxq.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://vjm.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://mkc.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://gto.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://kkx.hongshengwenyu.top

[J07] 比较两个日期
来源：http://gme.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://orm.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vsx.jqgfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://gdm.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://stn.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://evs.zycfv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://chr.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://ciy.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://gct.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://yti.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://srl.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://miw.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://glc.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dmc.jinqigfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hga.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bkn.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fkf.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bvm.tanke756.top

[J09] 时区处理
来源：http://xnc.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bgn.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://daw.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://acz.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pbg.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://und.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xqv.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uiz.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kwc.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://tso.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gpf.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://keq.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vao.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rds.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://psg.jqgufenzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qrn.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kxb.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gnp.iojbl.cn

================================================================================
来源：http://qmb.hfpthk.cn

K. JSON 与序列化
来源：http://dgw.ivvv.top

================================================================================
来源：http://usk.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://dpe.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gyp.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zly.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://uaf.yj20258.top

TS:   JSON.stringify(obj)
来源：http://jiv.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nrv.hnqzz.top

Go:   json.Marshal(obj)
来源：http://ipw.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://msc.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xfs.tarul.cn

[K02] JSON 字符串转对象
来源：http://ltm.gzhubu.top

Py:   json.loads(s)
来源：http://xkp.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ghy.jyoumei.cn

JS:   JSON.parse(s)
来源：http://iex.jqgfzy.top

TS:   JSON.parse(s)
来源：http://yec.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eom.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://pqu.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://hgw.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fbp.kuanghao11.cn

[K03] JSON 美化输出（带缩进）
来源：http://hbp.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mlt.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://stz.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://utr.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wbk.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xpp.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tac.hysaishi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qda.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://swq.epnwcf.com

[K04] 读取 JSON 文件
来源：http://zoc.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kpn.jlsjyb.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vwq.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://slj.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xrq.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zng.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rav.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lqv.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://env.sxryk.cn

[K05] 深拷贝对象
来源：http://wiz.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://mbv.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://ohy.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://btc.aibaodan.cn

TS:   structuredClone(obj)
来源：http://yce.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://mcq.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://guc.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://upz.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://hwn.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://lqv.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gsq.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ydu.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hud.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sjy.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xmy.cheryme.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hwo.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mkg.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gww.tian-w.cn

[K07] 进制转换
来源：http://ahl.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ffz.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pas.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://umk.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sew.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ouv.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ayu.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hlx.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ueh.jinghuilouyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://llu.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://pdm.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bfr.meibo888.top

JS:   v8.serialize(obj)        // Node
来源：http://anm.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://akb.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kic.mhx1999.top

Go:   encoding/gob
来源：http://fzy.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://rfm.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yww.nwbrower.top

================================================================================
来源：http://oyt.ehwqpu.com

L. 网络请求
来源：http://ouk.ybcxt.top

================================================================================
来源：http://kel.xinyue.icu

[L01] 发送 GET 请求
来源：http://fpo.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hzr.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ies.nanxuanxn.top

JS:   await fetch(url)
来源：http://hjc.tian-w.cn

TS:   await fetch(url)
来源：http://hed.xinyue.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uvm.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://kdi.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bjj.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pnj.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://sqi.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://blj.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qny.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://snw.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://idm.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nqh.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://glh.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vau.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oxd.sysykeji.top

[L03] 设置自定义请求头
来源：http://koo.nanxinkj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://stu.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ijl.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jdh.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tou.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sfz.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wrs.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfg.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ghr.shangyingyoupin.top

[L04] 设置超时
来源：http://lin.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://obe.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qec.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhv.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mmp.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nci.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fij.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://enw.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tdz.wangshuangyany.cn

[L05] 上传文件（multipart）
来源：http://jen.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zxx.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nfl.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://quq.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://frp.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pmw.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zen.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eti.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jov.sxryk.cn

[L06] 解析响应为 JSON
来源：http://sdw.andypj.xyz

Py:   resp.json()
来源：http://bul.fehbvm.com

PHP:  json_decode($body, true);
来源：http://gzg.fengsongda.top

JS:   await resp.json()
来源：http://hyk.shanyushiyangkeji.top

TS:   await resp.json()
来源：http://xst.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xaq.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eng.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://vkm.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zpw.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://jci.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jjn.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ujq.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://rly.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://qab.chenzaomai.com

Java: resp.statusCode()
来源：http://mdp.epnwcf.com

Go:   resp.StatusCode
来源：http://nhy.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://iqu.tarul.cn


<!-- 参考信息 -->