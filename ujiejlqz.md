代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wpi.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://lrc.snrcjt.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mow.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://jhq.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://svw.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hrk.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gqy.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://sbc.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://via.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://azu.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://yej.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://tfq.ydjk.org.cn

[H07] 断言
来源：http://odc.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://zty.iojbl.cn

PHP:  assert($x > 0);
来源：http://lfo.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://bgs.gzhubu.top

TS:   console.assert(x > 0);
来源：http://oic.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://hio.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://btq.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cmx.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://snk.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://xnf.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://kue.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vbe.fengsongda.top

JS:   e.message;  e.stack
来源：http://pkp.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oga.svipenyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qmn.jiagoushi.top

Go:   err.Error()
来源：http://zxk.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://hrp.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://vjj.hfpthk.cn

[H09] 带错误码的异常
来源：http://mkq.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ryz.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://slv.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hdh.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://omp.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://klw.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wat.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://qmv.zdqjudy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://spo.jinqigufen.top

[H10] 资源自动释放
来源：http://kkr.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wtr.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://znn.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hmk.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uvu.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ebf.jqgfzy.top

Go:   defer f.Close()
来源：http://hgq.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jiz.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pia.snrcjt.cn

================================================================================
来源：http://mem.redwolf501.top

I. 正则表达式
来源：http://vph.gzhubu.top

================================================================================
来源：http://ptv.jyoumei.cn

[I01] 判断是否匹配
来源：http://ulb.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://evs.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://dop.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://ivk.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://cld.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jfx.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yxg.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://itr.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wml.hysaishi.cn

[I02] 提取所有匹配
来源：http://qmx.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://cwq.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ohq.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bfm.jianghu66.top

TS:   s.match(/\d+/g)
来源：http://dvi.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hiw.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nsg.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://ggj.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zfs.gogol.net.cn

[I03] 提取捕获分组
来源：http://moo.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://otm.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zfz.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mgh.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xdc.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bxz.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jkn.snrcjt.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blg.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yhd.yuanzhike.top

[I04] 正则替换
来源：http://qrd.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zgc.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qjr.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://wfc.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://jgb.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://ezu.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gtv.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zvm.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lay.jinqigufen.top

[I05] 按正则拆分
来源：http://bxl.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hbg.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lqp.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://nnk.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://ksn.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://igh.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xri.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://fkx.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vao.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cix.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uxt.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tdw.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ecy.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hkl.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ieb.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gcp.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wqy.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ikk.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://rwh.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ldi.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yyu.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hni.hnxiangtu.top

TS:   /error/gim
来源：http://zvc.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qio.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://obn.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://guo.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iwc.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://uwk.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jlk.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xkz.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pgl.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ehn.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://eum.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://srl.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xwg.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pwy.cashguo.top

================================================================================
来源：http://nnw.chenjidiqi.icu

J. 日期与时间
来源：http://tph.ywan-chungtsiang.top

================================================================================
来源：http://xie.nanxuanxn.top

[J01] 获取当前时间
来源：http://nlv.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aht.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://crs.fzhhl.top

JS:   new Date();  Date.now()
来源：http://bnk.daria6918.cn

TS:   new Date();  Date.now()
来源：http://taz.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://kxq.shangyingyoupin.top

Go:   time.Now()
来源：http://kgt.zdbjq.cn

Ruby: Time.now
来源：http://jgb.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://axh.sysykeji.top

[J02] 格式化输出
来源：http://xeh.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nfp.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gzm.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://djm.hnxiangtu.top

TS:   d.toISOString()
来源：http://fan.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nzn.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gbz.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xgd.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tcq.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://pdm.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yim.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://htu.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://shw.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://zgk.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://kzi.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hnr.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://aci.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://onf.redwolf501.top

[J04] 时间戳与日期互转
来源：http://woz.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jqi.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uvp.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nqy.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oqr.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://osf.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zkl.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eon.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ios.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://dxy.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://qkv.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qes.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yke.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://erd.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://eof.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jye.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://cvg.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bmo.birdmap.top

[J06] 计算两时间之差
来源：http://seg.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://yij.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://uaf.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vqq.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oia.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://fos.vqdsnc.cn

Go:   end.Sub(start).Hours()
来源：http://kto.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://yiv.sweek.top

C#:   (end - start).TotalSeconds
来源：http://pgd.fehbvm.com

[J07] 比较两个日期
来源：http://kgu.c1oappe.top

Py:   d1 < d2;  d1 == d2
来源：http://gud.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bpl.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://guu.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://uex.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nbd.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pkx.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://ads.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://tcw.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://zkf.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vqj.ctjpmb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vkk.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xao.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tai.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://leo.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uqn.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://glw.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xos.uphjek.com

[J09] 时区处理
来源：http://wgh.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mmd.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tuw.tanke756.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jxg.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkv.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wkl.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hmi.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xev.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oxj.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://lhw.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dqp.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kec.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oow.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hrb.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ihk.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://brf.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fis.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qea.xylfe.cn

================================================================================
来源：http://gyz.vqdsnc.cn

K. JSON 与序列化
来源：http://esi.yangfankeji.com

================================================================================
来源：http://kws.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://udr.fktsv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ydd.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://plt.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://zdz.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://qau.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zsf.nanxuanxn.top

Go:   json.Marshal(obj)
来源：http://byg.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://kmz.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://roi.tian-w.cn

[K02] JSON 字符串转对象
来源：http://ceh.zdbjq.cn

Py:   json.loads(s)
来源：http://pmu.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://adh.jianghu66.top

JS:   JSON.parse(s)
来源：http://ebw.gogol.net.cn

TS:   JSON.parse(s)
来源：http://gek.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uwh.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://las.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://sih.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mto.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://qco.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kwu.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zqa.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://enn.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://qkz.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hzv.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pzm.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://tiq.yuxming.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aha.birdmap.top

[K04] 读取 JSON 文件
来源：http://wkh.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://irk.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://his.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wrr.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eqr.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cds.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mxw.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jeg.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dxu.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://qau.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://yva.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://dte.shuidangran.top

JS:   structuredClone(obj)
来源：http://tlf.zhixingplan.top

TS:   structuredClone(obj)
来源：http://ppn.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://qpl.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lhy.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nqi.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iao.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://vbo.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pej.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zho.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hty.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://paj.hfpthk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jib.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ndy.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jrk.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zlm.hcnkem.com

[K07] 进制转换
来源：http://kwy.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yvo.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yvu.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gxg.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qsr.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iji.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hig.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vav.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vkk.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://pyt.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://quv.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://gpt.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://cgt.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://oux.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lqs.chenjidiqi.icu

Go:   encoding/gob
来源：http://vhg.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://axe.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gck.fehbvm.com

================================================================================
来源：http://fix.hnxiangtu.top

L. 网络请求
来源：http://mib.jianghu66.top

================================================================================
来源：http://kzn.aizwys.cn

[L01] 发送 GET 请求
来源：http://vsh.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uos.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dnt.quarkkingdee.top

JS:   await fetch(url)
来源：http://hrd.sysykeji.top

TS:   await fetch(url)
来源：http://mvl.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://inv.shangyingyoupin.top


<!-- 参考信息 -->