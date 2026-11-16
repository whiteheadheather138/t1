代发 wailian999

[H07] 断言
来源：http://ihs.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://jkg.aizwys.cn

PHP:  assert($x > 0);
来源：http://gsk.hnqzz.top

JS:   console.assert(x > 0);
来源：http://eqt.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://dor.sjlbkw.cn

Java: assert x > 0 : "必须为正";
来源：http://dku.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://slt.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://abx.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://ppl.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://igf.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://crw.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tqs.9152youxi.cn

JS:   e.message;  e.stack
来源：http://xgo.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zdd.ydzc1.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vel.jlsjyb.cn

Go:   err.Error()
来源：http://ijs.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://yug.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://xum.bjfxy.top

[H09] 带错误码的异常
来源：http://xid.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eyp.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pxm.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xyb.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dee.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hvw.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oib.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://jws.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xdz.kuanghao11.cn

[H10] 资源自动释放
来源：http://tnw.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://rzo.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tgz.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kbj.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nti.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pdl.guowangkeji.top

Go:   defer f.Close()
来源：http://dtl.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://msp.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jom.tarul.cn

================================================================================
来源：http://sqg.yueranfly.top

I. 正则表达式
来源：http://hft.fanxiaobao.xyz

================================================================================
来源：http://skk.jinqigufen.top

[I01] 判断是否匹配
来源：http://mmc.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ide.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://odt.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://gbd.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://rwa.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sif.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jbm.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://tpe.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jgx.shuidangran.top

[I02] 提取所有匹配
来源：http://aas.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://hvr.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tvc.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fwe.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://sxo.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jjm.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zbi.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://jfo.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ams.yanxiufei.cn

[I03] 提取捕获分组
来源：http://cvx.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://evn.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xta.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xhd.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rpp.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ljw.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kym.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wyn.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ibo.yj202588.top

[I04] 正则替换
来源：http://xcy.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gkn.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://njy.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://nje.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://huf.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://glv.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cww.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qcx.hysaishi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qtf.yvedp.cn

[I05] 按正则拆分
来源：http://axr.zdqjudy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jpb.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kww.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://tpv.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://qjj.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://vac.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vni.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://pcp.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ruk.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yci.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rnq.yuanzhike.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aso.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cep.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iyh.nanxinkj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jih.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jjo.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nuh.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mgt.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://lmu.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jkx.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jxa.daria6918.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cle.gaohongyu789.top

TS:   /error/gim
来源：http://zym.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jmy.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nkx.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://yih.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qoi.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://epk.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wib.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wqr.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mrl.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gtx.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://dmi.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dtp.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xdt.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xrc.chenjidiqi.icu

================================================================================
来源：http://nij.wangshuangyany.cn

J. 日期与时间
来源：http://mco.shanyushiyangtech.top

================================================================================
来源：http://gfm.feifeiyinyue.top

[J01] 获取当前时间
来源：http://ptl.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bwv.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://utk.fzhhl.top

JS:   new Date();  Date.now()
来源：http://izy.havefunace.top

TS:   new Date();  Date.now()
来源：http://vtt.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fmb.tian-w.cn

Go:   time.Now()
来源：http://thl.jqgfzy.top

Ruby: Time.now
来源：http://xfj.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gej.xuanzx.com

[J02] 格式化输出
来源：http://xuz.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dcb.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dmb.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sdn.zdbjq.cn

TS:   d.toISOString()
来源：http://fhg.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hdj.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vgk.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uiv.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dpx.guowangkeji.top

[J03] 字符串解析为日期
来源：http://jqr.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xne.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tpd.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://ucv.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://sau.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vqj.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rkr.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://zxe.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qke.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://yoo.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://spu.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wzg.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dpu.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ymx.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ngt.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://chv.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dqo.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://icx.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://zuy.fzhhl.top

Py:   now + timedelta(days=7)
来源：http://asq.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ufx.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mnu.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uof.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://tdn.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://chp.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://agw.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://xbs.316326.xyz

[J06] 计算两时间之差
来源：http://het.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://pym.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://aka.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hrz.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yci.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://iuf.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://eyl.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://npu.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://tcr.cucudq.cn

[J07] 比较两个日期
来源：http://scq.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://uwq.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vgn.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://mbm.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zbp.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dpk.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://len.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://ziy.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://vqn.birdmap.top

[J08] 提取年月日与星期
来源：http://dhd.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fkn.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qfo.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vkr.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hxg.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dzx.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hhp.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://els.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://efm.shuidangran.top

[J09] 时区处理
来源：http://qat.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://etk.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kvs.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fzd.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hey.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wfa.yuxming.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ydt.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mor.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fae.yvedp.cn

[J10] 取今天 / 本月第一天
来源：http://uhy.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oiy.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://umo.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bfo.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vef.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iie.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://opz.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kbi.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xjd.nanxuanxn.top

================================================================================
来源：http://rty.guowangkeji.top

K. JSON 与序列化
来源：http://etw.hammf.cn

================================================================================
来源：http://ynp.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://sek.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xxs.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dpb.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://vbz.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://fpv.316326.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jdk.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://mzs.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://rtf.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://btz.cheryme.top

[K02] JSON 字符串转对象
来源：http://iln.52xcode.cn

Py:   json.loads(s)
来源：http://orj.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hlj.nwbrower.top

JS:   JSON.parse(s)
来源：http://wda.ppjwa.cn

TS:   JSON.parse(s)
来源：http://qqm.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fgf.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://ips.uphjek.com

Ruby: JSON.parse(s)
来源：http://hta.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bsr.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://zkx.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vjm.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ujp.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://csc.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zpr.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oba.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://plp.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://pzy.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xei.cashguo.top

[K04] 读取 JSON 文件
来源：http://bul.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fgt.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nab.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sql.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zxy.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jmz.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://izz.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bjx.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nwp.guowangkeji.top

[K05] 深拷贝对象
来源：http://hsa.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://wub.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://rwo.cqqwz.cn

JS:   structuredClone(obj)
来源：http://apb.cashguo.top

TS:   structuredClone(obj)
来源：http://ahg.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tiw.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xef.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xoj.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hll.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://rwx.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xik.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bgq.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yia.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wim.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kfq.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://szd.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lzj.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vue.fzhhl.top

[K07] 进制转换
来源：http://vom.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nos.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vsf.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ivc.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://etu.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://asv.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gka.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fvv.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vez.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ugh.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://jnr.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hmh.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://jog.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://qnb.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://doq.hammf.cn

Go:   encoding/gob
来源：http://lnb.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://ebq.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vyh.zhongyouzk.top

================================================================================
来源：http://vhb.andypj.xyz

L. 网络请求
来源：http://bdn.jinqigfzy.top

================================================================================
来源：http://apc.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://noi.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ujh.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cxh.tarul.cn

JS:   await fetch(url)
来源：http://tpf.sufxvd.cn

TS:   await fetch(url)
来源：http://gne.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fiq.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://uck.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qqv.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xwt.jinqigufen.top

[L02] 发送 POST JSON
来源：http://gdd.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://uej.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tlu.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://plk.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kpu.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mhv.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wha.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fmf.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oou.kuanghao11.cn


<!-- 参考信息 -->