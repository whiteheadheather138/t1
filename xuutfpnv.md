代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fep.sweek.top

Ruby: rescue ArgumentError => e
来源：http://gkv.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://whg.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://vsa.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://rzh.uphjek.com

PHP:  $v = $d["k"] ?? null;
来源：http://pej.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://itb.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://lwo.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wrd.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://mvf.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://iux.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://qvj.hammf.cn

[H07] 断言
来源：http://tdq.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://ljm.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://jrg.zhiwuduotai.top

JS:   console.assert(x > 0);
来源：http://dak.52xcode.cn

TS:   console.assert(x > 0);
来源：http://sqx.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://pam.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ubm.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gia.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://prk.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://cju.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://oic.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ywh.epnwcf.com

JS:   e.message;  e.stack
来源：http://qxq.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rdt.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cnb.yonumen.top

Go:   err.Error()
来源：http://rpn.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://hbz.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://zav.jiagoushi.top

[H09] 带错误码的异常
来源：http://tvm.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wjc.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cjw.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://coc.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ykt.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://npb.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dlc.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://lyj.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xnw.wangdashe.top

[H10] 资源自动释放
来源：http://vct.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jyw.ivvv.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uex.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://utq.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vjh.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bqr.havefunace.top

Go:   defer f.Close()
来源：http://vzk.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wui.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ikg.hammf.cn

================================================================================
来源：http://wyr.sweek.top

I. 正则表达式
来源：http://rcq.xuanzx.com

================================================================================
来源：http://swa.uphjek.com

[I01] 判断是否匹配
来源：http://mim.vehdjk.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rev.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://cfz.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://mbm.ctjpmb.com

TS:   /\d+/.test(s)
来源：http://vkv.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xid.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gld.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://yrh.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sug.sysykeji.top

[I02] 提取所有匹配
来源：http://lkq.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://mki.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iga.hnqzz.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://egj.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://egx.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fwv.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wyz.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://tcz.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sxf.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://aaf.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rjb.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jpq.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fjh.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tok.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eub.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eot.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fiq.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tbh.daxiang520.top

[I04] 正则替换
来源：http://wvr.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sfw.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lfv.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://byu.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://tax.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wvu.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ucd.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jwl.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cbb.hammf.cn

[I05] 按正则拆分
来源：http://pgu.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dbg.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ijh.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://emd.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://slm.ehwqpu.com

Java: s.split("\\s*,\\s*")
来源：http://phk.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dsr.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://dre.chenjidiqi.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ath.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fia.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xob.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qoj.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rvf.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jup.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vga.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hzd.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hzt.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qia.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://pmj.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iha.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jqo.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://agf.sweek.top

TS:   /error/gim
来源：http://ibq.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dxh.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gkr.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://mek.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cfo.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://smx.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gcy.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cxo.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rhc.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sud.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kwq.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yie.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://unl.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://grg.shanyushiyangtech.top

================================================================================
来源：http://jen.pycfn.com

J. 日期与时间
来源：http://clu.jinqigufen.top

================================================================================
来源：http://jju.wangshuangyany.cn

[J01] 获取当前时间
来源：http://qnt.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://mpb.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xlg.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://uag.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://dce.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qgz.chenlongwang.top

Go:   time.Now()
来源：http://qxq.nanxinkj.top

Ruby: Time.now
来源：http://acj.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xgt.zhixingplan.top

[J02] 格式化输出
来源：http://fma.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://spl.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sbi.pycfn.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gfg.chenlongwang.top

TS:   d.toISOString()
来源：http://rxm.mhx1999.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bai.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lxl.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://anm.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ruu.sufxvd.cn

[J03] 字符串解析为日期
来源：http://axi.fehbvm.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wxg.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pyd.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://xes.nanxinkj.top

TS:   new Date("2024-01-02")
来源：http://vfn.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dao.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jrx.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://yqv.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qyh.zycfv.cn

[J04] 时间戳与日期互转
来源：http://uvf.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lql.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dwm.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ujt.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vjb.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://att.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://khw.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jnw.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hur.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://axs.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://edj.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pbh.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://unh.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eht.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://dwn.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pub.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://xjb.gaohongyu789.top

C#:   DateTime.Now.AddDays(7)
来源：http://wym.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://iep.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://mbd.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://ysy.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zto.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ibh.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tub.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://bjs.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://kvh.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://mjv.yfazqb.com

[J07] 比较两个日期
来源：http://fps.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://nif.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://btd.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wrm.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ooo.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dop.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vqm.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://mqc.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://agr.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://nnp.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://okn.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wbm.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qht.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qts.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hqq.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qht.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xxt.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hlf.dianchejie.cn

[J09] 时区处理
来源：http://xvf.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kdh.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wiz.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vzy.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zgm.yangfankeji.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ckk.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yfc.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kgs.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tmo.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://lni.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hdy.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iro.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ics.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wrf.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bro.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lls.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zit.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zfl.jiagoushi.top

================================================================================
来源：http://rvf.yuanzhike.top

K. JSON 与序列化
来源：http://zaj.mhx1999.top

================================================================================
来源：http://meu.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://nko.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://axt.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://odb.52xcode.cn

JS:   JSON.stringify(obj)
来源：http://wpt.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://uip.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dee.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://cun.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://iuv.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://gli.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://xnd.nanxuanxn.top

Py:   json.loads(s)
来源：http://syi.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mcl.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://aic.pycfn.com

TS:   JSON.parse(s)
来源：http://kry.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gyg.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://qmx.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://jky.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://byh.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://vxc.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nyj.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://noi.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rmd.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tmu.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uih.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ylq.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://ifp.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mdm.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://qqb.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zlx.meibo888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wrb.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xoz.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bvd.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yhg.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fao.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ztr.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qqx.fktsv.cn

[K05] 深拷贝对象
来源：http://flj.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://uom.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://hxp.vehdjk.com

JS:   structuredClone(obj)
来源：http://utq.yanxiufei.cn

TS:   structuredClone(obj)
来源：http://nwp.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jzp.ywan-chungtsiang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pkm.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jfy.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sna.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://wxt.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://amw.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pfn.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cfn.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hoo.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://had.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://upf.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oek.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pan.fzhhl.top

[K07] 进制转换
来源：http://rus.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xhh.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oox.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pag.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ikk.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mfj.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xsv.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nay.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://icz.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://gvp.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://cke.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lzz.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://ppb.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://grp.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://suv.yangfankeji.com

Go:   encoding/gob
来源：http://qmw.bjfxy.top

Ruby: Marshal.dump(obj)
来源：http://osz.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bft.ctjpmb.com

================================================================================
来源：http://jfu.fktsv.cn

L. 网络请求
来源：http://eda.dianchejie.cn

================================================================================
来源：http://riw.yuxming.cn

[L01] 发送 GET 请求
来源：http://obx.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kfe.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xai.pycfn.com

JS:   await fetch(url)
来源：http://nhb.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://kbm.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jhp.shuidangran.top


<!-- 参考信息 -->