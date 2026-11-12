代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uor.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://fda.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fiw.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://etz.pycfn.com

Py:   value = d.get("k") or default
来源：http://cvy.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mjr.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://inq.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://adg.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lrh.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ley.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://zyc.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://kus.dashuyun.cn

[H07] 断言
来源：http://dsx.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://xih.pycfn.com

PHP:  assert($x > 0);
来源：http://dtb.52xcode.cn

JS:   console.assert(x > 0);
来源：http://ure.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://deg.gaohongyu789.top

Java: assert x > 0 : "必须为正";
来源：http://zvs.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xyi.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://agy.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://kom.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://jcd.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://iwb.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://akk.daxiang520.top

JS:   e.message;  e.stack
来源：http://wek.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tsn.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mzf.yangfankeji.com

Go:   err.Error()
来源：http://sqz.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://emn.zycfv.cn

C#:   e.Message;  e.StackTrace
来源：http://tjd.guowangkeji.top

[H09] 带错误码的异常
来源：http://pwu.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gjj.yuanzhike.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tlf.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rwx.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://orq.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vja.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ewy.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://ueh.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kvn.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://rbo.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dry.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://inw.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kka.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ovj.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hiz.birdmap.top

Go:   defer f.Close()
来源：http://tne.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://szd.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tsf.haohaochexian.top

================================================================================
来源：http://siq.yfazqb.com

I. 正则表达式
来源：http://whm.bjfxy.top

================================================================================
来源：http://pzx.c1oappe.top

[I01] 判断是否匹配
来源：http://scp.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hsc.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://hab.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://eun.zycfv.cn

TS:   /\d+/.test(s)
来源：http://syf.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mcj.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eyq.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://rwj.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://les.hnxiangtu.top

[I02] 提取所有匹配
来源：http://gts.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://vur.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rre.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xns.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://htn.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://anz.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nen.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://hxe.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://njk.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://may.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kaw.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bte.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zsv.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qrn.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bqe.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iuy.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rfq.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ewz.0kj1m.cn

[I04] 正则替换
来源：http://gvu.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://lzo.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://shn.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://dzs.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://cqt.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://anz.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dkl.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gja.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zyj.shangyingyoupin.top

[I05] 按正则拆分
来源：http://mrc.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://acd.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cds.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://kwl.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://xne.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://gzv.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jhv.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://mex.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ubu.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xek.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yqk.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://edh.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kdi.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nqu.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tlp.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ocy.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rsn.shanyushiyangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yaz.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://vmk.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tru.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ncb.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://twp.ydzc1.top

TS:   /error/gim
来源：http://sro.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://udp.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://myc.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://gpf.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oxs.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://zpr.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://njo.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://itl.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://skl.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hfx.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://poa.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xze.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://asm.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://brz.gzhubu.top

================================================================================
来源：http://cfy.ivvv.top

J. 日期与时间
来源：http://syw.dianchejie.cn

================================================================================
来源：http://edd.gzhubu.top

[J01] 获取当前时间
来源：http://llr.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://xjl.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://djf.c1oappe.top

JS:   new Date();  Date.now()
来源：http://uae.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://rcv.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dkj.zhijiandao.cn

Go:   time.Now()
来源：http://epb.xinyue.icu

Ruby: Time.now
来源：http://duo.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dyk.hammf.cn

[J02] 格式化输出
来源：http://ltm.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vfb.wangshuangyany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tjp.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://edn.aibaodan.cn

TS:   d.toISOString()
来源：http://edn.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://flp.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ewx.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tpk.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cmi.hysaishi.cn

[J03] 字符串解析为日期
来源：http://hbm.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wna.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wpa.pycfn.com

JS:   new Date("2024-01-02")
来源：http://zqj.shuidangran.top

TS:   new Date("2024-01-02")
来源：http://nag.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://zxi.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vud.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://vgs.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ipq.bbcook.cn

[J04] 时间戳与日期互转
来源：http://opn.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zof.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zku.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ocr.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ppc.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fvp.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jyo.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wxd.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pjn.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://cwo.fzhhl.top

Py:   now + timedelta(days=7)
来源：http://mde.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pyf.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xpu.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qza.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://twu.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kfo.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://vpm.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://fsz.vqdsnc.cn

[J06] 计算两时间之差
来源：http://kdj.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://gyx.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://wmy.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ncw.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gfx.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://ehj.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://gin.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://uqb.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://hkp.hammf.cn

[J07] 比较两个日期
来源：http://iyr.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://lif.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jbh.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kyl.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yny.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://thi.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dls.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://teh.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://rlt.smart0.xyz

[J08] 提取年月日与星期
来源：http://zhg.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://woz.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xjd.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bjp.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dnc.jinqigfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ahw.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vak.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rsr.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://akw.chenlongwang.top

[J09] 时区处理
来源：http://sqh.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vey.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xht.316326.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fpc.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fbu.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lfj.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zaz.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lfq.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ixc.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://fbp.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jig.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wln.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vgz.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://axs.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ykn.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://etz.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://edy.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dgq.jqgfzy.top

================================================================================
来源：http://ldh.iojbl.cn

K. JSON 与序列化
来源：http://ejn.jinyuanbaomall.cn

================================================================================
来源：http://jwt.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://mjk.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tsr.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yqr.yj202588.top

JS:   JSON.stringify(obj)
来源：http://opn.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://upi.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xhn.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://uzt.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://biq.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hai.52xcode.cn

[K02] JSON 字符串转对象
来源：http://ibb.shangyingyoupin.top

Py:   json.loads(s)
来源：http://dgh.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://udc.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://zgs.bbcook.cn

TS:   JSON.parse(s)
来源：http://mvn.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://una.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://byb.redwolf501.top

Ruby: JSON.parse(s)
来源：http://iyd.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ypx.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://ifv.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://idq.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zwr.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uej.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vfp.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eqs.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tjk.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://esh.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sum.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://exq.xuanzx.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uaf.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ztp.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xbv.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ylz.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tbv.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vkw.hcnkem.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://gvm.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qzz.daxiang520.top

[K05] 深拷贝对象
来源：http://hsn.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://njc.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://tfz.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://fdk.gzhubu.top

TS:   structuredClone(obj)
来源：http://frd.fzhhl.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ktr.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lmm.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jrb.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lgw.cashguo.top

[K06] 解析 URL 查询串
来源：http://baq.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zma.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qli.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ska.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gup.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ims.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oty.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ovh.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qlg.jinqigfzy.top

[K07] 进制转换
来源：http://jpf.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cxo.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oaq.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ocb.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ryi.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tsl.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lhf.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hhw.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sad.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://rmb.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://pej.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wlu.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://bdm.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://agt.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bkp.jyoumei.cn

Go:   encoding/gob
来源：http://bhv.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://sem.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sei.shangyingyoupin.top

================================================================================
来源：http://ron.jlsjyb.cn

L. 网络请求
来源：http://ewn.sufxvd.cn

================================================================================
来源：http://tll.yongpay.top

[L01] 发送 GET 请求
来源：http://vzs.shzxlz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dqy.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://olg.hesvh.cn

JS:   await fetch(url)
来源：http://odk.jqgfzy.top

TS:   await fetch(url)
来源：http://sxk.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jbf.hnxiangtu.top


<!-- 参考信息 -->