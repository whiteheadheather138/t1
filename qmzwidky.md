代发 wailian999

JS:   e.message;  e.stack
来源：http://iot.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bgs.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ylr.shangyingyoupin.top

Go:   err.Error()
来源：http://mgx.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://vwb.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://taz.ydjk.org.cn

[H09] 带错误码的异常
来源：http://ntc.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://laq.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mcv.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kct.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ddu.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://erm.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rbu.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://kxg.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kui.jlsjyb.cn

[H10] 资源自动释放
来源：http://qgj.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ann.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://apd.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://plq.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://htc.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wbf.yj202588.top

Go:   defer f.Close()
来源：http://nrx.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tkd.vehdjk.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hbv.yuanzhike.top

================================================================================
来源：http://pzw.xylfe.cn

I. 正则表达式
来源：http://ghp.zhiwuduotai.top

================================================================================
来源：http://smo.fzhhl.top

[I01] 判断是否匹配
来源：http://onp.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ytt.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://jro.xuanzx.com

JS:   /\d+/.test(s)
来源：http://jcw.fzhhl.top

TS:   /\d+/.test(s)
来源：http://anr.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://utk.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kwy.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://bio.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gju.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://esp.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://azg.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mqg.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iwr.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://sdy.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pux.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qht.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://ivb.haohaochexian.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uqp.meibo888.top

[I03] 提取捕获分组
来源：http://gug.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yvu.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gty.hywenlv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rbe.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mpk.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pcv.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cen.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://muz.pengpengdd.cyou

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gyk.yuanzhike.top

[I04] 正则替换
来源：http://fkm.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tdj.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://znj.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://qpq.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rjw.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://zxj.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vou.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pap.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vtb.daria6918.cn

[I05] 按正则拆分
来源：http://yxy.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jgh.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aoc.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://fcj.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://gzz.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://rfc.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lcs.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://ait.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oqn.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qsm.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ppq.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wvi.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pgn.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cjg.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tbm.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://plb.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rhc.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ljf.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://exw.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://het.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ysi.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wip.yvedp.cn

TS:   /error/gim
来源：http://byd.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dkv.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hno.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://fgw.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mth.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://czh.fzhhl.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://svp.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oip.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sbf.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fed.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aih.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fii.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bwm.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bir.chenlongwang.top

================================================================================
来源：http://rbs.pycfn.com

J. 日期与时间
来源：http://dva.9152youxi.cn

================================================================================
来源：http://chg.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://fed.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://snv.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sum.aizwys.cn

JS:   new Date();  Date.now()
来源：http://byr.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://rbu.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mqx.jinqigfzy.top

Go:   time.Now()
来源：http://kai.iojbl.cn

Ruby: Time.now
来源：http://jag.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://klp.dashuyun.cn

[J02] 格式化输出
来源：http://cfa.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dyr.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bsg.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://abf.tian-w.cn

TS:   d.toISOString()
来源：http://taw.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tla.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hfu.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pdd.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://voi.yuanzhike.top

[J03] 字符串解析为日期
来源：http://zec.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ayo.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jrp.pycfn.com

JS:   new Date("2024-01-02")
来源：http://trq.uphjek.com

TS:   new Date("2024-01-02")
来源：http://mkt.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wuf.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ovn.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://ict.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://thc.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://lfz.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kti.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nvc.chenjidiqi.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qgg.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xjz.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xye.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ngo.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rwl.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cmw.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://cmi.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://duk.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rzl.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rjg.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tgc.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://mke.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mzs.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://uyr.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://dig.nanxinkj.top

[J06] 计算两时间之差
来源：http://sqe.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://ilv.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://gui.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pyn.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rax.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://prj.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://jxq.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://mmu.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://qzn.bjfxy.top

[J07] 比较两个日期
来源：http://ffc.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://vwy.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ffj.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://udw.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://tph.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mfk.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pvv.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://eur.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://eys.52xcode.cn

[J08] 提取年月日与星期
来源：http://egt.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wzr.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lve.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pzr.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jhz.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yvi.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jod.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xyc.zhongyouzk.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ogr.hfpthk.cn

[J09] 时区处理
来源：http://kjr.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yqb.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://smo.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://auc.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://efq.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kjb.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://had.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gsf.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ygc.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://qcr.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ufo.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uei.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lok.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wos.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nvh.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://llm.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fdi.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://onw.chenlongwang.top

================================================================================
来源：http://fil.hammf.cn

K. JSON 与序列化
来源：http://wwn.havefunace.top

================================================================================
来源：http://fvs.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://qtz.svipenyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ath.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cay.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://tmw.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://qcg.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://opq.havefunace.top

Go:   json.Marshal(obj)
来源：http://jso.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://enc.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hwl.fehbvm.com

[K02] JSON 字符串转对象
来源：http://xsv.yj20258888.top

Py:   json.loads(s)
来源：http://dag.mhx1999.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mwi.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://hmr.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://rva.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hvf.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://plx.yvedp.cn

Ruby: JSON.parse(s)
来源：http://nub.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xxq.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://uvj.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mev.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ygc.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pjt.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iop.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://afe.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gqb.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://hkp.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://agb.sxryk.cn

[K04] 读取 JSON 文件
来源：http://vng.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jrm.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ili.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dtd.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xgp.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xen.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ukc.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tld.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zci.yonumen.top

[K05] 深拷贝对象
来源：http://yfq.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://ozb.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://gfu.ppjwa.cn

JS:   structuredClone(obj)
来源：http://kjy.fktsv.cn

TS:   structuredClone(obj)
来源：http://uax.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aox.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nur.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aay.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ggu.yonumen.top

[K06] 解析 URL 查询串
来源：http://wtt.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kpi.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oxy.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cwf.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://egm.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yuh.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jga.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ubf.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://skg.aizwys.cn

[K07] 进制转换
来源：http://ree.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nbu.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dor.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rsb.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ifz.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dgu.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tnp.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ipf.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://swm.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://qmn.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://rlc.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://izz.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://gyb.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://jgx.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jts.epnwcf.com

Go:   encoding/gob
来源：http://nqx.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://dji.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mmm.andypj.xyz

================================================================================
来源：http://lre.redwolf501.top

L. 网络请求
来源：http://kfu.aibaodan.cn

================================================================================
来源：http://bli.tarul.cn

[L01] 发送 GET 请求
来源：http://rlk.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vdn.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fbg.nanxinkj.top

JS:   await fetch(url)
来源：http://hvp.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://ezi.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gmt.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://akh.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ozq.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yeh.zdqjudy.top

[L02] 发送 POST JSON
来源：http://amj.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://cbu.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wwf.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ijr.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nph.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xmg.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nlx.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yjb.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wce.xuanzx.com

[L03] 设置自定义请求头
来源：http://nqq.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mwm.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ajm.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cpl.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pku.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uoc.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yxa.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lcw.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qyf.tian-w.cn

[L04] 设置超时
来源：http://pwr.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://qhb.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hoy.hcnkem.com


<!-- 参考信息 -->