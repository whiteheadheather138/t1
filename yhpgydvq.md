代发 wailian999

Py:   value = d.get("k") or default
来源：http://run.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://tpo.jlsjyb.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uja.hcnkem.com

TS:   obj?.a?.b;  d ?? default
来源：http://gba.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://org.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lxr.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://vag.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://nuo.hesvh.cn

[H07] 断言
来源：http://jyj.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://tbi.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://dnz.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://ehq.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://lws.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://agq.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://irb.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nzc.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://tvy.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://jyi.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://imc.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rcz.jyoumei.cn

JS:   e.message;  e.stack
来源：http://xrb.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qkd.yuxming.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pzc.sufxvd.cn

Go:   err.Error()
来源：http://xsx.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://ffi.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://glj.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://suq.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fps.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pil.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aij.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yef.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hil.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sph.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://svt.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bqs.9152youxi.cn

[H10] 资源自动释放
来源：http://jce.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://amd.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sjt.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tny.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tkd.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cff.sxryk.cn

Go:   defer f.Close()
来源：http://cun.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ezh.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mdb.shuidangran.top

================================================================================
来源：http://ghb.nwbrower.top

I. 正则表达式
来源：http://jts.hysaishi.cn

================================================================================
来源：http://jab.ctjpmb.com

[I01] 判断是否匹配
来源：http://wxm.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ols.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://bxw.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://evm.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://yja.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vrs.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hnb.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://wwk.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sqz.gogol.net.cn

[I02] 提取所有匹配
来源：http://uvi.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://gkr.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xxp.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cjd.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://ewl.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://orb.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wai.shanyushiyangkeji.top

Ruby: s.scan(/\d+/)
来源：http://yhx.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yos.jiagoushi.top

[I03] 提取捕获分组
来源：http://gbj.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gic.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kwe.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pnw.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bzi.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ivx.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qme.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rqp.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rzm.epnwcf.com

[I04] 正则替换
来源：http://dqq.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qfi.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sjg.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://cbf.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zmf.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://rkn.cucudq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rqi.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://fzv.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lgp.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://tsy.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wea.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nrm.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://mir.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://kce.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://rdr.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ghd.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://knu.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://coa.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vvn.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wdj.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kqs.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ozi.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://unz.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oxg.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zzt.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qik.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xdc.snrcjt.cn

[I07] 忽略大小写与多行模式
来源：http://khl.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sfo.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rck.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ayt.birdmap.top

TS:   /error/gim
来源：http://uku.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hui.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dim.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://fxi.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nna.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://bex.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jfv.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ifv.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fyi.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kja.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://sgq.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mjz.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oin.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ugn.zhoulong.xyz

================================================================================
来源：http://gyh.jyoumei.cn

J. 日期与时间
来源：http://xaa.zhaomingkeji.xyz

================================================================================
来源：http://mub.chenzaomai.com

[J01] 获取当前时间
来源：http://stu.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://icq.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nnq.hnqzz.top

JS:   new Date();  Date.now()
来源：http://hgg.sxryk.cn

TS:   new Date();  Date.now()
来源：http://nvc.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sep.yonumen.top

Go:   time.Now()
来源：http://uak.kuanghao11.cn

Ruby: Time.now
来源：http://xic.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://inx.yuxming.cn

[J02] 格式化输出
来源：http://vrc.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nwx.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sbi.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wka.jiagoushi.top

TS:   d.toISOString()
来源：http://zwm.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kjs.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://frk.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ooj.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gcb.sufxvd.cn

[J03] 字符串解析为日期
来源：http://wqd.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fgv.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pwf.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://owy.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://mma.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://art.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rmg.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://tff.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fse.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://sub.ydjk.org.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aon.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ble.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wgh.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jzm.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wen.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wkq.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sph.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hxj.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://xni.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://mlr.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ofw.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://edf.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://att.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://hrk.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tgg.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://cnw.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://aut.yanxiufei.cn

[J06] 计算两时间之差
来源：http://xkm.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://mau.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://bes.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iqi.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dbn.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://vhi.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://sil.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://yox.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://ydj.zhongyouzk.top

[J07] 比较两个日期
来源：http://til.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://gtf.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eic.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://xmt.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nyn.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dhh.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pia.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://sni.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://sio.sufxvd.cn

[J08] 提取年月日与星期
来源：http://kiq.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mfx.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ycq.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bfu.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cun.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hmt.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dsj.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xoo.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pjj.zhiwuduotai.top

[J09] 时区处理
来源：http://ctm.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://liq.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hho.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qsv.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aki.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qus.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://awy.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://phj.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bxg.bbcook.cn

[J10] 取今天 / 本月第一天
来源：http://dkv.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://kau.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dka.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oxh.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tiy.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kfc.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pms.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vki.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ozs.zhoulong.xyz

================================================================================
来源：http://smo.uphjek.com

K. JSON 与序列化
来源：http://urq.zdbjq.cn

================================================================================
来源：http://ksu.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://cvy.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mkk.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dfb.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://mec.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://qya.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rev.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://iri.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://tdr.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oow.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://lns.hnqzz.top

Py:   json.loads(s)
来源：http://neh.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ljl.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://txu.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://htq.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ohp.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://cyg.bbcook.cn

Ruby: JSON.parse(s)
来源：http://xtp.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gwi.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://wqt.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pfn.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eho.shuidangran.top

JS:   JSON.stringify(obj, null, 2)
来源：http://obg.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nph.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xaa.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yha.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://swb.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://imt.cashguo.top

[K04] 读取 JSON 文件
来源：http://nof.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zmv.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ayu.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jef.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xvv.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mal.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tcv.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dad.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dok.jiagoushi.top

[K05] 深拷贝对象
来源：http://tky.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://dmy.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://rkj.jinyuanbaomall.cn

JS:   structuredClone(obj)
来源：http://dyn.ybcxt.top

TS:   structuredClone(obj)
来源：http://hot.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mnx.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qnh.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yas.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xmw.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://oia.yuxming.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ccz.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uth.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pqt.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tie.bjfxy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ydt.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fua.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wjo.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mww.ivvv.top

[K07] 进制转换
来源：http://hzr.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zln.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jtn.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nfb.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ypl.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rpu.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jcv.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ohw.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ybq.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://nqj.hammf.cn

Py:   pickle.dumps(obj)
来源：http://nef.xuanzx.com

PHP:  serialize($obj);  unserialize($s);
来源：http://aeh.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://plv.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://qyq.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zwb.yongpay.top

Go:   encoding/gob
来源：http://hyb.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://owi.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vnf.jianghu66.top

================================================================================
来源：http://lkq.bbcook.cn

L. 网络请求
来源：http://htf.jqgufenzy.top

================================================================================
来源：http://ndc.tianlin.xyz

[L01] 发送 GET 请求
来源：http://eox.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qav.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qvy.yfazqb.com

JS:   await fetch(url)
来源：http://tno.zhijiandao.cn

TS:   await fetch(url)
来源：http://dtw.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yje.wangshuangyany.cn

Go:   resp, err := http.Get(url)
来源：http://ppp.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://quf.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://klb.guowangkeji.top

[L02] 发送 POST JSON
来源：http://nmx.smart0.xyz


<!-- 参考信息 -->