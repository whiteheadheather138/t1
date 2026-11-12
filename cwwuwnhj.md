代发 wailian999

Py:   value = d.get("k") or default
来源：http://etg.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gbz.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://roo.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://sis.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gjd.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oft.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://wvt.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://xyy.chenzaomai.com

[H07] 断言
来源：http://xyv.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://yhe.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://bae.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://oxf.yuxming.cn

TS:   console.assert(x > 0);
来源：http://stc.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://mnz.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://trp.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yom.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://tsx.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://zpn.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://bkk.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uic.ybcxt.top

JS:   e.message;  e.stack
来源：http://xhy.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nmf.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hig.cheryme.top

Go:   err.Error()
来源：http://nst.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://rdk.nanxuanxn.top

C#:   e.Message;  e.StackTrace
来源：http://pik.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://tag.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xtn.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vea.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qer.yj202588.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rsh.daria6918.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ebm.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iyk.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://wxp.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ooi.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://edu.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kwr.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://osy.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tgu.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tps.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xju.yuanzhike.top

Go:   defer f.Close()
来源：http://ttz.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ifb.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hly.hesvh.cn

================================================================================
来源：http://rbk.wangshuangyany.cn

I. 正则表达式
来源：http://vpg.pengpengdd.cyou

================================================================================
来源：http://ddc.yj20258888.top

[I01] 判断是否匹配
来源：http://nac.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://etc.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cfn.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://yxy.ivvv.top

TS:   /\d+/.test(s)
来源：http://isz.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bgi.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dgl.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://gee.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ddz.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://bvp.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://eih.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kir.ydjk.org.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://che.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://kok.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pum.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rpe.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://kkm.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oum.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://cxn.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kdd.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xve.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lea.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fdj.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wkv.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hmu.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pkl.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wvp.fengsongda.top

[I04] 正则替换
来源：http://ytd.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fci.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vzw.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zfc.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://nfs.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://qll.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lvx.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://iuw.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yub.dashuyun.cn

[I05] 按正则拆分
来源：http://jyv.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://niw.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ksn.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://tgi.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://bxo.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://gto.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iob.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://jco.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cfm.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ckd.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://upz.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://clj.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gaz.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tny.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gpt.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ast.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fow.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qsz.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://xzs.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vza.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bhb.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lji.hongshengwenyu.top

TS:   /error/gim
来源：http://gbd.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tao.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gmn.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://caz.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vmm.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://udx.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ydn.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://riv.shuidangran.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://egi.bbcook.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rsa.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uhg.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://otz.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vhp.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bbc.tanke756.top

================================================================================
来源：http://zjh.yangfankeji.com

J. 日期与时间
来源：http://vvj.tanke756.top

================================================================================
来源：http://zzp.quarkkingdee.top

[J01] 获取当前时间
来源：http://poi.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zws.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yxw.andypj.xyz

JS:   new Date();  Date.now()
来源：http://boz.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://gqp.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nsk.meibo888.top

Go:   time.Now()
来源：http://rwo.redwolf501.top

Ruby: Time.now
来源：http://pbc.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gux.xylfe.cn

[J02] 格式化输出
来源：http://rav.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nin.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fwf.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yck.quarkkingdee.top

TS:   d.toISOString()
来源：http://tgs.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qra.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://maj.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jfm.hfpthk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kxi.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://qkf.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jyv.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kqm.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://kqb.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://ucr.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://oke.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iuh.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://drx.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://axm.hcnkem.com

[J04] 时间戳与日期互转
来源：http://fwi.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://afl.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mdz.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dpp.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dce.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eig.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hkj.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mmg.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vtt.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://eub.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://ayh.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://foz.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bvd.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://imf.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://siz.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xol.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://bct.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://myo.haohaochexian.top

[J06] 计算两时间之差
来源：http://xgg.yj20258.top

Py:   (end - start).total_seconds()
来源：http://afw.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://rsr.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cwp.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ffx.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tle.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://zxm.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://pyx.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://qdy.gzhubu.top

[J07] 比较两个日期
来源：http://adg.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://rmj.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kjx.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hbs.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sjx.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qhl.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sbi.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://dlq.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://ahz.yueranfly.top

[J08] 提取年月日与星期
来源：http://wpg.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bxn.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qui.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uuy.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qly.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bvo.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ygo.jinqigfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rfj.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xlz.mhx1999.top

[J09] 时区处理
来源：http://lcu.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ubv.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mtg.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sdo.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kfp.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ofu.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kei.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qkk.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vbc.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://aqb.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cil.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://won.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vfm.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yed.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://msp.jianghu66.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vha.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hwk.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfg.chenzaomai.com

================================================================================
来源：http://mrf.fehbvm.com

K. JSON 与序列化
来源：http://flj.zdqjudy.top

================================================================================
来源：http://xcs.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://ncc.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tid.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uzr.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://ied.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://nhk.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rtr.ybcxt.top

Go:   json.Marshal(obj)
来源：http://hzd.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tfd.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gto.ehwqpu.com

[K02] JSON 字符串转对象
来源：http://qcs.bjfxy.top

Py:   json.loads(s)
来源：http://fhf.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ird.andypj.xyz

JS:   JSON.parse(s)
来源：http://tgh.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://hoe.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qnz.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://avb.fktsv.cn

Ruby: JSON.parse(s)
来源：http://xnv.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://orq.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://fcv.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yaa.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ywz.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://orn.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ucd.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://umm.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xvo.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jdb.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ttj.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://rhp.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://urk.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://puj.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uvg.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gof.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yst.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hoy.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://fzy.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dsd.jyoumei.cn

[K05] 深拷贝对象
来源：http://mkj.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://neh.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://dca.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://oqe.c1oappe.top

TS:   structuredClone(obj)
来源：http://rxa.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ywr.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bsr.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bfm.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://enb.nwbrower.top

[K06] 解析 URL 查询串
来源：http://kpp.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kgz.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uko.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hmf.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jvl.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fdh.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ion.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zba.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ica.shanyushiyangkeji.top

[K07] 进制转换
来源：http://gzf.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yga.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pvv.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ics.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zjy.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kjs.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ytv.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fjv.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jnk.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://zzb.yj20258.top

Py:   pickle.dumps(obj)
来源：http://uwf.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rei.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://jyl.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://qxc.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ier.gotoacloud.top

Go:   encoding/gob
来源：http://oxy.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://mum.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pio.sweek.top

================================================================================
来源：http://zuq.shzxlz.cn

L. 网络请求
来源：http://qec.gotoacloud.top

================================================================================
来源：http://bcs.cdnleiting.top

[L01] 发送 GET 请求
来源：http://qad.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ftx.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gpc.daria6918.cn

JS:   await fetch(url)
来源：http://wlm.nwbrower.top

TS:   await fetch(url)
来源：http://egk.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qed.ehwqpu.com

Go:   resp, err := http.Get(url)
来源：http://vlx.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nnb.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tvt.hywenlv.cn

[L02] 发送 POST JSON
来源：http://oil.zycfv.cn


<!-- 参考信息 -->