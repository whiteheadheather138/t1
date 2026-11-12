代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ric.yj202588.top

Ruby: rescue ArgumentError => e
来源：http://mau.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://acr.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://puj.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://nwa.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://xdt.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://tmw.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://xgw.ydjk.org.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uih.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tzx.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://kts.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://xmk.zhijiandao.cn

[H07] 断言
来源：http://emf.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://kdi.zdqjudy.top

PHP:  assert($x > 0);
来源：http://rae.andypj.xyz

JS:   console.assert(x > 0);
来源：http://rbv.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://khi.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://arn.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hze.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nqc.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://tnr.feifeiyinyue.top

[H08] 获取错误信息与堆栈
来源：http://gjz.shuidangran.top

Py:   str(e);  traceback.format_exc()
来源：http://dii.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ztx.havefunace.top

JS:   e.message;  e.stack
来源：http://ubp.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zhc.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nnm.yuxming.cn

Go:   err.Error()
来源：http://xxx.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://pbi.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://irz.yj20258888.top

[H09] 带错误码的异常
来源：http://rig.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nwc.pycfn.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://yid.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://etl.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dql.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cit.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rep.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://omz.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mwo.ehwqpu.com

[H10] 资源自动释放
来源：http://eas.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bzj.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ybn.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://csv.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cdg.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xcd.jqgfzy.top

Go:   defer f.Close()
来源：http://wcl.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://krv.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mlo.fengsongda.top

================================================================================
来源：http://azk.vqdsnc.cn

I. 正则表达式
来源：http://tak.aizwys.cn

================================================================================
来源：http://gqq.316326.xyz

[I01] 判断是否匹配
来源：http://osb.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ewr.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ylu.fktsv.cn

JS:   /\d+/.test(s)
来源：http://xsw.yfazqb.com

TS:   /\d+/.test(s)
来源：http://qso.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://udl.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://crj.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://mzy.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://irb.birdmap.top

[I02] 提取所有匹配
来源：http://xak.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://tou.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qoo.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ngc.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://xai.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nxv.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ors.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://cyl.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tfq.hnqzz.top

[I03] 提取捕获分组
来源：http://pus.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xow.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ril.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://acp.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wcg.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://agd.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xvl.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eyu.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://brl.yanxiufei.cn

[I04] 正则替换
来源：http://nps.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qke.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pzx.yangfankeji.com

JS:   s.replace(/\d+/g, "#")
来源：http://ozc.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://sad.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://afd.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://oef.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://swo.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lzi.iojbl.cn

[I05] 按正则拆分
来源：http://iah.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://pgm.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://url.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://pwx.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://uze.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://epv.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ozy.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pij.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xmq.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gvz.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rnr.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zzr.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xqy.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sra.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vjn.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://txv.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kef.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ydw.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://zjv.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://drx.hnxiangtu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jkz.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fvt.shanyushiyangkeji.top

TS:   /error/gim
来源：http://nxe.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://faq.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vxv.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://ktj.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kxy.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://wvf.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://six.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cjz.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfu.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ata.yuanzhike.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://opq.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lva.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xna.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ylm.zhoulong.xyz

================================================================================
来源：http://mrk.tarul.cn

J. 日期与时间
来源：http://ccb.sufxvd.cn

================================================================================
来源：http://spk.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://rqj.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://kdj.cqqwz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ltl.ybcxt.top

JS:   new Date();  Date.now()
来源：http://vvs.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://rcd.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://okh.snrcjt.cn

Go:   time.Now()
来源：http://dii.shanyushiyangtech.top

Ruby: Time.now
来源：http://cjw.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ohw.ydjk.org.cn

[J02] 格式化输出
来源：http://tpj.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vda.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xwy.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://klw.xziqi.cn

TS:   d.toISOString()
来源：http://vib.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vth.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://psl.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wui.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://idr.bjfxy.top

[J03] 字符串解析为日期
来源：http://qhk.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jdd.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oez.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://tgd.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://juu.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://dgs.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ahf.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://agt.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dis.guannengcc.top

[J04] 时间戳与日期互转
来源：http://oza.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rao.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ibk.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://loa.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fht.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wqz.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ihp.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bsk.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://usy.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://ffo.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://ybi.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hbg.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lte.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://muc.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://bna.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vck.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://nqs.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://tdy.snrcjt.cn

[J06] 计算两时间之差
来源：http://amg.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://zic.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://icz.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://djv.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fwk.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jfc.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://ock.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://ycs.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://qyw.yj20258888.top

[J07] 比较两个日期
来源：http://ucr.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://ywm.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eif.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://voe.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sbl.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fkv.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sac.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://slm.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://oui.tarul.cn

[J08] 提取年月日与星期
来源：http://dya.0kj1m.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iys.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://orc.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tbp.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pnr.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fko.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vpf.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qzm.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ccl.guowangkeji.top

[J09] 时区处理
来源：http://lrf.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aor.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://app.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zjr.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rpa.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://djf.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bdv.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eiv.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://htj.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://snk.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yyq.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://noh.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yuk.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tti.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hkx.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hkq.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dzb.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uvv.xuanzx.com

================================================================================
来源：http://fdr.yangfankeji.com

K. JSON 与序列化
来源：http://chx.smart0.xyz

================================================================================
来源：http://rtl.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://iyl.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blm.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zjd.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://kas.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://fqd.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rvy.havefunace.top

Go:   json.Marshal(obj)
来源：http://miz.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://wzr.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ypc.52xcode.cn

[K02] JSON 字符串转对象
来源：http://mli.ctjpmb.com

Py:   json.loads(s)
来源：http://bzs.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rrm.tarul.cn

JS:   JSON.parse(s)
来源：http://fck.redwolf501.top

TS:   JSON.parse(s)
来源：http://qmy.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://osa.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://cas.bjfxy.top

Ruby: JSON.parse(s)
来源：http://yvr.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://foz.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://jbr.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kwr.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://njt.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ryi.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ibl.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://igh.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://soe.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mon.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xsd.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://jss.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aet.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ock.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ioq.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dhc.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ilm.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dkb.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ugf.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://arw.xylfe.cn

[K05] 深拷贝对象
来源：http://vea.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://izj.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://xfj.daria6918.cn

JS:   structuredClone(obj)
来源：http://scv.daria6918.cn

TS:   structuredClone(obj)
来源：http://qbr.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://nov.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fke.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://axt.ywan-chungtsiang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qfo.uphjek.com

[K06] 解析 URL 查询串
来源：http://wei.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iiu.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zuw.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yyn.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zqz.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vmx.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://dzr.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pzy.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lwl.c1oappe.top

[K07] 进制转换
来源：http://abn.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://piq.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jye.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mbg.wangshuangyany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zjs.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cqw.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lwk.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jeo.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qpb.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://dfi.uphjek.com

Py:   pickle.dumps(obj)
来源：http://xkm.zhaomingkeji.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://imd.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://rvl.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://ftd.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://doq.gotoacloud.top

Go:   encoding/gob
来源：http://oeb.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://htq.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zsm.jinqigufen.top

================================================================================
来源：http://inv.jqgufenzy.top

L. 网络请求
来源：http://guk.jyoumei.cn

================================================================================
来源：http://fvg.dashuyun.cn

[L01] 发送 GET 请求
来源：http://ytx.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://grb.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ydp.shangyingyoupin.top

JS:   await fetch(url)
来源：http://nen.uphjek.com

TS:   await fetch(url)
来源：http://udf.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gld.bbcook.cn


<!-- 参考信息 -->