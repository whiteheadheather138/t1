代发 wailian999

TS:   s.match(/\d+/g)
来源：http://adi.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hzd.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sbz.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://vck.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xwq.mhx1999.top

[I03] 提取捕获分组
来源：http://bvl.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nfq.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iyj.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jsc.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://skv.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ejl.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fdm.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ewq.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cif.guannengcc.top

[I04] 正则替换
来源：http://hot.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pxi.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sch.zhengqikj.top

JS:   s.replace(/\d+/g, "#")
来源：http://aer.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://ibi.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://fqv.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bhy.zdbjq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rvj.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gus.shuidangran.top

[I05] 按正则拆分
来源：http://tyo.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ula.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ceo.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://cum.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://gtq.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://aog.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://maa.yuanzhike.top

Ruby: s.split(/\s*,\s*/)
来源：http://gyj.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aqj.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jnv.nanxuanxn.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://imn.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tss.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kvt.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ukj.fengsongda.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iow.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ujl.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xrf.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nmp.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://tui.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fgg.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ezt.ydzc1.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cke.yanxiufei.cn

TS:   /error/gim
来源：http://ftr.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bpt.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bzc.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://vrz.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vlf.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://pgo.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vgi.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zxn.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mgc.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jpl.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://upn.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pjg.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bfs.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kug.tianlin.xyz

================================================================================
来源：http://knr.xuanzx.com

J. 日期与时间
来源：http://afn.birdmap.top

================================================================================
来源：http://agg.xylfe.cn

[J01] 获取当前时间
来源：http://ikl.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://blo.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fsl.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://iia.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://atg.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zmv.redwolf501.top

Go:   time.Now()
来源：http://cej.yfazqb.com

Ruby: Time.now
来源：http://iak.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dxl.fzhhl.top

[J02] 格式化输出
来源：http://vrw.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tma.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bvt.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://elv.yj202588.top

TS:   d.toISOString()
来源：http://tcm.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dhe.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pls.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zww.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oqf.mhx1999.top

[J03] 字符串解析为日期
来源：http://veo.smart0.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://feq.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ypp.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://rws.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://try.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://slp.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vcu.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://vxf.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ygj.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://gvj.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ncm.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qpe.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jgg.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kkq.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gqv.fanxiaobao.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gcn.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://urn.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://aor.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://qmy.yuxming.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xxv.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pkk.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cwj.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://vix.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ayh.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://mbb.aibaodan.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xrz.zhengqikj.top

[J06] 计算两时间之差
来源：http://ysj.jqgufenzy.top

Py:   (end - start).total_seconds()
来源：http://inx.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://gfa.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yem.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ucp.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hjv.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://yez.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://hrk.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://hxi.zycfv.cn

[J07] 比较两个日期
来源：http://vsm.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://kjb.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kzh.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mfh.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://wio.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://izh.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tvr.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://tiy.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://ksh.nanxinkj.top

[J08] 提取年月日与星期
来源：http://ndf.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gou.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ner.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iyb.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bsi.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pet.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zku.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oij.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://svm.jinyuanbaomall.cn

[J09] 时区处理
来源：http://vff.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://llh.yj202588.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xcp.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fvn.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vtp.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://glr.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aef.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://guq.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nkd.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://kop.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://bhz.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xje.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fsa.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qop.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wfn.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kxe.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hdz.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xkd.svipenyu.cn

================================================================================
来源：http://qxz.birdmap.top

K. JSON 与序列化
来源：http://jfk.hnxiangtu.top

================================================================================
来源：http://uvk.vehdjk.com

[K01] 对象转 JSON 字符串
来源：http://ovz.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vyz.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qtg.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://luj.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://srh.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ian.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://dqv.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://xsf.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qix.xziqi.cn

[K02] JSON 字符串转对象
来源：http://ibx.gzhubu.top

Py:   json.loads(s)
来源：http://ekc.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ail.smart0.xyz

JS:   JSON.parse(s)
来源：http://vst.haohaochexian.top

TS:   JSON.parse(s)
来源：http://qen.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ljp.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://tho.cashguo.top

Ruby: JSON.parse(s)
来源：http://rdw.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bzg.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://jtj.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ebo.daxiang520.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vay.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xnm.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nrd.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://whv.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xxt.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://qum.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://szq.guannengcc.top

[K04] 读取 JSON 文件
来源：http://eis.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rjt.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gvw.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yma.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rex.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xdu.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tgo.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bqd.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uje.tanke756.top

[K05] 深拷贝对象
来源：http://axn.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://omo.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://ple.xylfe.cn

JS:   structuredClone(obj)
来源：http://zoo.vehdjk.com

TS:   structuredClone(obj)
来源：http://umk.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://mcj.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vpx.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ggs.yj20258888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nup.andypj.xyz

[K06] 解析 URL 查询串
来源：http://zjg.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vno.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ygk.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppd.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wnd.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://grb.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://quc.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xvg.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fkx.hcnkem.com

[K07] 进制转换
来源：http://mxa.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://abu.xuetiantiany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kjq.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wix.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zic.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kvo.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cqb.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nrj.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://add.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://bvn.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://iqz.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://orp.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://cmt.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://zqc.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vrr.gaohongyu789.top

Go:   encoding/gob
来源：http://saf.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://azi.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bgf.yj202588.top

================================================================================
来源：http://bab.tanke756.top

L. 网络请求
来源：http://nbn.sxryk.cn

================================================================================
来源：http://jzp.bjfxy.top

[L01] 发送 GET 请求
来源：http://xxo.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oyw.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yqt.pengpengdd.cyou

JS:   await fetch(url)
来源：http://vqw.fehbvm.com

TS:   await fetch(url)
来源：http://ojj.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ikh.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://pcg.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vos.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ybx.yj20258.top

[L02] 发送 POST JSON
来源：http://sbi.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://adj.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xdt.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lxi.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://duz.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mtg.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zuz.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://soq.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sce.yj202588.top

[L03] 设置自定义请求头
来源：http://dym.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jqn.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://krv.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xvc.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jpd.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oev.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zpo.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ekz.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mqe.zhongyouzk.top

[L04] 设置超时
来源：http://ggy.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://zkg.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ber.jqgfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ldd.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oxa.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mbn.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://shn.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yqt.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rcq.fktsv.cn

[L05] 上传文件（multipart）
来源：http://hql.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pwr.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oyq.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://knn.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eyz.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mwu.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tzl.jqgfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bpy.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xrn.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://ems.shanyushiyangkeji.top

Py:   resp.json()
来源：http://jau.tanke756.top

PHP:  json_decode($body, true);
来源：http://xor.birdmap.top

JS:   await resp.json()
来源：http://wwj.yj20258.top

TS:   await resp.json()
来源：http://yuk.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://viz.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zuu.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://ity.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lkp.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://whh.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://crx.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rye.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://axa.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://tnz.zhiwuduotai.top

Java: resp.statusCode()
来源：http://qnq.fktsv.cn

Go:   resp.StatusCode
来源：http://yqk.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://ztl.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://ypd.fktsv.cn

[L08] 并发请求多个地址
来源：http://rrh.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sgc.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://eig.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xdy.jianghu66.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://emd.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ayf.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tbb.daxiang520.top


<!-- 参考信息 -->