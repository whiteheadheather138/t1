代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tem.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://jrj.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://izu.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://jav.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sos.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nas.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://qsd.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vdi.shzxlz.cn

[I02] 提取所有匹配
来源：http://nox.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://urf.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://psn.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bkj.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://tpz.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://isw.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dxd.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://tlf.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rts.52xcode.cn

[I03] 提取捕获分组
来源：http://ubh.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tef.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jua.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bpo.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wdr.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://azs.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uxz.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jaj.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uaq.shanyushiyangtech.top

[I04] 正则替换
来源：http://uxm.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yow.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rrb.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://jnn.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://jyo.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uvd.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://apa.sjlbkw.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qji.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://glh.sxryk.cn

[I05] 按正则拆分
来源：http://pzq.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://peg.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wzo.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://otr.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://erl.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://dlt.daxiang520.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ypr.guannengcc.top

Ruby: s.split(/\s*,\s*/)
来源：http://sne.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pag.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dvb.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pah.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zhw.ivvv.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://flr.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hgt.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jmm.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sjj.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oco.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fsy.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://ihj.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ccd.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vvh.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://htw.hammf.cn

TS:   /error/gim
来源：http://ogg.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kkz.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uxr.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://szg.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lpk.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://yon.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rcd.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lmo.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xdt.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oge.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://syv.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://grm.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gqn.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bxo.yj20258888.top

================================================================================
来源：http://qbp.iojbl.cn

J. 日期与时间
来源：http://kho.9152youxi.cn

================================================================================
来源：http://gjg.nanxuanxn.top

[J01] 获取当前时间
来源：http://wot.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://iux.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rxn.mhx1999.top

JS:   new Date();  Date.now()
来源：http://tug.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://ttn.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://pqn.fzhhl.top

Go:   time.Now()
来源：http://zjx.svipenyu.cn

Ruby: Time.now
来源：http://yem.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wif.yuxming.cn

[J02] 格式化输出
来源：http://uli.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ecs.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wmq.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gjh.tanke756.top

TS:   d.toISOString()
来源：http://sit.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ees.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rdj.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eru.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mbt.yueranfly.top

[J03] 字符串解析为日期
来源：http://vrc.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bvx.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ayf.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://asn.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://jql.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://toi.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://scf.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://dmz.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rar.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://qqj.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jfr.9152youxi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ske.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://avw.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pad.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ewn.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bwh.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ojy.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fvr.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://zlj.tanke756.top

Py:   now + timedelta(days=7)
来源：http://hmp.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mvx.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gfc.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mhe.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://jga.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mdg.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://ssi.hongshengwenyu.top

C#:   DateTime.Now.AddDays(7)
来源：http://atw.ydjk.org.cn

[J06] 计算两时间之差
来源：http://dwf.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://quw.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://iys.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kzm.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ahf.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://lqf.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://wjg.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://qet.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://yoj.xuanzx.com

[J07] 比较两个日期
来源：http://zzc.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://ywp.52xcode.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://afu.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lkm.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://slb.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uaw.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hky.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://wte.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://nhu.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://mbs.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dwb.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bhe.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wve.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://esg.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dvc.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uha.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xvu.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wtz.jiagoushi.top

[J09] 时区处理
来源：http://pmq.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hrx.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lwf.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zvh.meibo888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hqm.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://onc.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uvv.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wzd.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jty.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://qhs.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sfw.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jpw.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nqe.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yqi.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://har.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://phg.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rpu.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rmj.birdmap.top

================================================================================
来源：http://uxg.uphjek.com

K. JSON 与序列化
来源：http://ygi.xuetiantiany.cn

================================================================================
来源：http://qmm.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://tbv.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://and.c1oappe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ikj.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://cij.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://hnq.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ogr.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://nna.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://xll.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zxq.epnwcf.com

[K02] JSON 字符串转对象
来源：http://dpr.birdmap.top

Py:   json.loads(s)
来源：http://ova.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xpd.dashuyun.cn

JS:   JSON.parse(s)
来源：http://njm.ctjpmb.com

TS:   JSON.parse(s)
来源：http://ftm.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nsd.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://mwc.fehbvm.com

Ruby: JSON.parse(s)
来源：http://puv.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://agd.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://xdt.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kuk.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zxb.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jkt.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jtc.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ref.snrcjt.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xnn.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nbp.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pog.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://fzd.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lgf.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fmv.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hdy.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iur.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cdq.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dxf.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gfo.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gig.sxryk.cn

[K05] 深拷贝对象
来源：http://etu.zhixingplan.top

Py:   copy.deepcopy(obj)
来源：http://axy.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://sqg.ehwqpu.com

JS:   structuredClone(obj)
来源：http://kci.smart0.xyz

TS:   structuredClone(obj)
来源：http://vqf.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ery.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lme.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xzn.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hbz.xinyue.icu

[K06] 解析 URL 查询串
来源：http://oyh.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qib.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zpi.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ami.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://abp.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ltz.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xhm.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mwf.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://edt.shanyushiyangkeji.top

[K07] 进制转换
来源：http://pxf.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nzg.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cxy.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://puc.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kep.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rld.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ggv.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bfx.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hjf.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://xuv.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://kji.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yju.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://vyc.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://cso.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://clr.sjlbkw.cn

Go:   encoding/gob
来源：http://rbd.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://rsy.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ukm.hfpthk.cn

================================================================================
来源：http://puu.gotoacloud.top

L. 网络请求
来源：http://mnf.yonumen.top

================================================================================
来源：http://fit.zhengqikj.top

[L01] 发送 GET 请求
来源：http://wyc.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://agd.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zmr.cheryme.top

JS:   await fetch(url)
来源：http://qfk.cheryme.top

TS:   await fetch(url)
来源：http://svr.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bsd.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://dop.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://pow.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zps.zhijiandao.cn

[L02] 发送 POST JSON
来源：http://avn.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://evr.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://koi.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fxn.fehbvm.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mtc.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://frr.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://czg.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eje.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gxl.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://gjx.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jgw.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://grb.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vdf.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cvg.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kfs.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vlx.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zdy.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tjx.jqgfzy.top

[L04] 设置超时
来源：http://uzw.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://gbo.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sye.cqqwz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bac.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://osj.nanxuanxn.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ipk.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yvn.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mtn.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nwu.xinyue.icu

[L05] 上传文件（multipart）
来源：http://dat.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://unl.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gcd.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jzd.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://omt.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jrc.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mtg.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dlg.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dhs.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://mhu.chenlongwang.top

Py:   resp.json()
来源：http://hko.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://ngv.cqqwz.cn

JS:   await resp.json()
来源：http://dtc.yonumen.top

TS:   await resp.json()
来源：http://qag.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jdt.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://syx.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://zep.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fnr.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://ynr.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cyr.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xml.jlsjyb.cn

JS:   resp.ok;  resp.status
来源：http://guf.fanxiaobao.xyz


<!-- 参考信息 -->