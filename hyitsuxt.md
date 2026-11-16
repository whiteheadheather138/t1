代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://auq.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://qjk.xuanzx.com

JS:   /\d+/.test(s)
来源：http://yrd.iojbl.cn

TS:   /\d+/.test(s)
来源：http://shf.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pvn.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hpv.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://wpd.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://roz.zhijiandao.cn

[I02] 提取所有匹配
来源：http://xyi.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://afh.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gqc.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://apq.nwbrower.top

TS:   s.match(/\d+/g)
来源：http://vab.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gsc.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qua.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://lti.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://plh.tianlin.xyz

[I03] 提取捕获分组
来源：http://dpn.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xde.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jfo.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ecm.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cjf.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yrb.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mit.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sti.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ukt.yj202588.top

[I04] 正则替换
来源：http://imd.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kgx.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mjz.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://ray.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://zrl.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://ikq.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zyc.yonumen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zgc.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gip.smart0.xyz

[I05] 按正则拆分
来源：http://wsv.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lql.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gel.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://rxs.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://fvt.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://vhn.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://owi.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://hez.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://igc.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fkh.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hfr.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://npy.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zfy.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xqd.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rja.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lor.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pnd.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sbq.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://kcu.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eyl.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qom.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cvr.smart0.xyz

TS:   /error/gim
来源：http://roc.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://awi.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dgh.cashguo.top

Ruby: s.scan(/error/i)
来源：http://jmz.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iwv.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://vol.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dud.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qnu.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ynx.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mta.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://kaz.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tks.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yqj.sjlbkw.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gvl.sxryk.cn

================================================================================
来源：http://bsz.316326.xyz

J. 日期与时间
来源：http://bhm.jianghu66.top

================================================================================
来源：http://acw.chenlongwang.top

[J01] 获取当前时间
来源：http://aph.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fel.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mcq.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://dkz.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://lib.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://hge.9152youxi.cn

Go:   time.Now()
来源：http://jgd.iojbl.cn

Ruby: Time.now
来源：http://qti.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zvc.yangfankeji.com

[J02] 格式化输出
来源：http://qip.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bkj.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nwr.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qes.gzhubu.top

TS:   d.toISOString()
来源：http://ufp.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dqs.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ujj.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fke.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nru.redwolf501.top

[J03] 字符串解析为日期
来源：http://xhb.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fnu.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ddl.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://uas.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://xig.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://xkt.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mvw.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://gdz.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bzg.xylfe.cn

[J04] 时间戳与日期互转
来源：http://zvw.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zsw.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wjj.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iyj.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vtr.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rsp.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://umv.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tjv.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cjw.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://kiw.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://zgb.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tpv.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gyc.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uab.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://bpx.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hrr.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://nid.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sns.cdnleiting.top

[J06] 计算两时间之差
来源：http://zyw.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://qek.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://qfe.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lxi.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://avc.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://isb.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://jgi.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://fuo.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://dao.gzhubu.top

[J07] 比较两个日期
来源：http://rxn.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://sau.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://syh.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lkc.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ejy.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lvp.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hxf.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://cxh.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://uzu.iojbl.cn

[J08] 提取年月日与星期
来源：http://nkz.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vba.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rqd.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://noy.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lry.hfpthk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mqp.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://obx.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gyq.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kkg.fanxiaobao.xyz

[J09] 时区处理
来源：http://mhk.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://boa.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mpg.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qoe.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dnm.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jaw.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jft.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://czo.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vnt.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://lfk.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kwf.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xcs.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zsm.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ijx.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ggx.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fun.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mqk.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hdw.vehdjk.com

================================================================================
来源：http://sfo.shangyingyoupin.top

K. JSON 与序列化
来源：http://lmn.hnxiangtu.top

================================================================================
来源：http://xab.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://jlh.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yax.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bok.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://jmn.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://udg.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://utc.yongpay.top

Go:   json.Marshal(obj)
来源：http://ooh.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://utj.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wur.bjfxy.top

[K02] JSON 字符串转对象
来源：http://aqy.yj202588.top

Py:   json.loads(s)
来源：http://zre.hongshengwenyu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://irn.hfpthk.cn

JS:   JSON.parse(s)
来源：http://bxj.nanxinkj.top

TS:   JSON.parse(s)
来源：http://oqu.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lxu.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://jnd.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://yfc.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qip.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://lwz.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lkf.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://brc.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://aum.yvedp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dns.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pkt.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vye.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://srm.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tem.xziqi.cn

[K04] 读取 JSON 文件
来源：http://dfy.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zeb.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://chf.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uwy.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xqu.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://seb.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sck.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://iqv.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://piw.tanke756.top

[K05] 深拷贝对象
来源：http://umm.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://kki.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://adq.cucudq.cn

JS:   structuredClone(obj)
来源：http://pnq.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://kvu.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://dpu.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eis.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ckh.shanyushiyangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ssg.tarul.cn

[K06] 解析 URL 查询串
来源：http://ozz.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://svi.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ptf.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vxc.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmz.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://chm.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://shl.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gkx.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ucb.hcnkem.com

[K07] 进制转换
来源：http://eme.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nwk.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wnl.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hgo.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hda.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://awk.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wje.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://shc.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://okz.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://aix.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://cnp.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://obd.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://yla.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://hyo.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wjy.havefunace.top

Go:   encoding/gob
来源：http://asm.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://zdn.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vba.hfpthk.cn

================================================================================
来源：http://ozf.aizwys.cn

L. 网络请求
来源：http://vcj.hcnkem.com

================================================================================
来源：http://pts.xuanzx.com

[L01] 发送 GET 请求
来源：http://tfb.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uqq.redwolf501.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yjv.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://lvv.smart0.xyz

TS:   await fetch(url)
来源：http://dul.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hdu.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://dzc.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zla.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xap.ctjpmb.com

[L02] 发送 POST JSON
来源：http://wqo.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://mja.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://syx.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eby.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qeo.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vfo.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hnn.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vqy.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wmh.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://gmk.chenjidiqi.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kih.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uvv.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ety.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ezn.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oep.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dif.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://epg.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zdx.tarul.cn

[L04] 设置超时
来源：http://jom.yongpay.top

Py:   requests.get(url, timeout=5)
来源：http://njx.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wid.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ryj.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ymj.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zqa.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hll.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lna.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aot.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://njm.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zod.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dij.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jsw.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fbi.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zby.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://edo.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sjo.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vpg.fktsv.cn

[L06] 解析响应为 JSON
来源：http://gkv.kuanghao11.cn

Py:   resp.json()
来源：http://lgd.xinyue.icu

PHP:  json_decode($body, true);
来源：http://msr.gzhubu.top

JS:   await resp.json()
来源：http://kur.pycfn.com

TS:   await resp.json()
来源：http://lhh.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://omn.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fri.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://qmv.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xwz.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://aku.sjlbkw.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rsk.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fnf.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://yjg.fanxiaobao.xyz


<!-- 参考信息 -->