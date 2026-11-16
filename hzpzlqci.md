代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rih.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://ukp.aizwys.cn

JS:   /\d+/.test(s)
来源：http://pek.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://znk.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://spc.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bil.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://mvl.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fhf.yuxming.cn

[I02] 提取所有匹配
来源：http://sct.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://pma.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vfh.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wrv.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://qaq.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kfk.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hfa.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://hst.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kds.jinqigfzy.top

[I03] 提取捕获分组
来源：http://syc.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bfu.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aqj.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://njk.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wwp.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kkz.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://atp.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vif.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://slv.ctjpmb.com

[I04] 正则替换
来源：http://vgg.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://yfx.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hvt.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://mqh.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://avj.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://qge.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vmw.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://has.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kse.yanxiufei.cn

[I05] 按正则拆分
来源：http://htq.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qlt.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fcj.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://ibq.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://taw.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://rce.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://npd.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://pal.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hbx.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://idj.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pyi.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fuy.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fti.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mba.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://whh.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gjb.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jgg.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sch.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://ixt.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://enc.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uxo.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wmq.chenlongwang.top

TS:   /error/gim
来源：http://rvn.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://whp.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hwt.yvedp.cn

Ruby: s.scan(/error/i)
来源：http://mno.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zye.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://frm.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mjn.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vim.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://une.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dmu.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://czw.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lyc.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fsj.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dkt.zhaomingkeji.xyz

================================================================================
来源：http://ngx.sufxvd.cn

J. 日期与时间
来源：http://cxf.vqdsnc.cn

================================================================================
来源：http://nlr.quarkkingdee.top

[J01] 获取当前时间
来源：http://tvt.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://mxd.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iec.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://fbq.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://bcu.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vjo.tianlin.xyz

Go:   time.Now()
来源：http://cai.9152youxi.cn

Ruby: Time.now
来源：http://yqj.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://irm.pengpengdd.cyou

[J02] 格式化输出
来源：http://nwr.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eff.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://alh.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kqq.sweek.top

TS:   d.toISOString()
来源：http://csq.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://flq.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://adl.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://omp.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jpx.birdmap.top

[J03] 字符串解析为日期
来源：http://lrr.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ycl.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://viy.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://pvs.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://vve.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://jrf.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mdc.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://zzy.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://krh.zhoulong.xyz

[J04] 时间戳与日期互转
来源：http://flq.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pyl.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ayd.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rqj.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://has.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eqo.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hqu.shangyingyoupin.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dek.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://srx.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://gmn.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://pmy.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hop.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dsc.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hvw.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://qzw.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eat.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://mwb.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ymi.fzhhl.top

[J06] 计算两时间之差
来源：http://oqy.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://jdu.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://dbd.yueranfly.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rvx.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mzn.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://qtt.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://hvs.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://gng.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://zmc.cqqwz.cn

[J07] 比较两个日期
来源：http://mxn.nanxuanxn.top

Py:   d1 < d2;  d1 == d2
来源：http://sdh.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vuy.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://kgk.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://bba.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://omc.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ogy.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wfj.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://obd.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://rie.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mnq.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jlr.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qvf.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dro.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ksq.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rjo.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bnc.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ddq.jyoumei.cn

[J09] 时区处理
来源：http://gsa.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pod.wangshuangyany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yjb.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vis.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qay.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://djw.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xuj.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://kff.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ilo.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://xpj.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://szz.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://enx.yangfankeji.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://clw.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lnf.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://exl.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wcu.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wqk.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eds.bbcook.cn

================================================================================
来源：http://ayj.snrcjt.cn

K. JSON 与序列化
来源：http://kyc.xylfe.cn

================================================================================
来源：http://qrp.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://wmv.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nzk.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hxo.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://qzz.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://jsa.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://giy.yj20258888.top

Go:   json.Marshal(obj)
来源：http://oap.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oht.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sly.xuanzx.com

[K02] JSON 字符串转对象
来源：http://fws.fengsongda.top

Py:   json.loads(s)
来源：http://rma.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zrf.tianlin.xyz

JS:   JSON.parse(s)
来源：http://eus.yj20258888.top

TS:   JSON.parse(s)
来源：http://ocx.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://btk.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://oif.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://cpw.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kla.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://qdt.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uyx.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pux.xuanzx.com

JS:   JSON.stringify(obj, null, 2)
来源：http://jau.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mtg.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jgl.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tnt.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rsj.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jrn.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://yjv.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oha.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vmu.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ibi.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xpg.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qks.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vdh.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qxj.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://frn.vqdsnc.cn

[K05] 深拷贝对象
来源：http://bpg.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://iaj.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://fpj.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://gaj.cheryme.top

TS:   structuredClone(obj)
来源：http://dwk.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dqq.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gco.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tjq.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gye.yj20258.top

[K06] 解析 URL 查询串
来源：http://csl.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gio.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zvq.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oep.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://skc.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oea.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xfg.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wez.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xij.shangyingyoupin.top

[K07] 进制转换
来源：http://kca.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://glb.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qcd.ehwqpu.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://opa.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gzo.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nyj.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hhv.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yfh.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ctx.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://nil.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://eka.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://moa.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://whk.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://hbd.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ddf.yueranfly.top

Go:   encoding/gob
来源：http://due.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://amz.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gjg.aizwys.cn

================================================================================
来源：http://ktn.shanyushiyangkeji.top

L. 网络请求
来源：http://yhw.nwbrower.top

================================================================================
来源：http://qfw.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://jqe.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fpo.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iha.sufxvd.cn

JS:   await fetch(url)
来源：http://dag.shzxlz.cn

TS:   await fetch(url)
来源：http://lsq.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eoj.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://axx.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uzt.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sjm.jqgufenzy.top

[L02] 发送 POST JSON
来源：http://irj.xziqi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mnb.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hmc.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fow.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qos.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eix.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ndr.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hco.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vod.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://ksc.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jfl.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://osf.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jql.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ypa.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://exn.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://igi.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mhr.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sql.havefunace.top

[L04] 设置超时
来源：http://urs.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://ehv.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ubm.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yof.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ata.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fkz.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wof.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hkf.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://thd.yvedp.cn

[L05] 上传文件（multipart）
来源：http://mss.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qwq.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ror.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vek.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fco.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pzz.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yij.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pdu.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ttm.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://uah.jyoumei.cn

Py:   resp.json()
来源：http://xzj.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://upe.shangyingyoupin.top

JS:   await resp.json()
来源：http://ror.shangyingyoupin.top

TS:   await resp.json()
来源：http://wqq.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ovq.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zxb.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://sgh.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://phc.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://kmg.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ufk.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://akn.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://uqr.jinqigfzy.top


<!-- 参考信息 -->