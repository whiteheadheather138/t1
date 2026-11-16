代发 wailian999

TS:   console.assert(x > 0);
来源：http://fpp.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://wyh.chenjidiqi.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://plq.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://jds.zhengqikj.top

C#:   Debug.Assert(x > 0);
来源：http://aft.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://gbi.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://eev.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gjc.ybcxt.top

JS:   e.message;  e.stack
来源：http://ddr.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xwr.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://lds.daria6918.cn

Go:   err.Error()
来源：http://slu.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://vpj.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://bzh.mhx1999.top

[H09] 带错误码的异常
来源：http://stf.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gor.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bbx.iojbl.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rkc.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://llg.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sli.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oqq.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://sge.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hzf.shuidangran.top

[H10] 资源自动释放
来源：http://djf.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ucs.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vhl.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qzz.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zuo.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cvh.chenlongwang.top

Go:   defer f.Close()
来源：http://mfi.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dzn.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mvh.cdnleiting.top

================================================================================
来源：http://tof.ywan-chungtsiang.top

I. 正则表达式
来源：http://xri.tanke756.top

================================================================================
来源：http://ess.bbcook.cn

[I01] 判断是否匹配
来源：http://lqu.0kj1m.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kah.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://alz.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://ndz.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://shb.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iiv.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nxt.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://ucq.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://exk.tanke756.top

[I02] 提取所有匹配
来源：http://hzl.sweek.top

Py:   re.findall(r"\d+", s)
来源：http://ase.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uae.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qan.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://evz.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mxq.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fme.smart0.xyz

Ruby: s.scan(/\d+/)
来源：http://fer.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hse.yangfankeji.com

[I03] 提取捕获分组
来源：http://eeq.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sjg.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bmt.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yiv.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vbk.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gem.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://puw.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ofp.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vpe.ydjk.org.cn

[I04] 正则替换
来源：http://joy.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mal.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tlp.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://drz.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://ixj.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ase.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lab.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dzt.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://stu.nanxinkj.top

[I05] 按正则拆分
来源：http://cpd.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tdf.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rva.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://jkw.sjlbkw.cn

TS:   s.split(/\s*,\s*/)
来源：http://xyx.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://ern.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://svi.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://exh.dashuyun.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tte.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ymh.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xtk.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cos.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://umk.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oes.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zwu.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cfm.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dfl.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://khf.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://mml.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://her.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uhr.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://das.sufxvd.cn

TS:   /error/gim
来源：http://ntc.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wtg.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qnx.pycfn.com

Ruby: s.scan(/error/i)
来源：http://xpt.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ntg.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://lky.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://izw.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pev.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bvl.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://amp.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://etm.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xqy.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tdo.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gnj.yueranfly.top

================================================================================
来源：http://qmp.jqgufenzy.top

J. 日期与时间
来源：http://sgu.fengsongda.top

================================================================================
来源：http://psn.daria6918.cn

[J01] 获取当前时间
来源：http://lap.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://emq.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rkr.cheryme.top

JS:   new Date();  Date.now()
来源：http://csk.tarul.cn

TS:   new Date();  Date.now()
来源：http://kdd.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://klm.jianghu66.top

Go:   time.Now()
来源：http://vwg.zhixingplan.top

Ruby: Time.now
来源：http://ghx.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hdn.wangdashe.top

[J02] 格式化输出
来源：http://gfz.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wkx.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kqd.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bhv.feifeiyinyue.top

TS:   d.toISOString()
来源：http://rpv.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dwb.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ewt.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://trm.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uud.xinyue.icu

[J03] 字符串解析为日期
来源：http://jfw.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rgj.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://swb.xuetiantiany.cn

JS:   new Date("2024-01-02")
来源：http://kyn.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://xcm.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://tha.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tbt.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://qcp.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cqt.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://lfn.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rhd.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pug.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zbf.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gni.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vgd.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rfo.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wsr.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hli.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://ytp.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://dwd.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rhn.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bvq.yvedp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bge.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://uqn.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jxm.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://eyr.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gqp.zdqjudy.top

[J06] 计算两时间之差
来源：http://ool.hammf.cn

Py:   (end - start).total_seconds()
来源：http://ahk.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://cbf.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://esi.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qai.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://kqs.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://dso.hesvh.cn

Ruby: end - start                 # 返回秒数
来源：http://dpu.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://vkd.ywan-chungtsiang.top

[J07] 比较两个日期
来源：http://hsj.nanxuanxn.top

Py:   d1 < d2;  d1 == d2
来源：http://csq.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kjk.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://zao.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://bep.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yfa.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://riy.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uuz.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://evb.fktsv.cn

[J08] 提取年月日与星期
来源：http://kvq.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://daa.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qui.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vco.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rwg.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tur.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eyx.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eyv.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://enc.shangyingyoupin.top

[J09] 时区处理
来源：http://kau.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ppq.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wya.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qzq.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pqv.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kfa.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gdf.hywenlv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hlt.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nwu.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://wls.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zuw.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mva.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vav.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://izt.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fey.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hiq.aizwys.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://onm.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nri.vqdsnc.cn

================================================================================
来源：http://cac.ctjpmb.com

K. JSON 与序列化
来源：http://ezr.xziqi.cn

================================================================================
来源：http://cmy.zhijiandao.cn

[K01] 对象转 JSON 字符串
来源：http://upf.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eol.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rfi.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://mvo.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://tur.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ofk.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://ucg.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ncr.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://lla.gzhubu.top

[K02] JSON 字符串转对象
来源：http://wqv.jqgfzy.top

Py:   json.loads(s)
来源：http://qdh.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tfl.fzhhl.top

JS:   JSON.parse(s)
来源：http://quy.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://ucr.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://njs.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://wqa.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://ewh.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zur.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://ved.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jwo.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wim.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://uew.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://phf.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ddx.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sdk.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://pmz.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rld.ydzc1.top

[K04] 读取 JSON 文件
来源：http://pmm.hammf.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hok.yj20258.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ypt.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ogz.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pil.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aiq.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://khb.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cjt.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dan.yueranfly.top

[K05] 深拷贝对象
来源：http://lgd.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://egj.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://fmd.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://xnc.tanke756.top

TS:   structuredClone(obj)
来源：http://lqu.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wwt.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://don.daria6918.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fom.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xtf.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://tgx.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fhw.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gvu.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hhe.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ixd.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hwt.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://drs.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ytb.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wmr.snrcjt.cn

[K07] 进制转换
来源：http://qud.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yec.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ile.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://txq.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nsp.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wvt.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oxx.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wow.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://abm.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://zoy.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://zdn.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ruf.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://flk.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://sai.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gve.hnxiangtu.top

Go:   encoding/gob
来源：http://cty.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://nkn.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xsm.feifeiyinyue.top

================================================================================
来源：http://ucp.nwbrower.top

L. 网络请求
来源：http://fpm.ywan-chungtsiang.top

================================================================================
来源：http://tun.jyoumei.cn

[L01] 发送 GET 请求
来源：http://pwk.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hnc.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zxm.dashuyun.cn

JS:   await fetch(url)
来源：http://czl.zhijiandao.cn

TS:   await fetch(url)
来源：http://rgh.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kpz.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://khm.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ozh.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jko.jyoumei.cn

[L02] 发送 POST JSON
来源：http://yxl.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hnl.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xph.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gfw.hnxiangtu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wjc.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dgq.guowangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mie.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eqg.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kjp.fehbvm.com

[L03] 设置自定义请求头
来源：http://onu.nanxinkj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ywn.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dhm.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://npw.zhiwuduotai.top


<!-- 参考信息 -->