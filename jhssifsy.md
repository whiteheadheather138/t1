代发 wailian999

[H07] 断言
来源：http://hvg.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://ldc.epnwcf.com

PHP:  assert($x > 0);
来源：http://exs.wangdashe.top

JS:   console.assert(x > 0);
来源：http://vey.sysykeji.top

TS:   console.assert(x > 0);
来源：http://nou.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://zwj.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hko.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://wih.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://pvr.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://cuj.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://qxm.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://thx.yangfankeji.com

JS:   e.message;  e.stack
来源：http://lsp.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tfe.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://uul.shangyingyoupin.top

Go:   err.Error()
来源：http://geo.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://jyo.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://obf.zycfv.cn

[H09] 带错误码的异常
来源：http://ubr.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xym.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jxd.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ome.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mwq.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dfp.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qpm.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://zsk.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mza.hysaishi.cn

[H10] 资源自动释放
来源：http://bue.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hdu.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://szl.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://spj.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wpr.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://afj.feifeiyinyue.top

Go:   defer f.Close()
来源：http://klo.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fzg.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jqg.yfazqb.com

================================================================================
来源：http://ftv.cheryme.top

I. 正则表达式
来源：http://exf.daria6918.cn

================================================================================
来源：http://idn.jinqigufen.top

[I01] 判断是否匹配
来源：http://iel.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sai.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://tbq.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://kaa.yonumen.top

TS:   /\d+/.test(s)
来源：http://sfo.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://idn.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sch.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://vyg.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://usc.wangdashe.top

[I02] 提取所有匹配
来源：http://hws.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://omi.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pyr.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ret.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://yts.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nif.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jgd.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://lay.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zhc.fengsongda.top

[I03] 提取捕获分组
来源：http://tak.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xsu.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kvk.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ceb.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mdk.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rlr.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xrc.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zaj.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eis.meibo888.top

[I04] 正则替换
来源：http://fjw.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://efq.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uuz.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zjr.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://dmr.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://kht.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mno.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://wry.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yli.52xcode.cn

[I05] 按正则拆分
来源：http://ike.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dbp.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ikp.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://hkr.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://tgg.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://rel.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gid.tian-w.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qxq.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tro.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://age.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ehg.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iqu.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uae.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nox.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dby.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qkv.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cph.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mbg.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://zps.0kj1m.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://new.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oim.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cas.shanyushiyangtech.top

TS:   /error/gim
来源：http://ihf.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://syn.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ysq.dashuyun.cn

Ruby: s.scan(/error/i)
来源：http://jkm.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dnq.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://zjk.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://htk.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lsh.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://inm.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zrq.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wrx.ybcxt.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ymy.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mje.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qvd.jinghuilouyu.cn

================================================================================
来源：http://nea.cashguo.top

J. 日期与时间
来源：http://yxb.hfpthk.cn

================================================================================
来源：http://hbo.zhengqikj.top

[J01] 获取当前时间
来源：http://woh.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ygj.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nhd.fktsv.cn

JS:   new Date();  Date.now()
来源：http://iis.shuidangran.top

TS:   new Date();  Date.now()
来源：http://szp.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://xzx.chenlongwang.top

Go:   time.Now()
来源：http://ujm.jinqigufen.top

Ruby: Time.now
来源：http://njh.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rxa.shuidangran.top

[J02] 格式化输出
来源：http://dbu.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://unx.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qeo.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://utz.zdqjudy.top

TS:   d.toISOString()
来源：http://kht.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hlg.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vpc.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pud.ywan-chungtsiang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tln.tian-w.cn

[J03] 字符串解析为日期
来源：http://jme.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ahi.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qhz.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://cyk.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://ufj.xinyue.icu

Java: LocalDate.parse("2024-01-02")
来源：http://jgk.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://csu.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://lpi.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sov.sweek.top

[J04] 时间戳与日期互转
来源：http://rnd.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pmb.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://agw.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sui.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dpq.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mup.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xsh.pycfn.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ast.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://osa.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://vpb.meibo888.top

Py:   now + timedelta(days=7)
来源：http://rkj.yanxiufei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rog.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mgx.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uhc.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://hrs.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xsv.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://gox.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vuz.yj20258.top

[J06] 计算两时间之差
来源：http://loa.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://ubv.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://kxt.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uft.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xhq.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://oiw.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://ciw.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://nyt.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://zce.cucudq.cn

[J07] 比较两个日期
来源：http://bhi.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://eht.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xze.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wls.tanke756.top

TS:   d1.getTime() < d2.getTime()
来源：http://pia.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pwu.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ipt.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://yga.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://pyo.xuanzx.com

[J08] 提取年月日与星期
来源：http://fgm.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wzu.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ftr.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://igj.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yws.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bjb.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ben.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xua.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://akk.ppjwa.cn

[J09] 时区处理
来源：http://mzp.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nac.ywan-chungtsiang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://art.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vlj.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oyh.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xev.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qab.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://udz.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gsy.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://qpa.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qrd.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xhx.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ymo.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zys.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sff.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nwe.hfpthk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zjx.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vgl.xuanzx.com

================================================================================
来源：http://uzu.gotoacloud.top

K. JSON 与序列化
来源：http://pcs.gaohongyu789.top

================================================================================
来源：http://era.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://dao.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gkv.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pzq.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://rxh.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://fls.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ywa.yvedp.cn

Go:   json.Marshal(obj)
来源：http://wfl.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://jbu.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://amg.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://nqa.epnwcf.com

Py:   json.loads(s)
来源：http://yre.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zii.0kj1m.cn

JS:   JSON.parse(s)
来源：http://wgj.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://koz.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wlf.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://nmg.yj20258.top

Ruby: JSON.parse(s)
来源：http://yvx.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vxg.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://zkf.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://liw.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cei.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rvc.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rby.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://njg.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kvj.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rtx.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fza.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://fmn.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mud.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fhi.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lxs.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tub.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eur.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mnl.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://otn.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lli.ybcxt.top

[K05] 深拷贝对象
来源：http://rsb.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://kjq.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://uhj.xinyue.icu

JS:   structuredClone(obj)
来源：http://muf.xziqi.cn

TS:   structuredClone(obj)
来源：http://awp.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ttv.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ksu.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cvh.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yrv.bjfxy.top

[K06] 解析 URL 查询串
来源：http://cfm.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kpd.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hjj.xuanzx.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hgq.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kgg.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mtl.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bph.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ttn.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eiy.hfpthk.cn

[K07] 进制转换
来源：http://mdj.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oso.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sph.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://auu.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rje.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gfr.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ybd.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mgs.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gjh.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://zmw.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://usw.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mru.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://wpx.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://eic.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cfn.tianlin.xyz

Go:   encoding/gob
来源：http://hiu.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://itd.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lnc.tanke756.top

================================================================================
来源：http://ozt.yongpay.top

L. 网络请求
来源：http://oqp.snrcjt.cn

================================================================================
来源：http://tnb.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://juf.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nct.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jdt.ydzc1.top

JS:   await fetch(url)
来源：http://wrv.nwbrower.top

TS:   await fetch(url)
来源：http://nqi.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pds.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://vbw.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qcd.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tei.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://hie.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wdf.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wif.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oog.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yno.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tus.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://agj.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://skv.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hmt.zdqjudy.top


<!-- 参考信息 -->