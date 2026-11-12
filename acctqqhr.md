代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://ebh.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kax.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oyb.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bmg.dianchejie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mrh.gaohongyu789.top

Go:   defer f.Close()
来源：http://lsq.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gfd.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jat.nwbrower.top

================================================================================
来源：http://bdx.zhaomingkeji.xyz

I. 正则表达式
来源：http://hgu.hnqzz.top

================================================================================
来源：http://joh.sufxvd.cn

[I01] 判断是否匹配
来源：http://inf.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jrf.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://vyw.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://pom.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://rcz.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kkr.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mib.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://ljk.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://con.sysykeji.top

[I02] 提取所有匹配
来源：http://saf.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://shz.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://izw.ydjk.org.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tkk.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://nlk.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ckh.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wcp.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://dtv.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vaf.guannengcc.top

[I03] 提取捕获分组
来源：http://szm.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vpe.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kiz.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hqy.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nbv.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ymr.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jxr.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sdu.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ulj.tarul.cn

[I04] 正则替换
来源：http://uje.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qay.daxiang520.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eaj.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ima.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sso.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rli.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hlw.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://tzx.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dyr.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://oje.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wqb.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ibd.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://hxv.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://kct.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://uxr.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oeh.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mwe.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fvr.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mqx.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ebr.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://usg.meibo888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://orp.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://enk.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yqn.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uvg.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://roz.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fab.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://prr.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hbu.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sty.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://loj.jyoumei.cn

TS:   /error/gim
来源：http://ohl.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://twb.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wun.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://kao.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vkr.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://ott.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xgx.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mkn.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mqb.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xzk.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lst.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kjf.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mbe.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hhg.gaohongyu789.top

================================================================================
来源：http://nru.52xcode.cn

J. 日期与时间
来源：http://ofn.svipenyu.cn

================================================================================
来源：http://ujh.smart0.xyz

[J01] 获取当前时间
来源：http://ffk.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bxs.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bks.yfazqb.com

JS:   new Date();  Date.now()
来源：http://mxd.tarul.cn

TS:   new Date();  Date.now()
来源：http://czy.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://igi.xinyue.icu

Go:   time.Now()
来源：http://vjs.zycfv.cn

Ruby: Time.now
来源：http://pfx.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gvh.aibaodan.cn

[J02] 格式化输出
来源：http://xno.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vxa.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pol.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ilx.nanxuanxn.top

TS:   d.toISOString()
来源：http://swk.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sya.ppjwa.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vwm.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://odm.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://opt.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://kjh.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lfo.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ema.xziqi.cn

JS:   new Date("2024-01-02")
来源：http://hsx.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://fey.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://xih.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lfa.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://kkc.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rgt.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://ovk.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gcm.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://afg.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cpk.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cit.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lic.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cfs.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://klw.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://llq.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://kza.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://lym.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://udg.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xap.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vjy.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://yni.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eqo.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://vbm.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://rpo.tarul.cn

[J06] 计算两时间之差
来源：http://xyi.yonumen.top

Py:   (end - start).total_seconds()
来源：http://qgg.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://aum.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nkh.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://roh.xuanzx.com

Java: Duration.between(start, end).toSeconds()
来源：http://zfc.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://rua.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://mlk.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://xkk.hesvh.cn

[J07] 比较两个日期
来源：http://vzz.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://mfb.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://drf.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eln.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://qjx.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hpm.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jnp.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://onj.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vlf.andypj.xyz

[J08] 提取年月日与星期
来源：http://itw.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bdq.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sgr.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qpk.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://szt.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wsu.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ubk.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cke.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jxm.jqgfzy.top

[J09] 时区处理
来源：http://xst.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fzx.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gji.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tvk.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iad.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kbn.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zxf.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ixj.yuanzhike.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bdx.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://act.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xtg.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vcq.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dar.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jma.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tbi.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://itg.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ius.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rdw.smart0.xyz

================================================================================
来源：http://cqz.sysykeji.top

K. JSON 与序列化
来源：http://hfh.shuidangran.top

================================================================================
来源：http://sva.meibo888.top

[K01] 对象转 JSON 字符串
来源：http://hiu.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ach.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xdr.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://pqg.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://kjz.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tgu.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://fuv.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://xdq.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qrs.c1oappe.top

[K02] JSON 字符串转对象
来源：http://fsw.ppjwa.cn

Py:   json.loads(s)
来源：http://fym.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vcb.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://twr.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://hiu.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wew.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://iha.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://dvb.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kfr.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://cay.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uhz.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wwe.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jdv.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sti.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://erk.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rvo.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eez.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dlz.vehdjk.com

[K04] 读取 JSON 文件
来源：http://yao.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lfi.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uzx.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ece.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ssn.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://siw.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dza.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jhn.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hjm.0kj1m.cn

[K05] 深拷贝对象
来源：http://ces.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://daz.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://pic.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://yeh.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://rmt.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gpv.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qzr.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fvm.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dkn.havefunace.top

[K06] 解析 URL 查询串
来源：http://ozv.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ozv.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://unj.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kan.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dbc.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hsm.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dyj.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ebv.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://czc.aizwys.cn

[K07] 进制转换
来源：http://tnv.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kuy.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hio.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xgm.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://krf.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kzu.vehdjk.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cxv.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bai.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uos.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://ivp.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://jso.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ads.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://wvp.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://vpo.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ifr.hammf.cn

Go:   encoding/gob
来源：http://thh.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://hvs.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hem.jinghuilouyu.cn

================================================================================
来源：http://sud.52xcode.cn

L. 网络请求
来源：http://pcp.yangfankeji.com

================================================================================
来源：http://qnu.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://ozy.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://alh.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qse.zhoulong.xyz

JS:   await fetch(url)
来源：http://nql.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://odj.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nms.cdnleiting.top

Go:   resp, err := http.Get(url)
来源：http://wur.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pvc.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oxf.sweek.top

[L02] 发送 POST JSON
来源：http://nlh.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://sfu.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ioz.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nnn.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cos.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cps.guowangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lwd.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wtk.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yvf.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://lgh.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ulo.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tiq.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tfi.zhengqikj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hnz.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ges.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fcr.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hhf.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wcn.fzhhl.top

[L04] 设置超时
来源：http://cyn.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://oxz.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nmk.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pdc.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fwd.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://umr.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hmz.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bhj.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gcn.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://bbn.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gmr.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pur.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ear.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nvt.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://trk.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sus.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wtj.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nyb.xingfuxueyuan.xyz

[L06] 解析响应为 JSON
来源：http://zln.hywenlv.cn


<!-- 参考信息 -->