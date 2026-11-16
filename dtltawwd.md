代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://ypb.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iue.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wxh.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bcw.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gtk.meibo888.top

Go:   defer f.Close()
来源：http://jwp.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pxx.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oyt.yonumen.top

================================================================================
来源：http://ead.xziqi.cn

I. 正则表达式
来源：http://esa.cucudq.cn

================================================================================
来源：http://gjm.hesvh.cn

[I01] 判断是否匹配
来源：http://ghn.ivvv.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cah.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://jtq.zhixingplan.top

JS:   /\d+/.test(s)
来源：http://gjw.fehbvm.com

TS:   /\d+/.test(s)
来源：http://ker.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lpf.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ona.xingfuxueyuan.xyz

Ruby: s.match?(/\d+/)
来源：http://mnc.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gsi.zhengqikj.top

[I02] 提取所有匹配
来源：http://qzu.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://hps.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xtm.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vik.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://leo.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gnq.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cyw.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://app.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://exq.andypj.xyz

[I03] 提取捕获分组
来源：http://oko.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jum.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qzu.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bkh.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dsw.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mnr.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ugz.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ysd.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xlk.vqdsnc.cn

[I04] 正则替换
来源：http://nox.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://pid.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zwa.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jrm.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://jec.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://doe.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hag.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sij.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://idp.xziqi.cn

[I05] 按正则拆分
来源：http://spr.316326.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://mfy.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mau.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://cbn.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://zqh.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://ykl.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://urz.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://bpb.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xxk.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vcx.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lmf.sweek.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://keu.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tky.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ese.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vca.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ccr.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cgk.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://joy.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://nwp.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yqv.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dys.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qrm.hcnkem.com

TS:   /error/gim
来源：http://dxt.zdbjq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rdk.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ejj.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://mdg.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sig.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://axj.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hfl.jyoumei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gxn.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xwg.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iii.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wix.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zxu.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tei.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xcf.dashuyun.cn

================================================================================
来源：http://aye.xziqi.cn

J. 日期与时间
来源：http://unn.hysaishi.cn

================================================================================
来源：http://hdp.gaohongyu789.top

[J01] 获取当前时间
来源：http://xwn.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fnr.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pcv.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://skl.sufxvd.cn

TS:   new Date();  Date.now()
来源：http://nxo.nanxuanxn.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qwe.zhongyouzk.top

Go:   time.Now()
来源：http://mje.snrcjt.cn

Ruby: Time.now
来源：http://fkf.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tpl.cashguo.top

[J02] 格式化输出
来源：http://eyf.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://haa.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qnn.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iob.gogol.net.cn

TS:   d.toISOString()
来源：http://esn.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zel.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kxg.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xlb.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hvx.jiagoushi.top

[J03] 字符串解析为日期
来源：http://jfv.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uso.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://efw.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://oej.kuanghao11.cn

TS:   new Date("2024-01-02")
来源：http://kxv.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yls.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fdq.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://qyx.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kbw.tarul.cn

[J04] 时间戳与日期互转
来源：http://smm.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jps.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://goi.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://inz.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iwr.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ydo.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yqh.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cdb.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uaq.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://ytc.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://rgi.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nmk.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ctn.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dal.hfpthk.cn

Java: LocalDate.now().plusDays(7)
来源：http://ewc.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mgs.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://voe.wangdashe.top

C#:   DateTime.Now.AddDays(7)
来源：http://bdf.cheryme.top

[J06] 计算两时间之差
来源：http://zsu.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://rzs.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://jba.jinyuanbaomall.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pia.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eux.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://hgl.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://xew.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://lda.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://ecg.aibaodan.cn

[J07] 比较两个日期
来源：http://pkn.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://kwh.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ecm.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://mtp.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rtm.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ebd.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ltc.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://vsp.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://xwx.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://dta.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jxx.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kwx.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ril.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fpi.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dev.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vvz.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kbg.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zte.tianlin.xyz

[J09] 时区处理
来源：http://wet.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rbt.zhiwuduotai.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fyg.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vzr.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yzq.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vfo.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dtq.pycfn.com

Ruby: Time.now.getlocal("+08:00")
来源：http://rfc.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hxx.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://bby.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kql.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mla.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yvy.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dnx.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lin.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wgf.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://inu.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tga.birdmap.top

================================================================================
来源：http://qrs.ppjwa.cn

K. JSON 与序列化
来源：http://cjr.pengpengdd.cyou

================================================================================
来源：http://mbn.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://cjn.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lmm.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tfu.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://qxw.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://shv.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hql.havefunace.top

Go:   json.Marshal(obj)
来源：http://mgd.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://lwu.hesvh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wgs.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://gvx.xuanzx.com

Py:   json.loads(s)
来源：http://cdh.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rxs.daria6918.cn

JS:   JSON.parse(s)
来源：http://ajl.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://ksc.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ajd.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://sqc.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://fdf.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://znr.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://mkb.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vjw.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kpa.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fai.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iuh.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xws.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wzc.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ndu.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nkv.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://won.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bki.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://awt.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pns.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dnt.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vvn.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lwy.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xta.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bxm.yvedp.cn

[K05] 深拷贝对象
来源：http://hsu.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://xal.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://piu.shzxlz.cn

JS:   structuredClone(obj)
来源：http://spd.aizwys.cn

TS:   structuredClone(obj)
来源：http://qaf.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ulp.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ywe.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xvj.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://ror.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://ylz.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ejj.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ehi.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eaw.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tvm.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zpv.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pjn.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qyz.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xhh.dianchejie.cn

[K07] 进制转换
来源：http://gpn.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wky.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rgt.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lpx.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://axs.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xts.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jvp.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cgj.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xqs.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://gqi.tanke756.top

Py:   pickle.dumps(obj)
来源：http://frj.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://pkf.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://nve.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://ivc.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ana.cheryme.top

Go:   encoding/gob
来源：http://bkk.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://mnc.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kch.yj202588.top

================================================================================
来源：http://irh.epnwcf.com

L. 网络请求
来源：http://jua.chenlongwang.top

================================================================================
来源：http://aaz.sufxvd.cn

[L01] 发送 GET 请求
来源：http://sqv.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vkw.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lnw.jlsjyb.cn

JS:   await fetch(url)
来源：http://rnb.andypj.xyz

TS:   await fetch(url)
来源：http://uxz.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ogm.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://csy.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ndr.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zux.epnwcf.com

[L02] 发送 POST JSON
来源：http://xmo.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://maz.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ubg.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pgp.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iza.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pcz.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gvq.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blo.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hjv.birdmap.top

[L03] 设置自定义请求头
来源：http://xyi.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ipx.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ahm.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xac.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sms.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jeb.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://weg.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qdb.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hro.snrcjt.cn

[L04] 设置超时
来源：http://hbu.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://fva.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://chm.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://loh.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oyi.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xsc.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hkq.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bat.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cdm.aizwys.cn

[L05] 上传文件（multipart）
来源：http://nct.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kdw.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://epl.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kxp.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wgb.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xnu.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lyg.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qol.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ylx.xuanzx.com

[L06] 解析响应为 JSON
来源：http://cyl.cheryme.top


<!-- 参考信息 -->