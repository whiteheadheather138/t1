代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aaz.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://aju.jianghu66.top

JS:   /\d+/.test(s)
来源：http://fko.birdmap.top

TS:   /\d+/.test(s)
来源：http://huu.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zpf.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aay.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://jmh.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://das.hnxiangtu.top

[I02] 提取所有匹配
来源：http://yda.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://jsh.gzhubu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://muk.iojbl.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://env.redwolf501.top

TS:   s.match(/\d+/g)
来源：http://svb.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://svh.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jff.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://hlf.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hti.fktsv.cn

[I03] 提取捕获分组
来源：http://nef.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pxf.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cby.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://skm.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eoa.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rib.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uhh.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://amv.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vph.cucudq.cn

[I04] 正则替换
来源：http://hkz.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://avs.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qzt.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oma.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ocd.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lfx.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://squ.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://utd.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pij.zdbjq.cn

[I05] 按正则拆分
来源：http://ahp.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mfq.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xfm.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://mvh.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://hcq.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://lpu.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aiw.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://ksv.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lky.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fhg.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rde.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ess.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://few.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zef.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vwe.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dio.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xbp.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://doe.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://lxx.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gwz.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://edl.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jup.xuetiantiany.cn

TS:   /error/gim
来源：http://zbs.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qzu.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yph.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://rwm.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wtk.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://uwl.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kcv.jqgfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vue.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uac.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fln.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oum.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eep.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ffb.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iot.pycfn.com

================================================================================
来源：http://own.redwolf501.top

J. 日期与时间
来源：http://xgk.jqgfzy.top

================================================================================
来源：http://lrv.dianchejie.cn

[J01] 获取当前时间
来源：http://kgd.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://esm.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tua.jianghu66.top

JS:   new Date();  Date.now()
来源：http://nva.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://wob.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xoe.uphjek.com

Go:   time.Now()
来源：http://ayl.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://odh.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jmg.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://ngn.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bqn.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pez.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cyi.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://yar.cqqwz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dzn.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ray.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rce.zhiwuduotai.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ygl.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://sqz.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://odr.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gpk.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://bna.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://kwj.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yqj.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cux.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://fgn.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sdk.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://vwt.yuxming.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://emf.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tio.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ixl.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xll.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://osk.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oss.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jzw.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qrc.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://tah.jinyuanbaomall.cn

Py:   now + timedelta(days=7)
来源：http://zpo.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://vqe.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://odi.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ffp.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://iih.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://irz.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://vfy.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://gpm.zhijiandao.cn

[J06] 计算两时间之差
来源：http://lxj.ivvv.top

Py:   (end - start).total_seconds()
来源：http://xic.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://xjm.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aqa.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uql.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://kpn.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://ykr.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://odm.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://twv.dashuyun.cn

[J07] 比较两个日期
来源：http://duc.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://wii.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://skq.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://rnt.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zrm.shzxlz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pma.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://opn.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://umg.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://rfj.hfpthk.cn

[J08] 提取年月日与星期
来源：http://hnw.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yan.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gnt.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wmi.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gmq.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://niw.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nvj.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://imr.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mwb.gzhubu.top

[J09] 时区处理
来源：http://rxa.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://skf.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ece.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zcq.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://paf.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bvm.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ybp.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dyq.tian-w.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mth.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://bxr.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jdh.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://upc.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://amw.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iwf.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ryj.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xkc.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bmt.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cgr.jiagoushi.top

================================================================================
来源：http://gpa.xziqi.cn

K. JSON 与序列化
来源：http://ymc.yfazqb.com

================================================================================
来源：http://uhd.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://rzp.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://czu.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://khd.yonumen.top

JS:   JSON.stringify(obj)
来源：http://wyr.uphjek.com

TS:   JSON.stringify(obj)
来源：http://agm.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dpg.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://xtj.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fid.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mmu.yongpay.top

[K02] JSON 字符串转对象
来源：http://lkl.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://uer.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ynp.aizwys.cn

JS:   JSON.parse(s)
来源：http://wxx.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://ezm.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mbx.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://gxa.xinyue.icu

Ruby: JSON.parse(s)
来源：http://nnx.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xjn.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://jnf.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://roq.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zed.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jpi.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://edm.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qnh.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tif.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://joz.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jzg.hesvh.cn

[K04] 读取 JSON 文件
来源：http://jhe.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://esm.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zjh.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qnf.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://glj.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qbj.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xyd.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://quq.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kdh.fktsv.cn

[K05] 深拷贝对象
来源：http://hpm.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://nsb.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://fcx.fzhhl.top

JS:   structuredClone(obj)
来源：http://wkg.jianghu66.top

TS:   structuredClone(obj)
来源：http://tpi.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yif.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gnf.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dvg.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://yzu.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://tcq.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rzm.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://coa.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hqq.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rip.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ooh.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://put.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sfe.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ykp.ydjk.org.cn

[K07] 进制转换
来源：http://bya.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gor.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vnh.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zjl.hywenlv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://urs.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rkc.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gmu.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tzs.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://erc.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://xtx.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://gan.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://knw.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://idi.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://wfy.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fcz.aibaodan.cn

Go:   encoding/gob
来源：http://isr.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://omm.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://var.guowangkeji.top

================================================================================
来源：http://hio.cdnleiting.top

L. 网络请求
来源：http://gjm.xuetiantiany.cn

================================================================================
来源：http://lek.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://rvk.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kyd.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xzo.sxryk.cn

JS:   await fetch(url)
来源：http://kbf.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://xjx.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mzz.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://xdr.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://zdq.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tei.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://foq.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://hfw.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mgp.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bdw.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gsn.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pak.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fbf.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://agi.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://teu.sysykeji.top

[L03] 设置自定义请求头
来源：http://pzy.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fph.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yis.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ijg.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vod.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iwc.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vmd.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://boy.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uyo.hongshengwenyu.top

[L04] 设置超时
来源：http://yzl.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://ida.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lnj.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eda.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wbj.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://npa.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://czm.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vak.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cfx.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://mvr.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uhk.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://txv.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lzo.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wav.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ifi.nwbrower.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dgx.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xfd.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yjr.fehbvm.com

[L06] 解析响应为 JSON
来源：http://gei.hesvh.cn

Py:   resp.json()
来源：http://vfy.hesvh.cn

PHP:  json_decode($body, true);
来源：http://syc.sxryk.cn

JS:   await resp.json()
来源：http://awv.gaohongyu789.top

TS:   await resp.json()
来源：http://xfu.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tkq.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://btm.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://boa.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uxt.ydjk.org.cn

[L07] 处理 HTTP 状态码
来源：http://hgx.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pix.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://szc.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://svc.ydzc1.top


<!-- 参考信息 -->