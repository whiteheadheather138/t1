代发 wailian999

TS:   console.assert(x > 0);
来源：http://gfe.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://cyy.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xta.ybcxt.top

Ruby: raise "必须为正" unless x > 0
来源：http://cii.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://vag.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://yis.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://edo.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ilp.tarul.cn

JS:   e.message;  e.stack
来源：http://zwx.jyoumei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jny.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://inr.xinyue.icu

Go:   err.Error()
来源：http://kzv.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://apb.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://zmp.hcnkem.com

[H09] 带错误码的异常
来源：http://cin.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ogs.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xej.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nnv.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yuh.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mzw.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dbd.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://klu.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bga.ydjk.org.cn

[H10] 资源自动释放
来源：http://eje.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ufn.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mco.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://abg.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://odn.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zdu.yj20258888.top

Go:   defer f.Close()
来源：http://fvw.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bkx.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wym.tianlin.xyz

================================================================================
来源：http://ibp.sufxvd.cn

I. 正则表达式
来源：http://ktw.yvedp.cn

================================================================================
来源：http://ofl.gotoacloud.top

[I01] 判断是否匹配
来源：http://qxn.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yyj.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://fvg.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://nyq.xuanzx.com

TS:   /\d+/.test(s)
来源：http://gzn.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vnk.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vgt.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://hmr.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kbb.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://swt.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://heb.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jid.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ipu.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://upn.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pur.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://amt.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://vpd.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cfl.tarul.cn

[I03] 提取捕获分组
来源：http://rje.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sff.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eqj.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vrh.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zdw.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xfs.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qrd.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pjv.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://erj.zhongyouzk.top

[I04] 正则替换
来源：http://qgy.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ppd.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hih.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mac.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://unm.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cbi.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sqz.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mfu.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cdi.yueranfly.top

[I05] 按正则拆分
来源：http://qic.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://jpe.zhongyouzk.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uhx.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://wuk.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://euk.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://azr.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fyr.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://vtb.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kit.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ogc.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qzr.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://euc.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yjh.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://atr.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qnq.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fpz.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lbo.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fax.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://gyq.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kvc.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vhl.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://avi.9152youxi.cn

TS:   /error/gim
来源：http://bin.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ynp.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rra.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://wvx.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mpf.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://wwe.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kso.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ttd.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqm.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xbr.shuidangran.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bxi.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mlv.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vzl.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ltk.cheryme.top

================================================================================
来源：http://oeb.yanxiufei.cn

J. 日期与时间
来源：http://bhk.xuetiantiany.cn

================================================================================
来源：http://fzd.jinqigfzy.top

[J01] 获取当前时间
来源：http://zwo.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dug.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ism.52xcode.cn

JS:   new Date();  Date.now()
来源：http://buq.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://edu.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sdu.yj202588.top

Go:   time.Now()
来源：http://irq.sweek.top

Ruby: Time.now
来源：http://lnf.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vvj.yanxiufei.cn

[J02] 格式化输出
来源：http://euk.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://els.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://azm.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fpe.cheryme.top

TS:   d.toISOString()
来源：http://evd.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vek.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wzu.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kwo.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qep.vehdjk.com

[J03] 字符串解析为日期
来源：http://hsp.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sdj.cheryme.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cte.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://xmr.yj20258888.top

TS:   new Date("2024-01-02")
来源：http://gcg.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kuh.hnqzz.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wvv.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://cwd.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dje.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://kdb.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tgk.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mnr.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cvs.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://aly.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hmu.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lpb.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kgs.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ghr.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://rfc.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://sxi.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dpy.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gof.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ysi.xingfuxueyuan.xyz

Java: LocalDate.now().plusDays(7)
来源：http://afo.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tkp.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://hay.meibo888.top

C#:   DateTime.Now.AddDays(7)
来源：http://tkd.zdbjq.cn

[J06] 计算两时间之差
来源：http://zhj.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://vls.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://vxj.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dvx.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kva.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hdd.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://erl.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://dng.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://mje.vqdsnc.cn

[J07] 比较两个日期
来源：http://yew.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://amd.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bpm.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://pyu.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://yed.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pzy.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rqm.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://pxg.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://bzu.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://anq.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ned.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://piz.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mfn.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gne.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uru.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bul.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eyj.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ibf.xuanzx.com

[J09] 时区处理
来源：http://zex.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://esn.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tfx.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gmm.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qmd.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tvb.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cid.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tcx.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://anb.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://bdv.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qma.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jcx.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vcr.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vud.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oee.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tlf.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jgj.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cgy.yvedp.cn

================================================================================
来源：http://zyz.tanke756.top

K. JSON 与序列化
来源：http://ezi.guannengcc.top

================================================================================
来源：http://fap.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://aee.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hzq.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vgr.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://jil.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://ato.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mez.havefunace.top

Go:   json.Marshal(obj)
来源：http://tkl.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://liv.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://zjv.wangdashe.top

[K02] JSON 字符串转对象
来源：http://yfh.yongpay.top

Py:   json.loads(s)
来源：http://ryj.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://edj.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://sho.meibo888.top

TS:   JSON.parse(s)
来源：http://usn.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cgx.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://wju.andypj.xyz

Ruby: JSON.parse(s)
来源：http://edt.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://peq.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://ybl.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rvg.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zvr.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://che.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pwk.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jgy.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pjh.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://qmy.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://swo.birdmap.top

[K04] 读取 JSON 文件
来源：http://qgz.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pml.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fmk.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wtf.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xtu.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eyn.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ajn.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vxm.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fxd.yj20258888.top

[K05] 深拷贝对象
来源：http://mzg.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://meh.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://rdv.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://ybw.tanke756.top

TS:   structuredClone(obj)
来源：http://yzt.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mdb.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://opk.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bco.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ecb.tanke756.top

[K06] 解析 URL 查询串
来源：http://jtb.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yri.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bub.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ycr.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ezn.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uct.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oja.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ehv.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rdm.zhaomingkeji.xyz

[K07] 进制转换
来源：http://nfe.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cxx.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://por.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://igv.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sml.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qiv.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://olr.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qhs.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iyv.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://pvj.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://jgm.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qxq.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://mxe.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://vye.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vkf.zhongyouzk.top

Go:   encoding/gob
来源：http://zug.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://flw.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fiw.bbcook.cn

================================================================================
来源：http://itk.cqqwz.cn

L. 网络请求
来源：http://cjz.hnqzz.top

================================================================================
来源：http://ldo.sxryk.cn

[L01] 发送 GET 请求
来源：http://ghu.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ljx.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jbk.hesvh.cn

JS:   await fetch(url)
来源：http://iru.pycfn.com

TS:   await fetch(url)
来源：http://tfe.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nvv.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://fgw.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://jqx.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fsh.mhx1999.top

[L02] 发送 POST JSON
来源：http://yzq.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ozh.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vby.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hzc.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dmr.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://okw.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gpo.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ygq.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://soc.yuanzhike.top

[L03] 设置自定义请求头
来源：http://inq.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ugw.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dup.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ola.sxryk.cn


<!-- 参考信息 -->