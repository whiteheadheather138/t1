代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rsg.fktsv.cn

Go:   defer f.Close()
来源：http://xeh.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://klh.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qrg.sxryk.cn

================================================================================
来源：http://ezi.bjfxy.top

I. 正则表达式
来源：http://poz.jlsjyb.cn

================================================================================
来源：http://urz.ybcxt.top

[I01] 判断是否匹配
来源：http://jwv.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://grf.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://yze.tanke756.top

JS:   /\d+/.test(s)
来源：http://yza.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://ide.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zfx.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rux.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://kcu.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xya.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://ahk.pengpengdd.cyou

Py:   re.findall(r"\d+", s)
来源：http://mqb.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pmw.chenjidiqi.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uht.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://fkf.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lvo.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qbj.shanyushiyangkeji.top

Ruby: s.scan(/\d+/)
来源：http://jpm.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nlp.daxiang520.top

[I03] 提取捕获分组
来源：http://hum.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vgu.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zmx.52xcode.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ucz.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://crb.jqgfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fbs.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sfh.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rmn.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iyv.havefunace.top

[I04] 正则替换
来源：http://fmp.cdnleiting.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ovx.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gbs.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fih.zhaomingkeji.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://zza.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://gml.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zpn.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bps.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uju.dashuyun.cn

[I05] 按正则拆分
来源：http://jki.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pso.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uqt.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://ith.andypj.xyz

TS:   s.split(/\s*,\s*/)
来源：http://jhj.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://inw.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://etc.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://top.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ntf.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rnh.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mok.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pvg.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ier.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pvs.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wwz.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xcd.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ayh.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nec.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://euy.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://inq.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://znu.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://whd.snrcjt.cn

TS:   /error/gim
来源：http://jbi.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iig.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qdd.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://hiv.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://shb.zhengqikj.top

[I08] 贪婪与非贪婪匹配
来源：http://xdd.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ywz.epnwcf.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://asg.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nty.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bsn.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nko.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://byr.birdmap.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://med.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gcv.cashguo.top

================================================================================
来源：http://kfx.zhongyouzk.top

J. 日期与时间
来源：http://dwv.feifeiyinyue.top

================================================================================
来源：http://rje.zhixingplan.top

[J01] 获取当前时间
来源：http://oha.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mwy.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qbu.andypj.xyz

JS:   new Date();  Date.now()
来源：http://mvl.bjfxy.top

TS:   new Date();  Date.now()
来源：http://god.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gmc.cdnleiting.top

Go:   time.Now()
来源：http://xnw.jiagoushi.top

Ruby: Time.now
来源：http://nxx.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cyg.zhoulong.xyz

[J02] 格式化输出
来源：http://ake.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wdf.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://app.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hnd.jyoumei.cn

TS:   d.toISOString()
来源：http://yvm.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xxi.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dlv.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vtv.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tua.hcnkem.com

[J03] 字符串解析为日期
来源：http://kci.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xgx.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://duy.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://yqd.sweek.top

TS:   new Date("2024-01-02")
来源：http://etp.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wos.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wsu.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://jjs.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ohr.cashguo.top

[J04] 时间戳与日期互转
来源：http://szi.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uyi.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aqo.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dyp.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vws.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ath.daxiang520.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hjq.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cqa.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://moo.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://taq.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://vgc.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ilv.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rox.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kpa.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://caw.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yyu.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://kfp.0kj1m.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jwq.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://ete.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://huq.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://tdn.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hbd.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dxt.fktsv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kud.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://pte.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://xxp.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://hwo.smart0.xyz

[J07] 比较两个日期
来源：http://lnp.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://tly.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mxv.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://hiu.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://izp.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tgf.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ljn.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://idx.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://oxd.fehbvm.com

[J08] 提取年月日与星期
来源：http://svt.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eoz.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bly.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xig.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bvs.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lhl.tianlin.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hfy.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vqv.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wbr.zhaomingkeji.xyz

[J09] 时区处理
来源：http://ooz.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zkg.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jjs.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://she.xuanzx.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hkk.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://crn.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lhg.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://uce.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tgr.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://ypd.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xhb.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fei.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fty.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kgn.jqgfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mys.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://btp.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bva.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ktv.9152youxi.cn

================================================================================
来源：http://ame.fanxiaobao.xyz

K. JSON 与序列化
来源：http://arq.pengpengdd.cyou

================================================================================
来源：http://prb.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://qxf.gotoacloud.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jyi.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ywc.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://tmr.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://pkb.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ipc.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://zgq.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ify.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cel.aizwys.cn

[K02] JSON 字符串转对象
来源：http://xbs.cashguo.top

Py:   json.loads(s)
来源：http://ckx.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zlf.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://mjq.daria6918.cn

TS:   JSON.parse(s)
来源：http://lci.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fzs.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://qbf.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://ytt.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pvn.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://qqw.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tdz.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qvn.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://znq.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://phk.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nmt.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fjg.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aeu.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wsu.fengsongda.top

[K04] 读取 JSON 文件
来源：http://kof.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vwe.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bmg.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lfo.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://drf.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zyr.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ick.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rgz.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://euu.chenzaomai.com

[K05] 深拷贝对象
来源：http://rgn.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://siz.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://fnu.yangfankeji.com

JS:   structuredClone(obj)
来源：http://mrz.yangfankeji.com

TS:   structuredClone(obj)
来源：http://olo.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://uay.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aqh.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qio.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://guw.aibaodan.cn

[K06] 解析 URL 查询串
来源：http://yyt.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ael.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hio.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cze.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uao.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kkl.vqdsnc.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rcf.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zgv.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zcj.bbcook.cn

[K07] 进制转换
来源：http://zcp.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vjt.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mgk.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lfu.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pnn.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fbs.mhx1999.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mzq.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zxk.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zvn.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://goq.yonumen.top

Py:   pickle.dumps(obj)
来源：http://kbr.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xqe.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://wwr.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://qxw.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kuj.pengpengdd.cyou

Go:   encoding/gob
来源：http://enk.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://yok.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://npf.hnxiangtu.top

================================================================================
来源：http://zwy.bjfxy.top

L. 网络请求
来源：http://dzc.yvedp.cn

================================================================================
来源：http://crd.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://aaq.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uyi.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pzz.jqgfzy.top

JS:   await fetch(url)
来源：http://qyj.9152youxi.cn

TS:   await fetch(url)
来源：http://vdb.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://poa.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://ijw.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sqd.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kqg.yongpay.top

[L02] 发送 POST JSON
来源：http://xmd.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wzp.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ijs.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nuf.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvp.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nar.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ewv.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yar.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dyr.xylfe.cn

[L03] 设置自定义请求头
来源：http://irk.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gmn.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ibz.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fuf.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pez.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tfr.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vqq.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cjb.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vlo.gaohongyu789.top

[L04] 设置超时
来源：http://rrd.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://epf.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://saf.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hkf.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://roi.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kox.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://plq.yfazqb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zru.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tvo.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://uly.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lrq.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ikg.iojbl.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ldq.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kpn.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ytp.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ebp.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lpx.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mto.daria6918.cn

[L06] 解析响应为 JSON
来源：http://pfu.chenjidiqi.icu

Py:   resp.json()
来源：http://dou.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://iif.shzxlz.cn

JS:   await resp.json()
来源：http://vhe.haohaochexian.top

TS:   await resp.json()
来源：http://etf.jianghu66.top


<!-- 参考信息 -->