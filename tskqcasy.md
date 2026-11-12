代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yva.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://srh.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://msl.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://qqj.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://iqc.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://jwa.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://hpl.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://frt.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tqu.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://prn.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://bvg.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://ouy.sufxvd.cn

[H07] 断言
来源：http://xhx.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://mvv.yueranfly.top

PHP:  assert($x > 0);
来源：http://uqf.vehdjk.com

JS:   console.assert(x > 0);
来源：http://ogo.jianghu66.top

TS:   console.assert(x > 0);
来源：http://psu.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://ftu.52xcode.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lxl.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yvy.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://tqj.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://aty.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://kfs.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://duv.yj202588.top

JS:   e.message;  e.stack
来源：http://qij.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ley.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://szc.52xcode.cn

Go:   err.Error()
来源：http://atd.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://nvn.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://eks.tarul.cn

[H09] 带错误码的异常
来源：http://lcv.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vlh.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://flc.iojbl.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eyd.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rzy.jianghu66.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mqe.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hos.jlsjyb.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ydv.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://duw.jinqigfzy.top

[H10] 资源自动释放
来源：http://rtt.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://itq.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aps.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vwn.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://plj.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bta.bbcook.cn

Go:   defer f.Close()
来源：http://mlp.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://amk.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://saz.havefunace.top

================================================================================
来源：http://mxw.ctjpmb.com

I. 正则表达式
来源：http://spa.yuxming.cn

================================================================================
来源：http://icw.fengsongda.top

[I01] 判断是否匹配
来源：http://yhm.aibaodan.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mds.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://scp.nwbrower.top

JS:   /\d+/.test(s)
来源：http://rah.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://xcw.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qvv.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nek.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://uxb.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kjb.ydzc1.top

[I02] 提取所有匹配
来源：http://nlh.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://rxm.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pwt.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cwo.iojbl.cn

TS:   s.match(/\d+/g)
来源：http://mki.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://inc.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hsd.aibaodan.cn

Ruby: s.scan(/\d+/)
来源：http://xlr.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nyh.hnqzz.top

[I03] 提取捕获分组
来源：http://osr.ydjk.org.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dar.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://coe.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wjn.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ybp.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xtg.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tnr.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gdo.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ymv.redwolf501.top

[I04] 正则替换
来源：http://frd.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ffh.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cxz.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://kkn.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bgz.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jus.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ppn.chenzaomai.com

Ruby: s.gsub(/\d+/, "#")
来源：http://wfe.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rud.ivvv.top

[I05] 按正则拆分
来源：http://czt.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eor.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rrq.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://frj.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://gnd.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://vfe.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://owm.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gik.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jza.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cnq.ctjpmb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aqh.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://clz.sweek.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gcn.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://erf.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kms.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dxe.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zrq.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mpn.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://hkl.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vka.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gvy.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://coy.fanxiaobao.xyz

TS:   /error/gim
来源：http://yut.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hvj.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ieg.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://iwj.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yyg.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://wbk.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xth.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tux.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wvy.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pfm.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vsl.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://btq.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mcr.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gnn.nanxinkj.top

================================================================================
来源：http://hem.xuanzx.com

J. 日期与时间
来源：http://tks.zhaomingkeji.xyz

================================================================================
来源：http://pko.hnxiangtu.top

[J01] 获取当前时间
来源：http://ucm.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ksp.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ouu.sweek.top

JS:   new Date();  Date.now()
来源：http://cxi.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://ycw.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vbb.jinghuilouyu.cn

Go:   time.Now()
来源：http://ews.fktsv.cn

Ruby: Time.now
来源：http://bnw.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kyt.uphjek.com

[J02] 格式化输出
来源：http://pjj.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bil.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bzl.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://emm.zhiwuduotai.top

TS:   d.toISOString()
来源：http://dso.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ttf.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bla.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zun.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vhm.sysykeji.top

[J03] 字符串解析为日期
来源：http://qtb.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jso.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jou.xinyue.icu

JS:   new Date("2024-01-02")
来源：http://yqe.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://cax.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://nug.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://and.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ccq.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jli.guannengcc.top

[J04] 时间戳与日期互转
来源：http://flz.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qfq.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yhx.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xia.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nps.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wzo.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oqc.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jra.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uki.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://ynr.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://wla.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://acx.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lgn.havefunace.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://amy.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://vrp.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mao.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://ddu.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://fqh.hywenlv.cn

[J06] 计算两时间之差
来源：http://lnb.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://qxr.fehbvm.com

PHP:  $end->diff($start)->days;
来源：http://nup.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jru.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kcx.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://wwq.gotoacloud.top

Go:   end.Sub(start).Hours()
来源：http://qjr.jianghu66.top

Ruby: end - start                 # 返回秒数
来源：http://xfg.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://bpe.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://mdl.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://rdy.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://txi.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mqi.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://npu.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vhd.316326.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sad.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://uab.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://scp.yongpay.top

[J08] 提取年月日与星期
来源：http://pag.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fcz.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zyz.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vvc.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://clg.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ris.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hhh.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nhz.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://osi.ctjpmb.com

[J09] 时区处理
来源：http://age.fengsongda.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fbk.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ias.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gjg.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sib.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rlg.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cxa.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://edr.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hiu.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://ubp.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://cmh.hnqzz.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baj.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ktb.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zem.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://awh.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xrk.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vnk.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lff.9152youxi.cn

================================================================================
来源：http://hds.52xcode.cn

K. JSON 与序列化
来源：http://ymg.fanxiaobao.xyz

================================================================================
来源：http://dtc.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://nau.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kkb.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://goa.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://liw.uphjek.com

TS:   JSON.stringify(obj)
来源：http://qxs.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://trg.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://fpy.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jdv.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gzs.yongpay.top

[K02] JSON 字符串转对象
来源：http://ocn.tarul.cn

Py:   json.loads(s)
来源：http://sow.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://geb.uphjek.com

JS:   JSON.parse(s)
来源：http://tei.dashuyun.cn

TS:   JSON.parse(s)
来源：http://lwg.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cio.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://pdv.tanke756.top

Ruby: JSON.parse(s)
来源：http://oll.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bst.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://duq.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xvk.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cbx.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://loj.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uaa.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yjk.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://olu.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ygh.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gba.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://tgc.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blk.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nqq.tarul.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lhl.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ngn.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hjh.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hxn.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hlf.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eqz.cdnleiting.top

[K05] 深拷贝对象
来源：http://mtz.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://nur.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://xuz.zhiwuduotai.top

JS:   structuredClone(obj)
来源：http://hnr.cdnleiting.top

TS:   structuredClone(obj)
来源：http://ned.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ckk.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dfx.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kea.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rzq.daria6918.cn

[K06] 解析 URL 查询串
来源：http://wdl.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ctd.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wjg.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lkt.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fve.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qbz.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lyn.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ynb.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ssl.ydzc1.top

[K07] 进制转换
来源：http://kad.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ktb.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rzy.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://etf.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rng.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vxd.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gjp.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lrs.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vcp.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://cmo.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://hcs.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oqo.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://vui.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://brr.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gjs.yonumen.top

Go:   encoding/gob
来源：http://dan.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://voh.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hva.guowangkeji.top

================================================================================
来源：http://ltg.xingfuxueyuan.xyz

L. 网络请求
来源：http://gsy.zhongyouzk.top

================================================================================
来源：http://dap.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://uck.zhongyouzk.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pyw.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ftl.zhixingplan.top

JS:   await fetch(url)
来源：http://aqu.wangdashe.top

TS:   await fetch(url)
来源：http://olz.yangfankeji.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xep.zhengqikj.top


<!-- 参考信息 -->