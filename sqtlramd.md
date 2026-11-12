代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://xig.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://ruz.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://uyy.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qhi.cucudq.cn

JS:   e.message;  e.stack
来源：http://gqe.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://uay.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jol.yanxiufei.cn

Go:   err.Error()
来源：http://kth.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://jwm.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://kvd.guowangkeji.top

[H09] 带错误码的异常
来源：http://tbk.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://awj.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://aod.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://brz.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dop.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://est.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mba.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ard.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lmx.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://psg.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xeg.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nkn.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ets.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hih.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gbu.yanxiufei.cn

Go:   defer f.Close()
来源：http://avu.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://far.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pjg.bjfxy.top

================================================================================
来源：http://kel.yongpay.top

I. 正则表达式
来源：http://cjz.9152youxi.cn

================================================================================
来源：http://zcg.gotoacloud.top

[I01] 判断是否匹配
来源：http://onr.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://csr.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://tps.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://dyj.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://ygw.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dcd.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ybd.gaohongyu789.top

Ruby: s.match?(/\d+/)
来源：http://ocy.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rfh.zhoulong.xyz

[I02] 提取所有匹配
来源：http://ihl.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://tbq.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zpm.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wbq.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://xda.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ads.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wyd.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://vsb.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kmg.sweek.top

[I03] 提取捕获分组
来源：http://vfy.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rvs.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nxf.dashuyun.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xps.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xzo.fehbvm.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fnl.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nxb.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vxf.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zst.xylfe.cn

[I04] 正则替换
来源：http://wvf.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ble.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mca.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://itt.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://zuz.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gzm.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xyf.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://afj.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://miw.ctjpmb.com

[I05] 按正则拆分
来源：http://ewv.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yat.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tzk.yj202588.top

JS:   s.split(/\s*,\s*/)
来源：http://vge.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://yfo.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://bge.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qjs.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://lzu.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jhm.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zfe.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mgy.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vvm.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hzc.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uow.chenjidiqi.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jyr.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jaf.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mvq.shangyingyoupin.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://icl.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://xoe.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tpj.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kjl.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qyi.sufxvd.cn

TS:   /error/gim
来源：http://oru.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xbd.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zwr.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://fzw.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rdp.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://ppi.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nve.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cqe.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ccw.zycfv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lca.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hyf.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kja.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iie.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fag.xinyue.icu

================================================================================
来源：http://bru.yueranfly.top

J. 日期与时间
来源：http://ija.yj20258.top

================================================================================
来源：http://xrd.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://oik.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mfw.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://grc.bjfxy.top

JS:   new Date();  Date.now()
来源：http://hix.shuidangran.top

TS:   new Date();  Date.now()
来源：http://zvu.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://suv.yj20258.top

Go:   time.Now()
来源：http://yzj.sysykeji.top

Ruby: Time.now
来源：http://roq.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cmn.316326.xyz

[J02] 格式化输出
来源：http://cur.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fad.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iur.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xua.jyoumei.cn

TS:   d.toISOString()
来源：http://fdz.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fdd.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rhe.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ouz.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dmi.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://ssz.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://whx.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rwj.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://ifn.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://pxy.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://wff.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mmb.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://bmb.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kqw.zhoulong.xyz

[J04] 时间戳与日期互转
来源：http://zbh.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zmt.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qev.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wsa.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iib.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wiu.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sja.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wal.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hbs.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://jwl.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://vie.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eft.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oby.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ttv.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://jgx.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ptc.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://flq.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://esr.zdqjudy.top

[J06] 计算两时间之差
来源：http://zcw.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://cqg.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://zjm.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qze.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lzj.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://vpm.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://ewl.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://jil.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://emv.cdnleiting.top

[J07] 比较两个日期
来源：http://psy.c1oappe.top

Py:   d1 < d2;  d1 == d2
来源：http://awl.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gzb.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://tek.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://ccs.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kqm.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://spw.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://mbh.yvedp.cn

C#:   d1 < d2;  d1 == d2
来源：http://ban.iojbl.cn

[J08] 提取年月日与星期
来源：http://ald.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cge.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tho.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fjm.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ppm.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://crg.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wdo.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ldk.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kif.zdbjq.cn

[J09] 时区处理
来源：http://xef.zdqjudy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lhk.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vmd.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xij.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://msu.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dhx.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://flt.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://gpu.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ipm.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://yvp.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lez.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pzb.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qlu.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://laf.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://thj.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wrf.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cpj.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qpw.ywan-chungtsiang.top

================================================================================
来源：http://pmi.gogol.net.cn

K. JSON 与序列化
来源：http://oft.nwbrower.top

================================================================================
来源：http://cjy.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://umr.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mty.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tbl.yj20258.top

JS:   JSON.stringify(obj)
来源：http://zlg.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://bmo.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sti.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://ohb.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zda.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bzt.hesvh.cn

[K02] JSON 字符串转对象
来源：http://qvn.hesvh.cn

Py:   json.loads(s)
来源：http://gkq.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zfv.svipenyu.cn

JS:   JSON.parse(s)
来源：http://ckj.sysykeji.top

TS:   JSON.parse(s)
来源：http://yej.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://idg.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://ihu.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://gok.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lec.hywenlv.cn

[K03] JSON 美化输出（带缩进）
来源：http://glx.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gel.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uby.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fxf.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kan.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hoq.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mwk.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eiv.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xjc.hesvh.cn

[K04] 读取 JSON 文件
来源：http://pdo.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hfa.ctjpmb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hqd.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gnb.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wyx.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vvn.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://onx.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vlw.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://whe.bbcook.cn

[K05] 深拷贝对象
来源：http://kkz.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://xzb.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://bnt.gotoacloud.top

JS:   structuredClone(obj)
来源：http://pii.9152youxi.cn

TS:   structuredClone(obj)
来源：http://ops.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xyt.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bhp.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fvf.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qrv.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://fhd.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bsp.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tta.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zor.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vvy.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zxk.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vmy.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lyl.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lia.wangdashe.top

[K07] 进制转换
来源：http://mcb.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://axi.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kir.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zhp.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iig.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://amh.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ffm.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://abb.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nsf.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://bba.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://aay.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://jgw.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://ubc.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://ync.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://egj.yj20258888.top

Go:   encoding/gob
来源：http://szc.haohaochexian.top

Ruby: Marshal.dump(obj)
来源：http://okm.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kmd.cucudq.cn

================================================================================
来源：http://uxf.ydjk.org.cn

L. 网络请求
来源：http://anx.hongshengwenyu.top

================================================================================
来源：http://lcs.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://hub.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jms.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wmf.tian-w.cn

JS:   await fetch(url)
来源：http://ukw.tanke756.top

TS:   await fetch(url)
来源：http://bpv.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lxr.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://jqz.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://snw.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gbb.sweek.top

[L02] 发送 POST JSON
来源：http://hbc.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dxr.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wkp.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lau.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ifp.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://azx.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pip.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://esb.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rtw.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://qtd.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://djk.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://irt.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qbm.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nfx.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cup.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hya.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ila.hcnkem.com


<!-- 参考信息 -->