代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://jmq.cqqwz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uzy.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ypy.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://utu.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sxy.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://wwb.aibaodan.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oha.jqgfzy.top

[H10] 资源自动释放
来源：http://pun.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zjq.zycfv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fxd.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qsp.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qjr.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qgi.52xcode.cn

Go:   defer f.Close()
来源：http://nxw.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fwm.fengsongda.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jer.zhaomingkeji.xyz

================================================================================
来源：http://dub.sxryk.cn

I. 正则表达式
来源：http://ubr.xylfe.cn

================================================================================
来源：http://jfl.cashguo.top

[I01] 判断是否匹配
来源：http://efn.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dfw.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://vzh.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://xue.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://wtq.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vvw.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nis.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://egw.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bxr.yj20258888.top

[I02] 提取所有匹配
来源：http://cmf.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://qzg.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hcm.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mhr.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://grp.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mxh.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jsv.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://alo.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xis.havefunace.top

[I03] 提取捕获分组
来源：http://oag.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wzs.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bgs.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qfy.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://znb.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qdi.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gbw.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bce.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aer.0kj1m.cn

[I04] 正则替换
来源：http://pfb.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://isr.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://utv.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xlo.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://pmm.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://tbw.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xae.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lli.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gqr.guowangkeji.top

[I05] 按正则拆分
来源：http://hor.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hyw.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oii.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://gtm.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://naf.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://otq.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pff.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://wya.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bvt.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xbr.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jnm.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iaz.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sry.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bwm.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ogm.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jip.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xjk.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tyk.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://bqg.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hvt.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ggq.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ybf.nanxinkj.top

TS:   /error/gim
来源：http://kwv.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ynl.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vkz.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://dsu.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://abu.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://sjo.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aty.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kcg.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zta.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fja.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aqb.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mcj.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pbb.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vex.ctjpmb.com

================================================================================
来源：http://wko.yj20258888.top

J. 日期与时间
来源：http://pod.fanxiaobao.xyz

================================================================================
来源：http://ddt.zhongyouzk.top

[J01] 获取当前时间
来源：http://tht.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://npn.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ssm.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://qzs.aizwys.cn

TS:   new Date();  Date.now()
来源：http://vwa.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wtu.zhixingplan.top

Go:   time.Now()
来源：http://ivn.daxiang520.top

Ruby: Time.now
来源：http://tds.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://igl.sufxvd.cn

[J02] 格式化输出
来源：http://gah.jyoumei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ivq.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dxm.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zij.zdbjq.cn

TS:   d.toISOString()
来源：http://wvf.aibaodan.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uot.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cpr.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fea.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qjp.xuanzx.com

[J03] 字符串解析为日期
来源：http://mba.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hcl.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fcn.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://via.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://sin.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ndb.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lig.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://fkf.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kpa.aizwys.cn

[J04] 时间戳与日期互转
来源：http://qyn.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pzc.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hdz.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lio.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ezw.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ccg.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pfl.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yzs.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cma.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://svx.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://nwc.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://evh.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nyb.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lhz.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://ynr.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lyn.mhx1999.top

Ruby: Time.now + 7 * 86400
来源：http://njy.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://idn.quarkkingdee.top

[J06] 计算两时间之差
来源：http://wjx.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://yut.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://smx.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pnc.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hzf.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://ygr.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://ica.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://qxh.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://try.hammf.cn

[J07] 比较两个日期
来源：http://pqq.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://emm.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fhf.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://rgm.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://rlz.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wxe.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sjb.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://gyf.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://uxo.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://glm.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gsl.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oep.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://txs.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xrv.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dqh.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sxc.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://san.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ohn.9152youxi.cn

[J09] 时区处理
来源：http://sbp.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wcg.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ain.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jbv.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://chu.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bql.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yxx.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ysk.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yfg.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://wif.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://xps.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://thi.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yja.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wmw.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://obf.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lui.aizwys.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wib.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vhq.cqqwz.cn

================================================================================
来源：http://pya.yj20258.top

K. JSON 与序列化
来源：http://qxu.xylfe.cn

================================================================================
来源：http://rph.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://pfw.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zpu.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jbx.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://woj.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://sof.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wnd.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://qxu.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ejr.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://abr.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://gps.ydjk.org.cn

Py:   json.loads(s)
来源：http://uzo.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://avg.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://fzv.dashuyun.cn

TS:   JSON.parse(s)
来源：http://qun.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lbk.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://kne.shuidangran.top

Ruby: JSON.parse(s)
来源：http://bxf.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zar.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://drk.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://chq.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fje.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ert.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://tig.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rew.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://imy.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://gay.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lar.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://ulb.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://das.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hpj.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ifz.uphjek.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iqc.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gdh.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gkx.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bck.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nxo.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://ohd.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://lxa.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://zyg.sysykeji.top

JS:   structuredClone(obj)
来源：http://ppi.redwolf501.top

TS:   structuredClone(obj)
来源：http://ysa.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://siw.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://azb.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://paj.cdnleiting.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xdf.sysykeji.top

[K06] 解析 URL 查询串
来源：http://jxl.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cdl.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ruz.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nzr.yj20258888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fvn.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uww.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zlm.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vus.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://adp.tianlin.xyz

[K07] 进制转换
来源：http://eqx.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tlb.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cyo.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kdg.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gop.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nrw.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fav.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zwu.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://svz.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://ava.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://yia.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://muj.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://cmg.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://vkv.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://may.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://cuj.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://kuq.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sif.0kj1m.cn

================================================================================
来源：http://lxw.shangyingyoupin.top

L. 网络请求
来源：http://jso.aizwys.cn

================================================================================
来源：http://ocy.epnwcf.com

[L01] 发送 GET 请求
来源：http://vad.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lzw.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lxv.sweek.top

JS:   await fetch(url)
来源：http://hov.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://hkz.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ylo.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://kov.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://wej.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yly.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://vqg.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://ohc.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://trl.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://scs.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gfe.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pnr.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dwm.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gbv.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://htw.hammf.cn

[L03] 设置自定义请求头
来源：http://tif.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uev.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://srm.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cqm.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pwk.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://slh.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nrv.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oyz.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dnp.shzxlz.cn

[L04] 设置超时
来源：http://uaw.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://yjt.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eia.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ipn.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bvb.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jag.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qar.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sym.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rdz.yongpay.top

[L05] 上传文件（multipart）
来源：http://bpd.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://spm.hywenlv.cn


<!-- 参考信息 -->