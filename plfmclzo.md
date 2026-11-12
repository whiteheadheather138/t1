代发 wailian999

[H07] 断言
来源：http://jsb.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://wii.tian-w.cn

PHP:  assert($x > 0);
来源：http://wwr.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://hsd.uphjek.com

TS:   console.assert(x > 0);
来源：http://lqk.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://evi.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://csr.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://afh.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://dss.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://huo.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://gge.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qbl.yuxming.cn

JS:   e.message;  e.stack
来源：http://dnd.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lut.cheryme.top

Java: e.getMessage();  e.printStackTrace()
来源：http://eqa.shanyushiyangtech.top

Go:   err.Error()
来源：http://fix.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://frp.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://xgg.nwbrower.top

[H09] 带错误码的异常
来源：http://dxj.shanyushiyangtech.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ylk.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tjt.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dmb.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://abw.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://els.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sjj.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://arl.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jrm.vqdsnc.cn

[H10] 资源自动释放
来源：http://zcq.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ulm.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://afr.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://psv.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ekm.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ytf.nwbrower.top

Go:   defer f.Close()
来源：http://ouy.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lia.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hra.ydzc1.top

================================================================================
来源：http://ixh.birdmap.top

I. 正则表达式
来源：http://ezg.epnwcf.com

================================================================================
来源：http://pzt.guannengcc.top

[I01] 判断是否匹配
来源：http://kxu.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ydq.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://yiz.daxiang520.top

JS:   /\d+/.test(s)
来源：http://xsa.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://mue.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://phl.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bnm.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://ghk.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://afh.shzxlz.cn

[I02] 提取所有匹配
来源：http://bma.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://wmi.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cys.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ewn.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://fix.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sed.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iuc.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://vzw.xylfe.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dhy.ybcxt.top

[I03] 提取捕获分组
来源：http://bax.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eia.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://drq.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://btx.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ebi.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nmu.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nyt.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vvd.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zws.ivvv.top

[I04] 正则替换
来源：http://ama.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jgy.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yqt.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://khs.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zyq.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lsd.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nua.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fix.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://muj.sjlbkw.cn

[I05] 按正则拆分
来源：http://mqy.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://prp.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qtg.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://ocj.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://omz.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://oyx.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lhh.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nad.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qjj.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://skm.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://upn.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uxr.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gbw.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rbq.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mtc.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gpv.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pit.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://awz.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://jkv.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qvk.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://udf.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wjc.jinghuilouyu.cn

TS:   /error/gim
来源：http://ipi.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zvf.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cte.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://hvp.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://drf.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://jei.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://chw.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://drk.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rcz.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uex.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bbs.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://suk.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wky.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dcn.hnqzz.top

================================================================================
来源：http://bfy.tianlin.xyz

J. 日期与时间
来源：http://cdc.yj202588.top

================================================================================
来源：http://cjl.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://bvd.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://geb.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://umi.xziqi.cn

JS:   new Date();  Date.now()
来源：http://rlg.fehbvm.com

TS:   new Date();  Date.now()
来源：http://tyu.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yux.ywan-chungtsiang.top

Go:   time.Now()
来源：http://vvm.bjfxy.top

Ruby: Time.now
来源：http://rpo.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tui.zdbjq.cn

[J02] 格式化输出
来源：http://xxc.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ecs.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nxs.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hyp.vqdsnc.cn

TS:   d.toISOString()
来源：http://kji.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cjd.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hfl.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tvf.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zpl.redwolf501.top

[J03] 字符串解析为日期
来源：http://tbm.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pfs.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wqo.uphjek.com

JS:   new Date("2024-01-02")
来源：http://ghw.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://cwm.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://tcy.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vuv.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://xqb.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ssq.jianghu66.top

[J04] 时间戳与日期互转
来源：http://wao.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bex.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rrw.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oog.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cdp.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mfs.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gis.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rkk.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wms.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://koj.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://lua.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://aag.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jbr.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mzv.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://bzn.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zkk.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://ofw.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://htm.uphjek.com

[J06] 计算两时间之差
来源：http://rbh.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://swd.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://dbl.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vfk.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fvj.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://yae.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://dri.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://oec.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://rnt.cheryme.top

[J07] 比较两个日期
来源：http://ycc.nanxuanxn.top

Py:   d1 < d2;  d1 == d2
来源：http://cjv.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iln.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://qav.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://nsh.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uiz.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hfp.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jkq.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://fll.hesvh.cn

[J08] 提取年月日与星期
来源：http://afz.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vxs.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tie.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eoc.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gaq.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uam.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hny.shuidangran.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jjt.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hei.ybcxt.top

[J09] 时区处理
来源：http://lbm.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vgu.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nza.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mdx.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://piu.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://whd.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://asl.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ucj.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ufo.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://hcq.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rvu.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cmn.9152youxi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://azq.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ynu.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gsp.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wzm.fehbvm.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gmw.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eza.daria6918.cn

================================================================================
来源：http://gmt.ydjk.org.cn

K. JSON 与序列化
来源：http://zao.jinqigfzy.top

================================================================================
来源：http://tzx.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://apf.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gsn.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ibo.tanke756.top

JS:   JSON.stringify(obj)
来源：http://iyd.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://uax.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://buk.ivvv.top

Go:   json.Marshal(obj)
来源：http://ksc.316326.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ype.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zee.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://uoa.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://gay.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qkr.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://syu.52xcode.cn

TS:   JSON.parse(s)
来源：http://lyv.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pni.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://wqp.sxryk.cn

Ruby: JSON.parse(s)
来源：http://pnc.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tao.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://rgj.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://plb.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ikz.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ofv.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bmp.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jsp.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yrl.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cvy.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yxm.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://pds.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hhb.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dgp.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tjn.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://znx.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qrk.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fpc.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tcb.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sfc.yonumen.top

[K05] 深拷贝对象
来源：http://gso.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://bod.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://wnp.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://wzp.jyoumei.cn

TS:   structuredClone(obj)
来源：http://sfw.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gbk.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://stf.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mnk.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://thx.bbcook.cn

[K06] 解析 URL 查询串
来源：http://nza.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kwa.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://des.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rrr.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agj.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nyt.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fzp.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iyy.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://guz.dianchejie.cn

[K07] 进制转换
来源：http://nmh.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ajl.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gpq.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ybc.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tcp.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fxp.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rrh.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qsx.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://icq.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://kpl.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://stx.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fzi.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://csd.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://cwr.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fzh.zhixingplan.top

Go:   encoding/gob
来源：http://mfd.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://itb.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lpx.316326.xyz

================================================================================
来源：http://czr.jqgufenzy.top

L. 网络请求
来源：http://wve.zhiwuduotai.top

================================================================================
来源：http://efx.yvedp.cn

[L01] 发送 GET 请求
来源：http://ihd.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ceu.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ypw.yueranfly.top

JS:   await fetch(url)
来源：http://kfl.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://wlm.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pii.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://phl.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://lvv.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wzu.jqgfzy.top

[L02] 发送 POST JSON
来源：http://dxl.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://qqh.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tjg.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://awq.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fla.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zog.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ynm.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bgb.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://knt.xylfe.cn


<!-- 参考信息 -->