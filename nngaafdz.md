代发 wailian999

JS:   e.message;  e.stack
来源：http://rss.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kft.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hoh.yanxiufei.cn

Go:   err.Error()
来源：http://oyd.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://yrt.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://ocm.0kj1m.cn

[H09] 带错误码的异常
来源：http://ybl.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jec.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://vwh.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rzy.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://msw.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iml.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ajz.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mws.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zoh.yuxming.cn

[H10] 资源自动释放
来源：http://afn.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kwm.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tjt.fanxiaobao.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://klr.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tdv.mhx1999.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pcf.c1oappe.top

Go:   defer f.Close()
来源：http://qgz.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://msw.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ado.pycfn.com

================================================================================
来源：http://jrw.aibaodan.cn

I. 正则表达式
来源：http://qqj.ybcxt.top

================================================================================
来源：http://lew.52xcode.cn

[I01] 判断是否匹配
来源：http://eph.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://arz.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lwu.gzhubu.top

JS:   /\d+/.test(s)
来源：http://lfm.yvedp.cn

TS:   /\d+/.test(s)
来源：http://htb.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lck.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yyp.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://ccx.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ozd.jqgufenzy.top

[I02] 提取所有匹配
来源：http://bei.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://gbk.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cut.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kgx.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://csy.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kgd.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hfk.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://daf.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dwr.fktsv.cn

[I03] 提取捕获分组
来源：http://etg.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pce.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rax.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gmk.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iwk.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bhn.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dys.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cvr.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qcr.tianlin.xyz

[I04] 正则替换
来源：http://eii.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iqy.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://myn.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://qvn.hcnkem.com

TS:   s.replace(/\d+/g, "#")
来源：http://pax.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://abh.pengpengdd.cyou

Go:   re.ReplaceAllString(s, "#")
来源：http://ukl.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nug.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hit.gaohongyu789.top

[I05] 按正则拆分
来源：http://drw.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://cah.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xmi.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://yvn.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://vxs.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://ahq.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gmf.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bod.andypj.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uja.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://clz.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xms.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pba.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hhd.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rqu.feifeiyinyue.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qss.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fpx.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kjq.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nfp.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://sye.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gsg.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yyj.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://akw.c1oappe.top

TS:   /error/gim
来源：http://wiz.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xat.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zje.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://amf.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mcb.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://zhz.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qwv.smart0.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dvw.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rsw.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wsr.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://umu.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gdf.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cwi.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wig.52xcode.cn

================================================================================
来源：http://hto.zhixingplan.top

J. 日期与时间
来源：http://vlw.nwbrower.top

================================================================================
来源：http://kto.sjlbkw.cn

[J01] 获取当前时间
来源：http://flz.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gff.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lfy.yj202588.top

JS:   new Date();  Date.now()
来源：http://cwn.yj202588.top

TS:   new Date();  Date.now()
来源：http://zwb.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://msx.fanxiaobao.xyz

Go:   time.Now()
来源：http://tof.andypj.xyz

Ruby: Time.now
来源：http://hms.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gwj.9152youxi.cn

[J02] 格式化输出
来源：http://sqy.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cnp.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iwz.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bds.snrcjt.cn

TS:   d.toISOString()
来源：http://lsq.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oqa.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dkj.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wcp.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://upm.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://ycz.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zzz.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hkg.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://mxd.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://iaf.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://qgc.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://skf.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://lhe.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://osf.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://pqu.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ztp.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iab.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xdk.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://puw.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://evu.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nhp.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cft.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xvn.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://gvj.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://kah.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://czg.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fgy.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://srw.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://pzw.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xcd.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://acu.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://cjv.yuanzhike.top

[J06] 计算两时间之差
来源：http://snj.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://nmv.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://prw.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fyn.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ivl.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://byp.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://jfx.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://yjs.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://nzo.cheryme.top

[J07] 比较两个日期
来源：http://xgp.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://hfg.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gsf.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fcn.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ade.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://osp.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ogr.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://cvn.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://kis.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://mya.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ssp.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pfk.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tej.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://inn.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pyp.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ieb.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://clu.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xpm.sufxvd.cn

[J09] 时区处理
来源：http://mkn.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hih.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hfu.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yww.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jam.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://khv.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ugb.hcnkem.com

Ruby: Time.now.getlocal("+08:00")
来源：http://jvw.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fce.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://toy.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://knz.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cul.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ide.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aar.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jgh.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fyi.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://liy.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://err.gotoacloud.top

================================================================================
来源：http://pfq.cashguo.top

K. JSON 与序列化
来源：http://ogc.jinghuilouyu.cn

================================================================================
来源：http://vsj.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://dws.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wpg.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xyo.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://fxb.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://mff.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://beb.zycfv.cn

Go:   json.Marshal(obj)
来源：http://rvc.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://mxq.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ewm.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://lkd.yj202588.top

Py:   json.loads(s)
来源：http://pno.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ice.mhx1999.top

JS:   JSON.parse(s)
来源：http://gax.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://zay.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tbh.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://wyq.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://tfv.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wwz.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://ios.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dcc.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ubm.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bbk.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ozl.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bdo.jinqigufen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dzr.hesvh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hhw.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mli.iojbl.cn

[K04] 读取 JSON 文件
来源：http://ubc.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pgt.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dpk.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lux.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yhd.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://trz.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fpz.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tuo.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jyv.zdbjq.cn

[K05] 深拷贝对象
来源：http://zkr.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://wkz.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://lot.shuidangran.top

JS:   structuredClone(obj)
来源：http://cqk.gogol.net.cn

TS:   structuredClone(obj)
来源：http://ejw.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eoq.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xzd.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wje.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pvn.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://xsp.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://few.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hij.vehdjk.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xhi.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yud.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wdo.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mnc.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tyw.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ldo.yvedp.cn

[K07] 进制转换
来源：http://gzq.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ztg.xuetiantiany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eqx.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pxz.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nat.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dsk.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ssj.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gfu.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cml.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://zrj.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://dxu.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eie.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://iso.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://vmf.jqgfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ubd.nanxuanxn.top

Go:   encoding/gob
来源：http://ifb.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://tgm.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tpu.ybcxt.top

================================================================================
来源：http://bko.ctjpmb.com

L. 网络请求
来源：http://dfc.hfpthk.cn

================================================================================
来源：http://jqp.gzhubu.top

[L01] 发送 GET 请求
来源：http://mcw.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fkm.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cps.tian-w.cn

JS:   await fetch(url)
来源：http://tuv.bjfxy.top

TS:   await fetch(url)
来源：http://wex.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tal.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://znc.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qsk.ehwqpu.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://koj.chenzaomai.com

[L02] 发送 POST JSON
来源：http://sbu.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fbp.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xyo.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yhz.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wkx.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qey.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iof.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dly.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zzc.xziqi.cn

[L03] 设置自定义请求头
来源：http://qcp.zhoulong.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sld.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bjc.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hni.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nhw.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bxd.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zme.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qso.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ibn.zdbjq.cn

[L04] 设置超时
来源：http://vbb.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://xxj.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sqa.sufxvd.cn


<!-- 参考信息 -->