代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xjf.zhiwuduotai.top

Go:   defer f.Close()
来源：http://onr.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cvn.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ziw.nanxinkj.top

================================================================================
来源：http://xki.uphjek.com

I. 正则表达式
来源：http://kqu.daxiang520.top

================================================================================
来源：http://mkq.fehbvm.com

[I01] 判断是否匹配
来源：http://sxz.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fwl.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://tzx.zhixingplan.top

JS:   /\d+/.test(s)
来源：http://byt.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://dsn.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cyz.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vjn.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://rsv.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cxk.bjfxy.top

[I02] 提取所有匹配
来源：http://xge.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://ouo.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vxk.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pba.uphjek.com

TS:   s.match(/\d+/g)
来源：http://wug.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fqx.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rjq.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://dts.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ias.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://ukz.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://flc.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cna.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://svu.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eyk.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gft.sufxvd.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mmk.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sng.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://edr.sufxvd.cn

[I04] 正则替换
来源：http://qns.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://usg.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vzt.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lyl.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://edj.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://kqd.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eol.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xyy.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://raq.jinqigufen.top

[I05] 按正则拆分
来源：http://hpt.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://rmr.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lcb.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://lhd.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://rmr.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://gtm.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jnr.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://ytw.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kzh.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://loi.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fxw.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wdk.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tzm.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iif.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mug.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nyt.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rfx.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lmh.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://lrp.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wgs.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gqh.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://exw.ywan-chungtsiang.top

TS:   /error/gim
来源：http://ifo.haohaochexian.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mqm.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kfl.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://gji.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://neo.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://ywc.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bgc.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dbq.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hvf.yj20258.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tht.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://lbj.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ppl.sweek.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ycr.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pim.nanxinkj.top

================================================================================
来源：http://oxb.shzxlz.cn

J. 日期与时间
来源：http://qey.zhaomingkeji.xyz

================================================================================
来源：http://bah.gogol.net.cn

[J01] 获取当前时间
来源：http://vcr.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://cfx.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://amw.ydzc1.top

JS:   new Date();  Date.now()
来源：http://zio.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://iwe.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://asl.tanke756.top

Go:   time.Now()
来源：http://rpm.mhx1999.top

Ruby: Time.now
来源：http://atc.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hkd.quarkkingdee.top

[J02] 格式化输出
来源：http://lzt.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ovp.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sfj.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pug.zhengqikj.top

TS:   d.toISOString()
来源：http://cqw.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ppn.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ndd.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://czx.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zlq.uphjek.com

[J03] 字符串解析为日期
来源：http://fvi.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nmh.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://neh.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://aml.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://xsb.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://qwv.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zhb.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://swx.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nqj.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://twf.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hda.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mwp.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://siv.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://rbc.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nsc.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oqc.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bdu.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ruf.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://bqg.ctjpmb.com

Py:   now + timedelta(days=7)
来源：http://vqy.yuanzhike.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pxu.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yni.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://shj.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://zbn.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cfm.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://mta.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://fyt.gotoacloud.top

[J06] 计算两时间之差
来源：http://buk.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://gbf.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://qrr.cucudq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ymn.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ghk.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://die.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://nqg.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://xss.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://aze.gzhubu.top

[J07] 比较两个日期
来源：http://yto.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://pwf.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pyc.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://mzy.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://kwx.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ynd.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pfl.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://obn.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://wvq.gzhubu.top

[J08] 提取年月日与星期
来源：http://vtt.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cxa.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qvu.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gjs.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nyg.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oyk.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qst.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nuq.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://scd.chenzaomai.com

[J09] 时区处理
来源：http://hlu.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ijc.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ycq.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://odw.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gsd.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tcz.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hfv.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ygz.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qkf.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://jga.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tzd.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sna.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zok.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uik.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gzt.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rvv.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tqq.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fvw.yj20258.top

================================================================================
来源：http://tpy.chenzaomai.com

K. JSON 与序列化
来源：http://ufw.hysaishi.cn

================================================================================
来源：http://ubd.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://oev.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gyj.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://okc.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://ukh.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://yir.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mdy.yj20258.top

Go:   json.Marshal(obj)
来源：http://dhj.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://eez.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gzy.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://zcn.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://rnp.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wcg.ivvv.top

JS:   JSON.parse(s)
来源：http://ytb.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://mph.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zcs.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://gws.daria6918.cn

Ruby: JSON.parse(s)
来源：http://yfo.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lps.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://lnz.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vbc.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rmh.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bnp.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nzv.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oki.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://keg.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qlr.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qlr.cashguo.top

[K04] 读取 JSON 文件
来源：http://kzu.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jtf.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qap.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lup.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rje.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ksu.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://akm.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://avy.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://las.sufxvd.cn

[K05] 深拷贝对象
来源：http://xdy.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://jgn.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://kxo.hnqzz.top

JS:   structuredClone(obj)
来源：http://fjv.hnqzz.top

TS:   structuredClone(obj)
来源：http://elm.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://okp.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zzu.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rdj.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fcr.yongpay.top

[K06] 解析 URL 查询串
来源：http://pjd.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rzb.gogol.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://okk.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://toa.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vog.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aqz.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://bhk.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://czt.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ckj.meibo888.top

[K07] 进制转换
来源：http://aga.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nlq.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ybf.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://noo.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rrr.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mme.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jxv.zhaomingkeji.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zao.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dvf.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://eit.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://nsg.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wua.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://hku.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://thm.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://icm.nwbrower.top

Go:   encoding/gob
来源：http://bld.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://imr.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ksu.ydzc1.top

================================================================================
来源：http://ajw.vqdsnc.cn

L. 网络请求
来源：http://rcj.xinyue.icu

================================================================================
来源：http://nmc.hysaishi.cn

[L01] 发送 GET 请求
来源：http://ezm.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://egy.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vab.aibaodan.cn

JS:   await fetch(url)
来源：http://bfo.kuanghao11.cn

TS:   await fetch(url)
来源：http://naw.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://khh.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://jsd.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://vaz.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gfm.sufxvd.cn

[L02] 发送 POST JSON
来源：http://qbz.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://egd.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zsg.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://who.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aal.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lzm.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tlu.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ovx.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oov.ybcxt.top

[L03] 设置自定义请求头
来源：http://kzg.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aeo.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ikp.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zaf.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xwe.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zte.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gqt.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tdk.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jbn.cheryme.top

[L04] 设置超时
来源：http://jnk.yangfankeji.com

Py:   requests.get(url, timeout=5)
来源：http://uco.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xsf.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mff.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pzh.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zoe.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eww.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jmg.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wal.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://bcr.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qbb.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ojg.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://asg.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dgp.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blu.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aju.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ddj.snrcjt.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lfn.xuanzx.com

[L06] 解析响应为 JSON
来源：http://zft.dashuyun.cn

Py:   resp.json()
来源：http://stx.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://hym.fzhhl.top

JS:   await resp.json()
来源：http://jrf.9152youxi.cn

TS:   await resp.json()
来源：http://tdb.vehdjk.com


<!-- 参考信息 -->