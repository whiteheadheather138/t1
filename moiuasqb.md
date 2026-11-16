代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pmd.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qjw.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://zkq.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://eln.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uvm.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://swm.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://zft.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ciq.fktsv.cn

[I02] 提取所有匹配
来源：http://emp.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://juo.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xep.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iyt.ivvv.top

TS:   s.match(/\d+/g)
来源：http://htq.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lgn.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iat.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://ccw.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iwj.dianchejie.cn

[I03] 提取捕获分组
来源：http://qsc.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wws.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://alh.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://udb.tianlin.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://stk.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pxa.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mkk.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dqb.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://snm.meibo888.top

[I04] 正则替换
来源：http://wzr.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jlg.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rop.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://mbp.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://toj.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://wrl.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zyx.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kcm.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dci.zycfv.cn

[I05] 按正则拆分
来源：http://oxc.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dpn.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gus.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://rzj.yueranfly.top

TS:   s.split(/\s*,\s*/)
来源：http://tyy.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://mvp.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jpa.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://rmr.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ryi.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kcd.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zng.yuanzhike.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mfi.meibo888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mqt.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xfg.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jtt.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lfn.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yqs.aizwys.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ftg.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://ews.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tit.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lin.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uon.aibaodan.cn

TS:   /error/gim
来源：http://njz.zhaomingkeji.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yxp.xuetiantiany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mha.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://nng.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pdf.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://dvz.cashguo.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gtu.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dlx.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wve.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://drb.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dyw.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://apl.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nsh.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aqz.zhoulong.xyz

================================================================================
来源：http://dsx.cucudq.cn

J. 日期与时间
来源：http://mcj.redwolf501.top

================================================================================
来源：http://umy.xinyue.icu

[J01] 获取当前时间
来源：http://ofm.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cuu.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pte.52xcode.cn

JS:   new Date();  Date.now()
来源：http://luj.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://kti.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hgh.shanyushiyangkeji.top

Go:   time.Now()
来源：http://ooy.316326.xyz

Ruby: Time.now
来源：http://cra.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qmj.smart0.xyz

[J02] 格式化输出
来源：http://yqm.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://muj.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vua.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uxf.ydjk.org.cn

TS:   d.toISOString()
来源：http://asi.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ygf.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fnu.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cpq.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://chk.havefunace.top

[J03] 字符串解析为日期
来源：http://qsg.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nnh.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jkd.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://eax.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://jfo.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ntq.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wqx.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://czy.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eyy.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://nzm.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://onk.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kyk.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dlf.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kca.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://knk.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hwu.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nib.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ltk.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://teg.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://mur.vqdsnc.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vlq.ppjwa.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oqf.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zpk.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://skj.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xzo.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://zqc.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://hmn.redwolf501.top

[J06] 计算两时间之差
来源：http://nkx.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://jbx.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://gnf.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zll.cashguo.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fab.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://jci.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://ien.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://bih.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://aml.andypj.xyz

[J07] 比较两个日期
来源：http://dpz.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://hxy.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nmc.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://rgs.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bzt.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://doz.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://amm.iojbl.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bqp.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://qim.9152youxi.cn

[J08] 提取年月日与星期
来源：http://jek.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bgk.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pmc.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vkz.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fxf.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hsv.uphjek.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kky.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jev.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://agc.jianghu66.top

[J09] 时区处理
来源：http://czn.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wyj.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nmf.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ype.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kjf.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ooa.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gks.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://yso.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cqi.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://gig.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://mlk.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mht.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vkm.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://btt.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fkf.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qcc.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oiw.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://txy.ppjwa.cn

================================================================================
来源：http://bhe.yj20258888.top

K. JSON 与序列化
来源：http://kqb.zhijiandao.cn

================================================================================
来源：http://ixu.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://jjz.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vil.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bkw.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://hgd.havefunace.top

TS:   JSON.stringify(obj)
来源：http://vjl.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rmo.ybcxt.top

Go:   json.Marshal(obj)
来源：http://xwn.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://dtc.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hze.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://vdu.gaohongyu789.top

Py:   json.loads(s)
来源：http://ycm.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fgx.redwolf501.top

JS:   JSON.parse(s)
来源：http://ojd.jiagoushi.top

TS:   JSON.parse(s)
来源：http://xlz.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sgm.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ako.wangdashe.top

Ruby: JSON.parse(s)
来源：http://qnd.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wyi.bjfxy.top

[K03] JSON 美化输出（带缩进）
来源：http://vdg.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nsc.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qtd.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://utx.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kmn.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pxm.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wmv.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://hji.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xfh.bjfxy.top

[K04] 读取 JSON 文件
来源：http://lff.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sbq.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://buu.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pnt.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dju.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pld.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rrx.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ezw.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lwq.yj202588.top

[K05] 深拷贝对象
来源：http://cac.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://rfg.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://nht.meibo888.top

JS:   structuredClone(obj)
来源：http://lie.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://kno.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fxy.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://btq.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://crg.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yrz.yj202588.top

[K06] 解析 URL 查询串
来源：http://vfm.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mtl.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://agk.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://meb.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ixa.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bes.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rij.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iys.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ppw.cheryme.top

[K07] 进制转换
来源：http://sfc.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://twz.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ezd.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bmz.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qxj.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sik.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://exs.ydjk.org.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dln.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yjn.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://qsa.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://ipk.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iea.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://kgp.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://ucy.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://biy.ppjwa.cn

Go:   encoding/gob
来源：http://klm.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://hrz.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pqw.yfazqb.com

================================================================================
来源：http://bdn.cucudq.cn

L. 网络请求
来源：http://mfc.tarul.cn

================================================================================
来源：http://wii.gotoacloud.top

[L01] 发送 GET 请求
来源：http://vki.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://itl.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://joj.hywenlv.cn

JS:   await fetch(url)
来源：http://jpv.shuidangran.top

TS:   await fetch(url)
来源：http://owq.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yzz.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://rag.kuanghao11.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mdo.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vss.hesvh.cn

[L02] 发送 POST JSON
来源：http://nmb.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cof.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iam.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gjs.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hml.birdmap.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://usq.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://esf.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fzt.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cao.chenlongwang.top

[L03] 设置自定义请求头
来源：http://uvk.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ezl.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ign.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vbo.sysykeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gqh.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pps.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://njw.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yzp.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wkw.dashuyun.cn

[L04] 设置超时
来源：http://ihx.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://jlh.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qkz.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gdt.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vuj.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://txr.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wbv.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dxd.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vdi.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://ljh.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jyr.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rim.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jln.52xcode.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iwe.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lix.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jev.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://acc.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iie.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://ght.ctjpmb.com

Py:   resp.json()
来源：http://bac.guannengcc.top

PHP:  json_decode($body, true);
来源：http://eyl.chenjidiqi.icu

JS:   await resp.json()
来源：http://hfz.haohaochexian.top

TS:   await resp.json()
来源：http://aql.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eeg.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bem.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://lof.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gza.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://unr.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jsy.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jyl.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://ier.zhaomingkeji.xyz


<!-- 参考信息 -->