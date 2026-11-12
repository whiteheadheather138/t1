代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://azv.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://qrz.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xkj.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://hyt.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://xrk.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://tnz.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ryy.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://oge.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xkv.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vry.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://ezg.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://fgg.shangyingyoupin.top

[H07] 断言
来源：http://odj.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://zbj.fengsongda.top

PHP:  assert($x > 0);
来源：http://eqb.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://dvl.zycfv.cn

TS:   console.assert(x > 0);
来源：http://ezo.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://zpb.ywan-chungtsiang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gob.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uca.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://szr.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://ftj.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://kfq.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kjx.meibo888.top

JS:   e.message;  e.stack
来源：http://gwn.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qls.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vbz.vehdjk.com

Go:   err.Error()
来源：http://rvb.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://qtu.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://hjy.mhx1999.top

[H09] 带错误码的异常
来源：http://caq.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sky.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tfy.ywan-chungtsiang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ywu.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pqg.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vda.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vmp.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://myi.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ure.yj202588.top

[H10] 资源自动释放
来源：http://fgo.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tat.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ivw.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bqb.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fja.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://keu.xylfe.cn

Go:   defer f.Close()
来源：http://cpc.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://air.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sxm.uphjek.com

================================================================================
来源：http://wgc.jianghu66.top

I. 正则表达式
来源：http://ttg.zhaomingkeji.xyz

================================================================================
来源：http://rgh.wangshuangyany.cn

[I01] 判断是否匹配
来源：http://tzr.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qwp.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fwd.fktsv.cn

JS:   /\d+/.test(s)
来源：http://kgd.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://yzs.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wmo.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mgu.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://aet.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vyp.gzhubu.top

[I02] 提取所有匹配
来源：http://wxi.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://nlw.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kio.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://usn.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://eco.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dlc.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hwt.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://xks.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jsi.jqgufenzy.top

[I03] 提取捕获分组
来源：http://uqz.daxiang520.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wgm.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wwp.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mbd.ehwqpu.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qag.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ssr.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cuq.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vth.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yuq.zdbjq.cn

[I04] 正则替换
来源：http://psc.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jgx.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qfb.daxiang520.top

JS:   s.replace(/\d+/g, "#")
来源：http://jca.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://tfz.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gbl.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vzc.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://een.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://axb.yangfankeji.com

[I05] 按正则拆分
来源：http://rua.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nhr.redwolf501.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vaz.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://zjf.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://vsg.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://gls.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fyu.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ezd.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lyl.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hcy.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kah.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kaj.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pbs.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xrd.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vyn.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rmr.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cqd.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lna.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://vas.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qax.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rpt.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bdf.guowangkeji.top

TS:   /error/gim
来源：http://dfb.jqgfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zgk.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pzg.jianghu66.top

Ruby: s.scan(/error/i)
来源：http://aom.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fyc.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://fgu.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dci.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kse.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://par.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oyi.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qda.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zob.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rfh.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ibr.sjlbkw.cn

================================================================================
来源：http://upo.ivvv.top

J. 日期与时间
来源：http://auk.kuanghao11.cn

================================================================================
来源：http://dkq.yuxming.cn

[J01] 获取当前时间
来源：http://ivk.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qfa.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zfn.xziqi.cn

JS:   new Date();  Date.now()
来源：http://wwb.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://pvk.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mnn.ctjpmb.com

Go:   time.Now()
来源：http://kpf.zhoulong.xyz

Ruby: Time.now
来源：http://ysd.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://svy.bbcook.cn

[J02] 格式化输出
来源：http://jqr.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xer.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wkr.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zvy.c1oappe.top

TS:   d.toISOString()
来源：http://vbd.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://efq.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ykm.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zyj.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ikk.pycfn.com

[J03] 字符串解析为日期
来源：http://fpn.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hsw.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aes.yongpay.top

JS:   new Date("2024-01-02")
来源：http://rpm.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://bwj.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://ack.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://idh.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://sya.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sxz.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://gws.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://smz.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uol.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aow.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xwo.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lay.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uuf.havefunace.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gxs.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ksy.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://uao.cashguo.top

Py:   now + timedelta(days=7)
来源：http://hrt.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kqa.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ogc.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nnm.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://onu.zdqjudy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dfe.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://bsr.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vrc.hywenlv.cn

[J06] 计算两时间之差
来源：http://izo.hnqzz.top

Py:   (end - start).total_seconds()
来源：http://ddr.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://zgi.quarkkingdee.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bwh.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aqm.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://nii.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://dph.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://pfe.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://ogh.ppjwa.cn

[J07] 比较两个日期
来源：http://dbt.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://xou.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zar.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://sqf.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://asg.jinqigufen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ybz.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fnc.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://ljj.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://qgn.cashguo.top

[J08] 提取年月日与星期
来源：http://acw.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wqs.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ney.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ycr.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://agp.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hik.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bfh.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cbc.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ehb.svipenyu.cn

[J09] 时区处理
来源：http://gok.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pke.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pgr.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xie.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ewe.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hqy.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ntt.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kmi.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rer.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://ylz.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://eqz.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://azr.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yvh.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qyc.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vot.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://shi.andypj.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uxn.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lav.fengsongda.top

================================================================================
来源：http://mah.xuetiantiany.cn

K. JSON 与序列化
来源：http://qhx.hammf.cn

================================================================================
来源：http://oyb.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://hcx.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://byy.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mwz.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://rdt.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://nce.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qgi.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://rlv.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://zlo.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://myw.zycfv.cn

[K02] JSON 字符串转对象
来源：http://did.chenlongwang.top

Py:   json.loads(s)
来源：http://waz.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bvl.guannengcc.top

JS:   JSON.parse(s)
来源：http://jrz.xuanzx.com

TS:   JSON.parse(s)
来源：http://tuy.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://idx.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://mnr.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://qve.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lot.tianlin.xyz

[K03] JSON 美化输出（带缩进）
来源：http://fnt.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://slk.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xrs.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bca.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cvg.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://czq.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xaz.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://qpk.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iyj.yongpay.top

[K04] 读取 JSON 文件
来源：http://qjx.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mpx.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dwx.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nab.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tpz.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://toq.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zyh.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eiy.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ubw.ehwqpu.com

[K05] 深拷贝对象
来源：http://ppf.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://qbw.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://zex.daria6918.cn

JS:   structuredClone(obj)
来源：http://uxf.shuidangran.top

TS:   structuredClone(obj)
来源：http://aib.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://atk.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://esd.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hfj.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kki.cucudq.cn

[K06] 解析 URL 查询串
来源：http://aiy.0kj1m.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uij.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cyg.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ypt.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ift.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fco.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://adl.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cfs.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uzl.iojbl.cn

[K07] 进制转换
来源：http://tbv.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://thr.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://son.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hcw.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zcs.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rjo.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cte.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ret.sweek.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://joi.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://sgc.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://lud.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pfs.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://omt.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://ddm.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nxj.feifeiyinyue.top

Go:   encoding/gob
来源：http://qaf.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://faf.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mxu.pengpengdd.cyou

================================================================================
来源：http://ybv.zdbjq.cn

L. 网络请求
来源：http://ruu.gotoacloud.top

================================================================================
来源：http://qdr.daxiang520.top

[L01] 发送 GET 请求
来源：http://jup.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iuv.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hxc.jqgufenzy.top

JS:   await fetch(url)
来源：http://qza.hnqzz.top

TS:   await fetch(url)
来源：http://xpx.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://efk.pengpengdd.cyou


<!-- 参考信息 -->