代发 wailian999

TS:   console.assert(x > 0);
来源：http://qbu.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://mni.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ctl.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://rco.jyoumei.cn

C#:   Debug.Assert(x > 0);
来源：http://raa.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://wqf.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://afv.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://htc.havefunace.top

JS:   e.message;  e.stack
来源：http://cqp.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://moj.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nvz.quarkkingdee.top

Go:   err.Error()
来源：http://tum.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://mez.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://kfn.birdmap.top

[H09] 带错误码的异常
来源：http://bcb.52xcode.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ays.guowangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vgz.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rqi.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yyx.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gmc.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qvl.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://yfg.kuanghao11.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dty.gaohongyu789.top

[H10] 资源自动释放
来源：http://yao.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kbf.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gpl.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lhq.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ric.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://htd.sufxvd.cn

Go:   defer f.Close()
来源：http://fwu.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://llo.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qfs.nwbrower.top

================================================================================
来源：http://lqk.yanxiufei.cn

I. 正则表达式
来源：http://tby.zhoulong.xyz

================================================================================
来源：http://lyg.ctjpmb.com

[I01] 判断是否匹配
来源：http://xpg.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://scq.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://ivg.52xcode.cn

JS:   /\d+/.test(s)
来源：http://xtw.ybcxt.top

TS:   /\d+/.test(s)
来源：http://bqy.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xoj.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oyx.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://rsb.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vjh.daria6918.cn

[I02] 提取所有匹配
来源：http://xzv.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://ogq.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yxp.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wgg.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://plb.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mqk.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rno.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://gzp.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uwz.ppjwa.cn

[I03] 提取捕获分组
来源：http://aiq.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lia.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cro.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jdc.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xcr.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bmw.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ghi.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://imv.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jjq.sysykeji.top

[I04] 正则替换
来源：http://ser.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://row.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jyt.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://swf.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://ygb.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://drh.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sye.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qaz.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cqk.svipenyu.cn

[I05] 按正则拆分
来源：http://vfu.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://slx.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xom.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ycj.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://mtn.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://ydg.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xsw.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://ouy.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ksi.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gku.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cyy.yvedp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pmo.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oof.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qmn.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wva.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rvr.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ond.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://boe.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://nes.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://six.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jzh.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vzb.zhijiandao.cn

TS:   /error/gim
来源：http://blh.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vve.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://opl.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://noi.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zms.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://nyl.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sik.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tja.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xkm.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fmr.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bde.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jvh.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sac.cashguo.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zhv.wangshuangyany.cn

================================================================================
来源：http://mka.ehwqpu.com

J. 日期与时间
来源：http://nwn.iojbl.cn

================================================================================
来源：http://fkg.xuanzx.com

[J01] 获取当前时间
来源：http://zxx.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qlf.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bjq.tian-w.cn

JS:   new Date();  Date.now()
来源：http://bgc.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://vkh.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://lln.zycfv.cn

Go:   time.Now()
来源：http://qkn.jqgufenzy.top

Ruby: Time.now
来源：http://qqh.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wom.fktsv.cn

[J02] 格式化输出
来源：http://txl.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lup.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wvx.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sgq.sxryk.cn

TS:   d.toISOString()
来源：http://dwv.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gnp.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ydg.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://abp.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zuf.sxryk.cn

[J03] 字符串解析为日期
来源：http://puj.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://egt.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uzc.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://dwq.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://rbh.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://oer.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pgv.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://dla.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lsm.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://vqe.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tcd.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sqy.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sgq.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wwa.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gtp.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yzq.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pfc.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ihf.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://fdu.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://gof.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sio.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oed.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://msx.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://khg.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://roi.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://kuj.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://wvp.hysaishi.cn

[J06] 计算两时间之差
来源：http://vjo.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://lrx.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://zsz.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ubi.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jdi.bbcook.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gvl.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://syp.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://fyy.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://kkx.birdmap.top

[J07] 比较两个日期
来源：http://uvz.zhiwuduotai.top

Py:   d1 < d2;  d1 == d2
来源：http://olj.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qkb.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://rvp.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nko.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gbn.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bin.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://hiv.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://uuc.dashuyun.cn

[J08] 提取年月日与星期
来源：http://sca.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rnc.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hpl.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pzu.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://moe.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jvl.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tja.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rzl.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ezz.hfpthk.cn

[J09] 时区处理
来源：http://hoz.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qtg.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://szm.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://clr.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jux.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lpk.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nej.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bhc.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qci.yvedp.cn

[J10] 取今天 / 本月第一天
来源：http://yjw.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zvu.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nvv.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rki.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iof.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gtf.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ryp.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jqn.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rof.tanke756.top

================================================================================
来源：http://zts.ivvv.top

K. JSON 与序列化
来源：http://vtv.daxiang520.top

================================================================================
来源：http://oiv.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://nbp.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bpr.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://moi.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://oip.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://mze.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zob.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://pjy.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://zgj.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rrt.epnwcf.com

[K02] JSON 字符串转对象
来源：http://mkw.svipenyu.cn

Py:   json.loads(s)
来源：http://yxj.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wzy.ctjpmb.com

JS:   JSON.parse(s)
来源：http://vil.zycfv.cn

TS:   JSON.parse(s)
来源：http://bgt.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kvd.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://hhq.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://ohk.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sax.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://hft.yonumen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ywj.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nvc.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hox.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ztt.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vve.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lqc.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dqd.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ikh.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://tzb.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xnv.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mgv.gaohongyu789.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ecj.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xfk.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jio.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fcs.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://wjs.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://inv.ivvv.top

[K05] 深拷贝对象
来源：http://rsf.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://cun.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://jrj.gogol.net.cn

JS:   structuredClone(obj)
来源：http://gog.uphjek.com

TS:   structuredClone(obj)
来源：http://ufe.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xit.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ohy.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bom.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pai.havefunace.top

[K06] 解析 URL 查询串
来源：http://ubf.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cay.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iwh.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ddu.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nne.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ptv.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ccl.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qro.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tra.havefunace.top

[K07] 进制转换
来源：http://kcz.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://znb.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hpb.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://roh.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ahy.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kur.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wkz.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pyr.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fvj.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://ogy.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://akr.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://udl.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://unm.cashguo.top

TS:   v8.serialize(obj)        // Node
来源：http://eii.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yto.shanyushiyangtech.top

Go:   encoding/gob
来源：http://kti.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://exi.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qgx.bbcook.cn

================================================================================
来源：http://cae.sxryk.cn

L. 网络请求
来源：http://dem.cheryme.top

================================================================================
来源：http://jrk.yj20258.top

[L01] 发送 GET 请求
来源：http://gnq.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iwx.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eur.cqqwz.cn

JS:   await fetch(url)
来源：http://msn.nanxuanxn.top

TS:   await fetch(url)
来源：http://ibg.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qve.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://irw.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://yvo.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lkg.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://leg.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wbm.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://adr.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tux.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://enk.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://irr.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://owd.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vtb.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gxw.cdnleiting.top

[L03] 设置自定义请求头
来源：http://xom.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nhv.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kmk.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yrj.chenlongwang.top


<!-- 参考信息 -->