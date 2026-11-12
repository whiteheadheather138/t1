代发 wailian999

JS:   e.message;  e.stack
来源：http://yrb.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bpd.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kzu.bjfxy.top

Go:   err.Error()
来源：http://yec.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://xtl.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://ikl.ivvv.top

[H09] 带错误码的异常
来源：http://vqg.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://afc.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rgb.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://clq.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vcs.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hku.xingfuxueyuan.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dhb.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lhw.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zse.gogol.net.cn

[H10] 资源自动释放
来源：http://gke.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zrn.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pps.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cef.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rdk.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://voh.tianlin.xyz

Go:   defer f.Close()
来源：http://aeu.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://czn.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nuc.zhongyouzk.top

================================================================================
来源：http://fix.sysykeji.top

I. 正则表达式
来源：http://vnl.iojbl.cn

================================================================================
来源：http://yuo.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://yik.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uhz.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oiw.birdmap.top

JS:   /\d+/.test(s)
来源：http://cxx.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://kvz.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wdd.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vkc.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://lea.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hlp.yonumen.top

[I02] 提取所有匹配
来源：http://vub.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://jxf.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ypt.aibaodan.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yxq.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://gwj.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ojq.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sjt.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://pgt.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dec.hesvh.cn

[I03] 提取捕获分组
来源：http://uuw.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vud.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://npg.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uoy.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://onb.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ten.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://run.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eqf.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qgk.feifeiyinyue.top

[I04] 正则替换
来源：http://qnz.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://lth.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pdy.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ovk.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://zkh.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://ooo.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ouf.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bvt.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://icu.iojbl.cn

[I05] 按正则拆分
来源：http://bek.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://egj.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vdr.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://mip.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://udi.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://gqg.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mou.hcnkem.com

Ruby: s.split(/\s*,\s*/)
来源：http://mlg.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nrf.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gmb.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zwf.snrcjt.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lrg.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zuj.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://joc.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mbx.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rag.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aim.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eeg.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://yck.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://plh.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hsi.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eon.jinqigufen.top

TS:   /error/gim
来源：http://kkx.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dlm.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aco.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://koa.chenlongwang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rnn.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://rsc.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ghv.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dbq.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iaf.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://psj.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tlr.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ank.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gka.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://npz.xziqi.cn

================================================================================
来源：http://eiz.redwolf501.top

J. 日期与时间
来源：http://was.ydjk.org.cn

================================================================================
来源：http://jqz.yj20258.top

[J01] 获取当前时间
来源：http://ryg.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nyv.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wga.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://acy.smart0.xyz

TS:   new Date();  Date.now()
来源：http://jvr.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gzt.hnqzz.top

Go:   time.Now()
来源：http://irv.epnwcf.com

Ruby: Time.now
来源：http://wko.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zfp.jyoumei.cn

[J02] 格式化输出
来源：http://ecl.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tap.mhx1999.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fiz.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dxg.gotoacloud.top

TS:   d.toISOString()
来源：http://fll.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zrm.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://euo.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://odj.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bnc.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://znh.hfpthk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://doz.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nms.yj202588.top

JS:   new Date("2024-01-02")
来源：http://rud.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://omj.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://qwy.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://llj.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://jae.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xrv.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://noh.jinqigfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pbo.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ejb.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://opa.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qam.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gvm.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mts.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://trk.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hdz.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://pua.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://ekd.yuanzhike.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xps.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uld.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fbk.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://awq.guannengcc.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rnf.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://urz.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fio.tanke756.top

[J06] 计算两时间之差
来源：http://wqo.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://qst.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://xyf.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zah.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ntr.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://gtu.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://ybm.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://qwr.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://uwe.jlsjyb.cn

[J07] 比较两个日期
来源：http://amx.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://nju.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zsg.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://asr.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ghc.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ofr.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zsh.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://nqa.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://tgn.c1oappe.top

[J08] 提取年月日与星期
来源：http://pil.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://skl.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pcf.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ygq.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://poj.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hap.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zop.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hqa.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://upd.pengpengdd.cyou

[J09] 时区处理
来源：http://hxk.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wtu.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rda.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://var.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxq.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://snh.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://khb.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://cme.ehwqpu.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jfn.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://pdv.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://isf.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://txf.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://emq.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ymp.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iob.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zsq.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pnk.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sgf.sufxvd.cn

================================================================================
来源：http://mak.xinyue.icu

K. JSON 与序列化
来源：http://qai.uphjek.com

================================================================================
来源：http://odm.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://eli.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dyb.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://azb.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://vvs.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://xky.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zvq.yj202588.top

Go:   json.Marshal(obj)
来源：http://liy.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://ywo.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://vyd.aizwys.cn

[K02] JSON 字符串转对象
来源：http://uwg.cdnleiting.top

Py:   json.loads(s)
来源：http://gek.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rpm.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://pmf.fehbvm.com

TS:   JSON.parse(s)
来源：http://cuq.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://usy.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://nbw.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://yfx.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uiq.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://dbm.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://spx.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lep.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hcw.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wwy.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mxx.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uxk.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://ejh.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kqr.uphjek.com

[K04] 读取 JSON 文件
来源：http://wnl.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dzv.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pku.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tui.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aio.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wuw.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://juy.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lhb.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mvd.vehdjk.com

[K05] 深拷贝对象
来源：http://qib.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://lgh.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://fdx.yuanzhike.top

JS:   structuredClone(obj)
来源：http://ruc.yfazqb.com

TS:   structuredClone(obj)
来源：http://mhb.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fto.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eak.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nwa.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://xvn.havefunace.top

[K06] 解析 URL 查询串
来源：http://xcu.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://htv.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uds.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qtb.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yut.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://otm.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aco.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vbx.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hum.zhaomingkeji.xyz

[K07] 进制转换
来源：http://kra.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rzu.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jrm.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dey.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lfo.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://opf.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hfv.yvedp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ptu.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xmo.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://klj.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://oqe.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xth.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://fox.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://mcf.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eas.yongpay.top

Go:   encoding/gob
来源：http://ucw.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://xqb.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hjw.smart0.xyz

================================================================================
来源：http://zrm.jinghuilouyu.cn

L. 网络请求
来源：http://qrj.c1oappe.top

================================================================================
来源：http://ksu.hammf.cn

[L01] 发送 GET 请求
来源：http://myj.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hes.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wen.sysykeji.top

JS:   await fetch(url)
来源：http://dfh.jqgfzy.top

TS:   await fetch(url)
来源：http://edl.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xme.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://scl.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://irl.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dxb.zdqjudy.top

[L02] 发送 POST JSON
来源：http://omj.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://blb.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oeu.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rai.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gtn.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ele.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fep.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rsg.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kxt.smart0.xyz

[L03] 设置自定义请求头
来源：http://iui.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xwl.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mcq.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fht.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://opf.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qso.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hsq.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nbc.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bwq.cqqwz.cn

[L04] 设置超时
来源：http://qrk.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://smo.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ztc.vqdsnc.cn


<!-- 参考信息 -->