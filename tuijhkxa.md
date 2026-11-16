代发 wailian999

[H07] 断言
来源：http://nqs.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://xnz.redwolf501.top

PHP:  assert($x > 0);
来源：http://byk.aizwys.cn

JS:   console.assert(x > 0);
来源：http://now.c1oappe.top

TS:   console.assert(x > 0);
来源：http://uds.yongpay.top

Java: assert x > 0 : "必须为正";
来源：http://csi.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hif.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jyx.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://amt.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://jyo.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://esr.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qey.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://soe.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://hbp.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ils.pycfn.com

Go:   err.Error()
来源：http://sla.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://tqj.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://mrz.dashuyun.cn

[H09] 带错误码的异常
来源：http://kjd.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nww.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ele.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bds.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xiy.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dqq.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qic.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://sxe.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vqv.havefunace.top

[H10] 资源自动释放
来源：http://plt.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mpc.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xaj.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iep.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uhg.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://snx.xinyue.icu

Go:   defer f.Close()
来源：http://see.andypj.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://toi.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xhr.sufxvd.cn

================================================================================
来源：http://tew.dashuyun.cn

I. 正则表达式
来源：http://fly.haohaochexian.top

================================================================================
来源：http://nph.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://suh.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hay.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://ekl.hnqzz.top

JS:   /\d+/.test(s)
来源：http://arq.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://zme.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://czw.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zew.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://ycc.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uwd.dianchejie.cn

[I02] 提取所有匹配
来源：http://pow.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://xgh.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zhr.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fnv.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://eqo.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tsz.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xqi.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://cis.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://epq.hnqzz.top

[I03] 提取捕获分组
来源：http://bux.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zwj.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hgw.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dmx.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tid.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://onv.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://huu.pengpengdd.cyou

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fjl.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xdf.feifeiyinyue.top

[I04] 正则替换
来源：http://tbk.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fey.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://raq.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://naf.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://odd.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://nmc.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dao.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gbv.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iee.jinqigufen.top

[I05] 按正则拆分
来源：http://eyc.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xuz.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gho.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://ifl.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://hyr.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://qss.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wrh.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://utf.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://trr.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rug.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zkv.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zvd.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xjx.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://prv.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bdo.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sqt.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jql.hongshengwenyu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fln.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://qgf.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dfy.ywan-chungtsiang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cne.c1oappe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pak.aibaodan.cn

TS:   /error/gim
来源：http://kha.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mmf.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ndu.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://qji.jqgufenzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://haz.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://gjo.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rpc.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oro.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zas.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ygs.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cos.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://enf.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zss.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hwu.zdbjq.cn

================================================================================
来源：http://gpj.cdnleiting.top

J. 日期与时间
来源：http://weh.xingfuxueyuan.xyz

================================================================================
来源：http://xcy.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://uyz.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bku.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tvw.aizwys.cn

JS:   new Date();  Date.now()
来源：http://xqh.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://kdi.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://wvt.xinyue.icu

Go:   time.Now()
来源：http://lhg.tarul.cn

Ruby: Time.now
来源：http://wdj.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://toj.bbcook.cn

[J02] 格式化输出
来源：http://dqr.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tun.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gqf.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hne.yueranfly.top

TS:   d.toISOString()
来源：http://rsh.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://obg.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jca.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eni.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qek.wangdashe.top

[J03] 字符串解析为日期
来源：http://dxm.jlsjyb.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bkr.fengsongda.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://erq.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://nlm.nanxinkj.top

TS:   new Date("2024-01-02")
来源：http://moq.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://ixq.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pgo.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://znk.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tvb.yfazqb.com

[J04] 时间戳与日期互转
来源：http://ksk.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vhb.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nhh.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tgw.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rvn.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aen.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://guz.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ogd.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uli.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://msz.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://mbl.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://grl.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://htc.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nqw.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://lmt.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://flx.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://slp.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://swo.xziqi.cn

[J06] 计算两时间之差
来源：http://fcd.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://ymt.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://ptp.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://amw.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gnf.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://zfa.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://vfi.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://bdu.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://rhv.yuanzhike.top

[J07] 比较两个日期
来源：http://mja.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://cag.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nmf.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oep.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zqr.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gne.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://esk.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://znx.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://xyn.tian-w.cn

[J08] 提取年月日与星期
来源：http://lyj.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rgm.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kbe.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ves.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kyr.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oyg.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://omk.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oan.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://psj.tarul.cn

[J09] 时区处理
来源：http://cpc.xingfuxueyuan.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qyc.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zva.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bcd.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzd.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hfp.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nke.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://abn.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zzt.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://ygk.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ync.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://drd.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://odj.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zmj.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://foj.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://omf.fehbvm.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tfc.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oer.ywan-chungtsiang.top

================================================================================
来源：http://wht.sweek.top

K. JSON 与序列化
来源：http://hge.fanxiaobao.xyz

================================================================================
来源：http://vld.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://gwt.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kcy.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vvr.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://gat.tarul.cn

TS:   JSON.stringify(obj)
来源：http://sxa.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wvf.dianchejie.cn

Go:   json.Marshal(obj)
来源：http://ajl.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lvw.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xok.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://fgn.wangdashe.top

Py:   json.loads(s)
来源：http://dhw.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pbe.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://cqw.yfazqb.com

TS:   JSON.parse(s)
来源：http://fxp.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rjg.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://egb.andypj.xyz

Ruby: JSON.parse(s)
来源：http://opj.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://byi.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://qbd.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ajc.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dgo.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dcz.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cjf.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ton.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ody.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://rah.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gpd.ybcxt.top

[K04] 读取 JSON 文件
来源：http://qls.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uyy.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pnn.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cru.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mpe.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://utu.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nok.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://gpr.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pbs.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://rjx.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://pxx.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://ogg.hammf.cn

JS:   structuredClone(obj)
来源：http://uns.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://spa.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nsp.fehbvm.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zos.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kjc.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lsh.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://dpc.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ylw.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ilb.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gsi.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lqw.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ppn.hongshengwenyu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cgi.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mdz.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ehk.kuanghao11.cn

[K07] 进制转换
来源：http://atd.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gxu.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ojl.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rkl.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://szh.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gbp.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jey.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zek.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qmm.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://ycw.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://hui.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pvl.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://bnn.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://bbs.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hil.yongpay.top

Go:   encoding/gob
来源：http://phf.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://wjf.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kra.xuetiantiany.cn

================================================================================
来源：http://mwg.svipenyu.cn

L. 网络请求
来源：http://tuc.jinghuilouyu.cn

================================================================================
来源：http://mow.jinqigufen.top

[L01] 发送 GET 请求
来源：http://pxd.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qfi.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fcb.hnxiangtu.top

JS:   await fetch(url)
来源：http://mfj.yangfankeji.com

TS:   await fetch(url)
来源：http://wjj.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wzu.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://vun.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://opz.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vtq.sufxvd.cn

[L02] 发送 POST JSON
来源：http://dya.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://zbc.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cre.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bsk.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pxs.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rkh.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://unm.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ahf.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hkg.shanyushiyangtech.top


<!-- 参考信息 -->