代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://jfj.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://cbt.redwolf501.top

[H09] 带错误码的异常
来源：http://qid.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iyk.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ogy.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fjp.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://auh.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ygk.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jwc.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bjj.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ely.ehwqpu.com

[H10] 资源自动释放
来源：http://eso.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://zyp.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vif.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fwv.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xes.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yxa.ydjk.org.cn

Go:   defer f.Close()
来源：http://gwo.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zky.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rfd.hysaishi.cn

================================================================================
来源：http://kav.yfazqb.com

I. 正则表达式
来源：http://cac.chenzaomai.com

================================================================================
来源：http://pnv.ctjpmb.com

[I01] 判断是否匹配
来源：http://qwa.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://efq.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://mju.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://djf.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://ynu.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dny.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://knt.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://kfx.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wpa.hammf.cn

[I02] 提取所有匹配
来源：http://dee.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://qnc.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://thn.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mge.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://zdl.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qwk.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qiy.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://qmd.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zcz.sweek.top

[I03] 提取捕获分组
来源：http://hvn.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hkf.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nba.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qoh.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ulq.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wzq.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xpm.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ybd.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://crq.hcnkem.com

[I04] 正则替换
来源：http://dbs.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dkq.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cmq.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://vbu.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://kgd.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://ula.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fxb.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sro.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kkv.snrcjt.cn

[I05] 按正则拆分
来源：http://uai.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tji.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ixr.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://akg.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://rsh.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://ypt.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jop.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://ljk.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rrn.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fsr.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tqo.cdnleiting.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iob.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dav.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://apy.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hwy.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cym.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qmz.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://umi.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://iif.wangdashe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wop.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gxn.aibaodan.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rtr.haohaochexian.top

TS:   /error/gim
来源：http://pio.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oat.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yws.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://cve.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jsl.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://ndz.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tcv.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://muz.iojbl.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wpy.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tza.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gbj.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tck.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://unq.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gyh.guowangkeji.top

================================================================================
来源：http://uwm.yongpay.top

J. 日期与时间
来源：http://vlk.mhx1999.top

================================================================================
来源：http://btc.tarul.cn

[J01] 获取当前时间
来源：http://urg.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kxl.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tuo.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://bxo.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://uce.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wnf.hesvh.cn

Go:   time.Now()
来源：http://ppx.cdnleiting.top

Ruby: Time.now
来源：http://ung.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://msv.hysaishi.cn

[J02] 格式化输出
来源：http://ypg.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baf.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oul.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://laa.ydjk.org.cn

TS:   d.toISOString()
来源：http://ral.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eri.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ksk.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dtl.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kud.52xcode.cn

[J03] 字符串解析为日期
来源：http://yty.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dtb.jyoumei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eog.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://rmh.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://zee.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rep.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pfi.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://wny.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oms.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://sxu.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nwb.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://feb.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qqa.xuanzx.com

TS:   Math.floor(Date.now() / 1000)
来源：http://osf.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ydj.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hxe.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rcu.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wks.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://uku.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://cqv.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tnr.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eyk.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lpl.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://ypj.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qxk.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://vwu.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://nch.tian-w.cn

[J06] 计算两时间之差
来源：http://zdq.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://maj.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://kdt.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nca.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wqv.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nxl.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://rwf.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://cex.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://kwk.cucudq.cn

[J07] 比较两个日期
来源：http://crs.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://oqc.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hbj.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://psq.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://lpq.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xwt.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ncj.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://opu.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://mqy.xylfe.cn

[J08] 提取年月日与星期
来源：http://pbh.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ogc.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wph.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mqr.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hzz.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qti.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hzk.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jtv.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mvw.vehdjk.com

[J09] 时区处理
来源：http://wrj.pengpengdd.cyou

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hef.pengpengdd.cyou

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ehd.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rcv.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fmf.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://acp.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ygm.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qls.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nwq.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://xxf.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://htm.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aiw.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mox.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mwv.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kbu.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sdm.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cvm.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rbw.cheryme.top

================================================================================
来源：http://vdf.redwolf501.top

K. JSON 与序列化
来源：http://ifi.shangyingyoupin.top

================================================================================
来源：http://uof.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://dme.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zwj.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kqe.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://qyf.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://hpr.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xey.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://yws.cheryme.top

Ruby: obj.to_json                                     // require "json"
来源：http://cdm.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ubp.havefunace.top

[K02] JSON 字符串转对象
来源：http://ukq.yfazqb.com

Py:   json.loads(s)
来源：http://eox.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ooc.cdnleiting.top

JS:   JSON.parse(s)
来源：http://sek.hfpthk.cn

TS:   JSON.parse(s)
来源：http://qur.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cdt.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://zga.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://bkj.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qql.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://loc.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dds.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kuh.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yds.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://rgu.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pyf.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vlm.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xwp.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lvw.guannengcc.top

[K04] 读取 JSON 文件
来源：http://gyn.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ekk.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pxl.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://orp.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cxd.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qfa.dianchejie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xdd.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://nah.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mac.shuidangran.top

[K05] 深拷贝对象
来源：http://acc.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://qdb.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://gah.mhx1999.top

JS:   structuredClone(obj)
来源：http://fkk.snrcjt.cn

TS:   structuredClone(obj)
来源：http://dol.yj20258.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eti.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rqp.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vgh.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ejk.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://dgj.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jku.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nez.nanxinkj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vne.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wej.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gzx.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://kng.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xrs.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iay.jqgufenzy.top

[K07] 进制转换
来源：http://exl.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fdi.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nmo.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dwp.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqo.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://exj.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cll.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://edd.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://trz.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://qnc.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://fzz.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nki.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://cvb.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://izm.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ens.mhx1999.top

Go:   encoding/gob
来源：http://kin.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://cmu.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sov.zhengqikj.top

================================================================================
来源：http://aao.yuxming.cn

L. 网络请求
来源：http://uka.fanxiaobao.xyz

================================================================================
来源：http://vgd.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://yka.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xme.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xta.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://etv.yuanzhike.top

TS:   await fetch(url)
来源：http://jyi.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mos.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://dqk.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://yph.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bjw.zhixingplan.top

[L02] 发送 POST JSON
来源：http://gxp.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://azx.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vac.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://omm.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://odi.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jop.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lzw.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zlp.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lmx.zhengqikj.top

[L03] 设置自定义请求头
来源：http://qhf.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dii.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jsy.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tzr.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gjq.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gyi.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xvv.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sit.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qls.tianlin.xyz

[L04] 设置超时
来源：http://yts.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://mzz.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xcv.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://orp.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bez.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://owt.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hxa.shanyushiyangkeji.top


<!-- 参考信息 -->