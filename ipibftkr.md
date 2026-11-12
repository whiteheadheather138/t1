代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yjj.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://rrr.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://end.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://hxs.daria6918.cn

Py:   value = d.get("k") or default
来源：http://nlh.jqgufenzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://idc.jqgufenzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://rrn.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://sgd.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cmj.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ycp.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://efu.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://axu.xuanzx.com

[H07] 断言
来源：http://emd.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://qqo.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://hof.smart0.xyz

JS:   console.assert(x > 0);
来源：http://lmm.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://fel.yongpay.top

Java: assert x > 0 : "必须为正";
来源：http://yxi.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yru.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://ytc.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://adp.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://qdm.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://ccw.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cym.cucudq.cn

JS:   e.message;  e.stack
来源：http://myn.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pub.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://beo.jiagoushi.top

Go:   err.Error()
来源：http://bai.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://fnt.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://tqd.tanke756.top

[H09] 带错误码的异常
来源：http://rlt.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xlv.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://opi.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://psb.jqgufenzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lxb.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://njx.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pfn.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wqu.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://raa.hnqzz.top

[H10] 资源自动释放
来源：http://cex.smart0.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://avr.sysykeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gxc.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://giq.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yka.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zgv.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://hmu.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lgi.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://avl.uphjek.com

================================================================================
来源：http://igc.tian-w.cn

I. 正则表达式
来源：http://gqy.jinqigufen.top

================================================================================
来源：http://kii.xinyue.icu

[I01] 判断是否匹配
来源：http://rle.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bmv.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://ukp.cheryme.top

JS:   /\d+/.test(s)
来源：http://cme.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://kus.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nyw.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://joz.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://wvo.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bpq.dianchejie.cn

[I02] 提取所有匹配
来源：http://wna.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://xst.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tli.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://edo.cheryme.top

TS:   s.match(/\d+/g)
来源：http://pzd.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bia.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jyp.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://wab.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wip.svipenyu.cn

[I03] 提取捕获分组
来源：http://upw.hnxiangtu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cqi.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ckz.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aas.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cbh.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dmr.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://obt.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vtp.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ojl.nwbrower.top

[I04] 正则替换
来源：http://daj.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qyp.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qvy.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://kei.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hyn.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gxb.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yuo.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nty.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rym.sjlbkw.cn

[I05] 按正则拆分
来源：http://kbg.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kaw.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vjr.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://lcs.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://oid.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://dci.c1oappe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ahg.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://iwe.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kih.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fya.nwbrower.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rag.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://agb.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqm.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xlg.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lfw.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uyq.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vnn.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cah.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://yvu.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://akq.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ouw.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hrm.yvedp.cn

TS:   /error/gim
来源：http://cnr.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fkf.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hyq.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://wdk.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rfn.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://vbc.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tjr.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://akv.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://myh.bbcook.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gfl.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xij.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://muc.tanke756.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://apz.daxiang520.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vos.kuanghao11.cn

================================================================================
来源：http://pcc.hesvh.cn

J. 日期与时间
来源：http://cer.sjlbkw.cn

================================================================================
来源：http://jjs.dashuyun.cn

[J01] 获取当前时间
来源：http://hji.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://awk.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ver.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://qzg.ivvv.top

TS:   new Date();  Date.now()
来源：http://wob.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://shs.chenjidiqi.icu

Go:   time.Now()
来源：http://agh.sxryk.cn

Ruby: Time.now
来源：http://kxf.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://roq.yj20258888.top

[J02] 格式化输出
来源：http://hli.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lwu.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xur.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zvf.yj20258.top

TS:   d.toISOString()
来源：http://tao.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jfe.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dfk.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bgq.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://edd.9152youxi.cn

[J03] 字符串解析为日期
来源：http://rjl.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vpf.vehdjk.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://duc.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://gns.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://xkn.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://mnp.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kof.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://qaj.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wyf.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://qcx.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uwl.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eyx.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jmf.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qum.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dwr.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dbb.xinyue.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://orl.yonumen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zer.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://uki.sweek.top

Py:   now + timedelta(days=7)
来源：http://ysi.kuanghao11.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bkt.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xpw.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xbu.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://rih.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rlj.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://ynu.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://irx.fktsv.cn

[J06] 计算两时间之差
来源：http://fju.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://imi.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://zxa.yj20258888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cpm.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eom.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://bph.sweek.top

Go:   end.Sub(start).Hours()
来源：http://dpu.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://itd.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://rdg.guowangkeji.top

[J07] 比较两个日期
来源：http://wlt.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://ase.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sve.yj202588.top

JS:   d1.getTime() < d2.getTime()
来源：http://efb.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fjn.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bzw.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kmy.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bzt.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://xru.yuanzhike.top

[J08] 提取年月日与星期
来源：http://tjj.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fme.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sqm.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cer.cqqwz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eld.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ocu.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cfu.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://euh.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vqo.fzhhl.top

[J09] 时区处理
来源：http://gjr.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qkm.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jlo.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tbz.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rff.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uut.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://frz.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://zfv.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://squ.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://niz.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wii.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eca.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mod.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zet.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://npz.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nax.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://der.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kji.aizwys.cn

================================================================================
来源：http://bzj.cqqwz.cn

K. JSON 与序列化
来源：http://zia.c1oappe.top

================================================================================
来源：http://qhu.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://pth.bjfxy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gml.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gqk.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://evv.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://dtq.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://idv.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://nof.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yit.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fqj.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://vur.chenjidiqi.icu

Py:   json.loads(s)
来源：http://fxo.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xxu.52xcode.cn

JS:   JSON.parse(s)
来源：http://wbu.cashguo.top

TS:   JSON.parse(s)
来源：http://vsk.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tfm.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://cpr.xziqi.cn

Ruby: JSON.parse(s)
来源：http://zzi.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bjr.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://kqc.yonumen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hib.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ism.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fid.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ihf.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ysz.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ice.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://sep.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://snt.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://isn.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zmb.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://icd.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dcc.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oqo.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bju.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ook.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xzn.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uhu.316326.xyz

[K05] 深拷贝对象
来源：http://rob.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://bcn.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://hgr.hesvh.cn

JS:   structuredClone(obj)
来源：http://qzn.jinqigufen.top

TS:   structuredClone(obj)
来源：http://vvj.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://adk.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jgr.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zwj.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uqw.sweek.top

[K06] 解析 URL 查询串
来源：http://okk.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://usl.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ixs.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tap.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cgw.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ima.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ybj.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://emr.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rxk.ivvv.top

[K07] 进制转换
来源：http://cnj.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jlc.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dhz.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kbc.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pbh.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qze.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zue.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fwg.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dno.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://avo.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://dit.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hdv.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://lff.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://xzr.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cud.tanke756.top

Go:   encoding/gob
来源：http://ebg.fktsv.cn

Ruby: Marshal.dump(obj)
来源：http://dfg.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rzf.sjlbkw.cn

================================================================================
来源：http://udg.ppjwa.cn

L. 网络请求
来源：http://tdn.gzhubu.top

================================================================================
来源：http://jax.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://arf.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ryf.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mah.yueranfly.top

JS:   await fetch(url)
来源：http://new.redwolf501.top

TS:   await fetch(url)
来源：http://snw.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jvj.wangshuangyany.cn


<!-- 参考信息 -->