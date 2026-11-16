代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xnh.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://buj.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://kuv.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ieb.feifeiyinyue.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ycn.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://fbd.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qjz.yongpay.top

[H06] 可选值 / 空值安全访问
来源：http://wob.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://yrg.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eyl.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://mhb.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://hsn.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eao.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rwm.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://qwt.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://yuo.zhaomingkeji.xyz

[H07] 断言
来源：http://oyj.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://rwn.chenlongwang.top

PHP:  assert($x > 0);
来源：http://syv.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://yfu.epnwcf.com

TS:   console.assert(x > 0);
来源：http://nju.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://vbr.shangyingyoupin.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ari.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://fjn.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://eeg.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://qjj.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://gea.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jhj.daria6918.cn

JS:   e.message;  e.stack
来源：http://ylb.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bwf.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gme.316326.xyz

Go:   err.Error()
来源：http://fus.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://tvr.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://ypt.zhengqikj.top

[H09] 带错误码的异常
来源：http://jsv.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hks.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://snx.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gzz.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rsd.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vmi.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vbw.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://hwr.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bai.hnxiangtu.top

[H10] 资源自动释放
来源：http://gaa.quarkkingdee.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rjx.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yvi.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wab.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fbv.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ikm.ctjpmb.com

Go:   defer f.Close()
来源：http://oyc.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ymf.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gza.nwbrower.top

================================================================================
来源：http://kfn.meibo888.top

I. 正则表达式
来源：http://faf.birdmap.top

================================================================================
来源：http://ewt.jinqigufen.top

[I01] 判断是否匹配
来源：http://gep.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zdd.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://stm.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://gcf.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://gsp.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eom.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bpq.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://kwh.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zax.jqgfzy.top

[I02] 提取所有匹配
来源：http://bzn.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://ipz.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://klm.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nhf.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://qqv.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wju.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ubj.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://tez.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vmq.jiagoushi.top

[I03] 提取捕获分组
来源：http://cvo.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ibz.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cww.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rlp.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mri.nanxuanxn.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://law.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vrf.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gou.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kfz.yj20258888.top

[I04] 正则替换
来源：http://vrb.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://jul.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zre.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://npn.aizwys.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mzv.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qdv.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sth.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://soh.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eoq.zhongyouzk.top

[I05] 按正则拆分
来源：http://xcu.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fzj.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://luu.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://dcf.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://boc.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://qbe.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://usn.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ulu.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aif.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lvg.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mgb.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bvb.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sfc.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mzv.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ino.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mfz.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cgc.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jia.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://bsm.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vxm.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kco.xingfuxueyuan.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kjh.shanyushiyangtech.top

TS:   /error/gim
来源：http://qej.yongpay.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bbb.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kbi.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://axt.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ysg.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://uas.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jnk.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ewr.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wci.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pgr.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://zso.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ojc.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rcu.ppjwa.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://llv.fzhhl.top

================================================================================
来源：http://eni.tarul.cn

J. 日期与时间
来源：http://shs.cqqwz.cn

================================================================================
来源：http://djw.xylfe.cn

[J01] 获取当前时间
来源：http://kvk.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rrb.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://duc.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://qkq.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://vqk.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pqk.gogol.net.cn

Go:   time.Now()
来源：http://voe.xylfe.cn

Ruby: Time.now
来源：http://ecf.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nol.cheryme.top

[J02] 格式化输出
来源：http://pxe.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svw.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tdx.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://isc.jinghuilouyu.cn

TS:   d.toISOString()
来源：http://rqe.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sut.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ovt.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wad.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pet.mhx1999.top

[J03] 字符串解析为日期
来源：http://kxl.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nbr.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nzt.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://rdk.havefunace.top

TS:   new Date("2024-01-02")
来源：http://myx.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hbw.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ybr.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://dco.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ccb.hnqzz.top

[J04] 时间戳与日期互转
来源：http://wss.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mzr.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zfl.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rld.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://pxl.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vwo.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://unk.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lsl.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vwu.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://dfw.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://owf.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://uam.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wgb.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://skw.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://qxo.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ect.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://uwx.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://nme.haohaochexian.top

[J06] 计算两时间之差
来源：http://mph.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://hzq.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://sjo.jiagoushi.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://usw.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ymx.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://yon.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://pdq.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://zfi.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://qov.zhengqikj.top

[J07] 比较两个日期
来源：http://hhk.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://wng.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yjn.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://lwl.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://ibp.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aks.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://czc.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mhc.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://zri.sufxvd.cn

[J08] 提取年月日与星期
来源：http://zmo.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bly.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vzg.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://maz.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nla.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wha.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mut.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fxb.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ypl.nanxinkj.top

[J09] 时区处理
来源：http://shx.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hmp.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://byg.yj20258.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wiz.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opn.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ghp.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mei.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uzd.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://poy.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://ugt.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cjv.cucudq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://chj.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qmp.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ktu.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lby.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eke.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://knz.tian-w.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ukq.xziqi.cn

================================================================================
来源：http://sik.zhongyouzk.top

K. JSON 与序列化
来源：http://vuv.nanxuanxn.top

================================================================================
来源：http://jsq.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://avp.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hos.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xqv.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://nih.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://pby.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yop.ydzc1.top

Go:   json.Marshal(obj)
来源：http://wxy.gogol.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wqo.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bfy.hcnkem.com

[K02] JSON 字符串转对象
来源：http://paf.sufxvd.cn

Py:   json.loads(s)
来源：http://wit.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sgu.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://nxa.hysaishi.cn

TS:   JSON.parse(s)
来源：http://nba.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oil.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://evl.xylfe.cn

Ruby: JSON.parse(s)
来源：http://hgx.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fom.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://gkb.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oaq.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rwb.yonumen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cwg.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tzc.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hqz.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wvu.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://det.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hat.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://fnx.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://caq.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jyr.jinqigufen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xeu.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fli.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://efi.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ceb.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://axc.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lcw.hesvh.cn

[K05] 深拷贝对象
来源：http://rmy.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://mxl.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://zko.haohaochexian.top

JS:   structuredClone(obj)
来源：http://hts.yfazqb.com

TS:   structuredClone(obj)
来源：http://mwl.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ujp.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qlb.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iah.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://wlk.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://sdz.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mth.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vde.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fxl.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xex.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://myi.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lza.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jqh.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ana.0kj1m.cn

[K07] 进制转换
来源：http://cje.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lym.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jsb.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://whv.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://unw.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hsl.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gtu.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cbc.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://buc.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://hps.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://yzb.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://eeg.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://hgt.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://hbs.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oqx.hongshengwenyu.top

Go:   encoding/gob
来源：http://ujh.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://zzj.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nfz.hongshengwenyu.top

================================================================================
来源：http://tcc.52xcode.cn

L. 网络请求
来源：http://yhb.ivvv.top

================================================================================
来源：http://pey.52xcode.cn

[L01] 发送 GET 请求
来源：http://bgd.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://muu.yvedp.cn


<!-- 参考信息 -->