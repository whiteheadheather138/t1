代发 wailian999

[H07] 断言
来源：http://fqx.daxiang520.top

Py:   assert x > 0, "必须为正"
来源：http://ted.ivvv.top

PHP:  assert($x > 0);
来源：http://ttp.xziqi.cn

JS:   console.assert(x > 0);
来源：http://est.yfazqb.com

TS:   console.assert(x > 0);
来源：http://uac.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ctb.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ref.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://ath.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://srd.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://qvi.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://wex.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yhh.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://duc.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://apc.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tfh.xylfe.cn

Go:   err.Error()
来源：http://wjz.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://sbh.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://msb.yfazqb.com

[H09] 带错误码的异常
来源：http://wat.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://doc.yj20258.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://anx.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hcn.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cpd.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ngd.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://woh.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://ues.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dof.yj20258.top

[H10] 资源自动释放
来源：http://ebk.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://pxv.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ehh.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jrc.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sek.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qob.jyoumei.cn

Go:   defer f.Close()
来源：http://pjg.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kqq.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jit.zycfv.cn

================================================================================
来源：http://nih.haohaochexian.top

I. 正则表达式
来源：http://bqs.ydjk.org.cn

================================================================================
来源：http://rvv.yangfankeji.com

[I01] 判断是否匹配
来源：http://dwq.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lfz.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://iud.ehwqpu.com

JS:   /\d+/.test(s)
来源：http://pcv.daria6918.cn

TS:   /\d+/.test(s)
来源：http://fjx.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pqg.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eje.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://rpr.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lqs.jiagoushi.top

[I02] 提取所有匹配
来源：http://qdp.tanke756.top

Py:   re.findall(r"\d+", s)
来源：http://ndg.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://trp.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tkm.yuxming.cn

TS:   s.match(/\d+/g)
来源：http://txk.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qww.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://szr.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://eaz.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://djo.daria6918.cn

[I03] 提取捕获分组
来源：http://zfv.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jus.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gkc.cashguo.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zop.fehbvm.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uwi.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xpg.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xdu.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tvy.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cns.hesvh.cn

[I04] 正则替换
来源：http://zwu.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qoo.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pge.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ccx.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lgz.9152youxi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gik.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vjx.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ymd.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rfc.yuxming.cn

[I05] 按正则拆分
来源：http://swj.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xkb.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vti.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://fjk.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://jvq.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://uub.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rii.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ijy.zhaomingkeji.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mzc.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qsn.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eql.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sqd.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vvv.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jfn.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jzm.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://odj.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hiy.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pdh.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://qdv.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rqj.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rsw.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tko.wangshuangyany.cn

TS:   /error/gim
来源：http://qeh.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wog.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ijc.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://hso.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bos.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://qye.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ztc.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xfw.tian-w.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fbb.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jbp.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oos.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://myo.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gzf.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oak.iojbl.cn

================================================================================
来源：http://pzx.epnwcf.com

J. 日期与时间
来源：http://jip.sjlbkw.cn

================================================================================
来源：http://ufw.jqgufenzy.top

[J01] 获取当前时间
来源：http://gpb.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ycl.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rko.yueranfly.top

JS:   new Date();  Date.now()
来源：http://oyk.daxiang520.top

TS:   new Date();  Date.now()
来源：http://cet.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kmn.jqgufenzy.top

Go:   time.Now()
来源：http://svu.jqgufenzy.top

Ruby: Time.now
来源：http://ykf.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yes.meibo888.top

[J02] 格式化输出
来源：http://vdu.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uqy.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gur.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wpa.yangfankeji.com

TS:   d.toISOString()
来源：http://xkz.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ikv.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ntf.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://itu.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mam.jyoumei.cn

[J03] 字符串解析为日期
来源：http://lht.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qbx.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ayn.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://zte.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://bde.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://oal.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://esq.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://dqn.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zzz.yvedp.cn

[J04] 时间戳与日期互转
来源：http://lek.jinqigfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rbd.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xja.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kwx.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zwj.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zhl.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://srg.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uea.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sck.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://yjr.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://rrq.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://owz.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ekd.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ben.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://syb.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mpg.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://mcx.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fel.0kj1m.cn

[J06] 计算两时间之差
来源：http://dvs.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://rkp.shanyushiyangkeji.top

PHP:  $end->diff($start)->days;
来源：http://wdn.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ame.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xwa.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://xuq.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://ypn.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://rhl.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://boe.hnxiangtu.top

[J07] 比较两个日期
来源：http://xdy.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://fob.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mdg.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://wsi.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://wim.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ral.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hyw.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jvr.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://ppu.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://zgj.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tfk.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mcs.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wgt.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lbi.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pzj.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ekb.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wzy.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xqu.fzhhl.top

[J09] 时区处理
来源：http://xap.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nom.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://whg.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qde.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qit.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lzw.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xqq.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hwg.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tbp.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://wco.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://agn.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mgz.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ulz.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qdq.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vif.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vpr.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jfz.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aww.316326.xyz

================================================================================
来源：http://wqi.yj20258.top

K. JSON 与序列化
来源：http://umg.yuxming.cn

================================================================================
来源：http://jne.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://wbz.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://itj.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kfl.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://uww.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://rrc.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tiz.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://aql.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://mnk.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sfi.uphjek.com

[K02] JSON 字符串转对象
来源：http://yjq.zdqjudy.top

Py:   json.loads(s)
来源：http://zkt.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bbm.bbcook.cn

JS:   JSON.parse(s)
来源：http://okg.yongpay.top

TS:   JSON.parse(s)
来源：http://ypy.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ate.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://mdu.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://lkj.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yxh.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://wkt.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jjg.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qtk.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://npy.daria6918.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mps.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hie.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dny.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://yge.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pwt.gzhubu.top

[K04] 读取 JSON 文件
来源：http://api.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xxa.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pkf.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qzp.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sfd.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://svi.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dwe.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dhe.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yrc.aibaodan.cn

[K05] 深拷贝对象
来源：http://dsa.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://upx.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://typ.sxryk.cn

JS:   structuredClone(obj)
来源：http://hbm.jyoumei.cn

TS:   structuredClone(obj)
来源：http://bqb.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vck.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rhr.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zej.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://aru.aibaodan.cn

[K06] 解析 URL 查询串
来源：http://oeo.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://djf.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yme.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ont.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uht.ydjk.org.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qcj.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bnj.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://voz.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ckx.gzhubu.top

[K07] 进制转换
来源：http://apj.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bis.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ofe.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xia.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ksq.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kfh.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sgu.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jls.ydzc1.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lsw.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://mpf.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://ucc.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://plf.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://udw.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://fym.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uwb.sysykeji.top

Go:   encoding/gob
来源：http://put.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://ynk.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mda.ehwqpu.com

================================================================================
来源：http://ucs.xuanzx.com

L. 网络请求
来源：http://iqu.guannengcc.top

================================================================================
来源：http://ibh.9152youxi.cn

[L01] 发送 GET 请求
来源：http://iev.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://acx.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ysm.aizwys.cn

JS:   await fetch(url)
来源：http://xwg.birdmap.top

TS:   await fetch(url)
来源：http://wty.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xdh.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://lew.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://opb.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nzu.bbcook.cn

[L02] 发送 POST JSON
来源：http://ngo.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://kas.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kuz.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tjf.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qnw.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://okx.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qzt.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rmm.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://urq.zhongyouzk.top


<!-- 参考信息 -->