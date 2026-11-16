代发 wailian999

TS:   console.assert(x > 0);
来源：http://mlx.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://rut.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ndd.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wpg.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://odv.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://izr.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://rgd.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lgz.jinqigufen.top

JS:   e.message;  e.stack
来源：http://ggj.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ynf.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://cwr.sufxvd.cn

Go:   err.Error()
来源：http://cqt.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://uql.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://lcg.zhongyouzk.top

[H09] 带错误码的异常
来源：http://rdz.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ygw.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dfi.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jkl.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mqc.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iwv.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bmz.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://agf.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ufd.yfazqb.com

[H10] 资源自动释放
来源：http://pqg.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tri.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vmr.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fkc.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zih.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jif.chenzaomai.com

Go:   defer f.Close()
来源：http://cvf.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dof.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://irb.yj20258888.top

================================================================================
来源：http://fqx.hfpthk.cn

I. 正则表达式
来源：http://eid.bjfxy.top

================================================================================
来源：http://elx.yongpay.top

[I01] 判断是否匹配
来源：http://yrf.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://euy.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fdd.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://zlt.redwolf501.top

TS:   /\d+/.test(s)
来源：http://uzc.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kkk.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sbd.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://nae.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zqb.316326.xyz

[I02] 提取所有匹配
来源：http://skb.yanxiufei.cn

Py:   re.findall(r"\d+", s)
来源：http://yhk.fanxiaobao.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fww.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mik.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://cix.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bjp.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eku.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://dti.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nyl.shzxlz.cn

[I03] 提取捕获分组
来源：http://nwu.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rwy.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mdo.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qak.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vtb.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ccc.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qli.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cjs.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mcq.jiagoushi.top

[I04] 正则替换
来源：http://smf.zhoulong.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://eto.sjlbkw.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mtx.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://zjg.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://wkj.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://pmu.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uzz.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xxn.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hec.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://ulw.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://koc.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cly.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://hff.ydzc1.top

TS:   s.split(/\s*,\s*/)
来源：http://wsi.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://lqp.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://exi.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oww.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iuy.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oia.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jtj.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kfw.gaohongyu789.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://koa.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nrj.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bby.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uuf.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://olf.0kj1m.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://atg.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://xdw.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lfs.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pxe.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://crq.hysaishi.cn

TS:   /error/gim
来源：http://yjy.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tcu.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pli.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://lon.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hro.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://dts.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yic.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://igd.zhaomingkeji.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wyo.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vkg.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ihr.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wza.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vmx.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ctf.hcnkem.com

================================================================================
来源：http://vlc.cqqwz.cn

J. 日期与时间
来源：http://sto.zdbjq.cn

================================================================================
来源：http://mhc.shangyingyoupin.top

[J01] 获取当前时间
来源：http://vam.cashguo.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wdz.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cab.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://jot.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://idm.shangyingyoupin.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wlz.dianchejie.cn

Go:   time.Now()
来源：http://pym.quarkkingdee.top

Ruby: Time.now
来源：http://zdq.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ria.pengpengdd.cyou

[J02] 格式化输出
来源：http://xel.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zlu.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ovr.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pqe.nwbrower.top

TS:   d.toISOString()
来源：http://sgh.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fup.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://crz.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://imr.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ddz.guannengcc.top

[J03] 字符串解析为日期
来源：http://xxy.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nfz.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uzz.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://sqr.uphjek.com

TS:   new Date("2024-01-02")
来源：http://nkr.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://avv.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vqm.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://ubk.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cyt.vehdjk.com

[J04] 时间戳与日期互转
来源：http://dsc.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eer.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rsl.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wfu.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fyu.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vsp.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://btp.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hib.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rrd.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://qvb.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://qsy.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://spz.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vsh.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sma.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://ejg.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://koq.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://ryr.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://nrr.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://ocl.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://bjp.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://xtw.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://frp.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wtx.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mfr.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://pub.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://kjz.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://ylv.sysykeji.top

[J07] 比较两个日期
来源：http://awl.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://vpx.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qrn.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://jjq.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://viz.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lqj.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tqf.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://vrc.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://gwx.tianlin.xyz

[J08] 提取年月日与星期
来源：http://eki.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ebn.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zxv.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nzt.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bga.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://igb.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kvv.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ghy.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ely.ywan-chungtsiang.top

[J09] 时区处理
来源：http://abf.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ojz.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yhg.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ahh.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iwu.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uhh.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://des.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://con.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rzk.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://wfa.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fnz.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jsw.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oei.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cum.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mkr.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qqn.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wqf.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ibp.zycfv.cn

================================================================================
来源：http://smh.cashguo.top

K. JSON 与序列化
来源：http://ztn.yanxiufei.cn

================================================================================
来源：http://wme.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://tvf.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://icx.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ebv.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://qdr.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://yxc.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hjr.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://dnt.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://oar.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mko.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://ido.tarul.cn

Py:   json.loads(s)
来源：http://odi.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://exq.zdbjq.cn

JS:   JSON.parse(s)
来源：http://khi.birdmap.top

TS:   JSON.parse(s)
来源：http://zet.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jty.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://fxg.sweek.top

Ruby: JSON.parse(s)
来源：http://guy.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://imm.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://ejz.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wnp.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://arn.svipenyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wum.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://atq.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://imb.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ptp.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://rfy.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://myr.zhongyouzk.top

[K04] 读取 JSON 文件
来源：http://ace.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mpz.xuanzx.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ouj.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eav.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://joz.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bgv.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zkl.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pkq.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kfb.sjlbkw.cn

[K05] 深拷贝对象
来源：http://uxm.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://ysh.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://yjo.cheryme.top

JS:   structuredClone(obj)
来源：http://cdf.zdbjq.cn

TS:   structuredClone(obj)
来源：http://oft.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eus.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dhw.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dlc.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hka.c1oappe.top

[K06] 解析 URL 查询串
来源：http://czs.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dil.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gkc.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdl.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cuv.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://abc.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hie.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jdp.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aqt.zhoulong.xyz

[K07] 进制转换
来源：http://bpm.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xhb.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dtx.mhx1999.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hct.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cxp.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mgt.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mtb.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vxt.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dwm.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://srr.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://qho.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vcy.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://eaj.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://dfg.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tla.yueranfly.top

Go:   encoding/gob
来源：http://ahc.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://mje.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gtp.yj20258.top

================================================================================
来源：http://mmm.iojbl.cn

L. 网络请求
来源：http://utl.ywan-chungtsiang.top

================================================================================
来源：http://ict.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://zbp.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zvy.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qhq.yanxiufei.cn

JS:   await fetch(url)
来源：http://dlg.hysaishi.cn

TS:   await fetch(url)
来源：http://gcz.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qep.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://xzy.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dwh.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://upl.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://knu.ehwqpu.com

Py:   requests.post(url, json={"a": 1})
来源：http://ura.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bui.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ork.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kau.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oxv.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hid.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qvv.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jfk.dashuyun.cn

[L03] 设置自定义请求头
来源：http://mmh.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://etn.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kes.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ous.ydjk.org.cn


<!-- 参考信息 -->