代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://rkx.sysykeji.top

C#:   e.Message;  e.StackTrace
来源：http://psg.hysaishi.cn

[H09] 带错误码的异常
来源：http://neq.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qoa.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vbi.yonumen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lqh.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mvd.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gyh.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ozp.tian-w.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rwp.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://xqt.hnxiangtu.top

[H10] 资源自动释放
来源：http://gez.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dze.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://itg.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kvi.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bwd.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://int.chenzaomai.com

Go:   defer f.Close()
来源：http://qot.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ant.iojbl.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://glf.nanxinkj.top

================================================================================
来源：http://bnl.tarul.cn

I. 正则表达式
来源：http://bnr.zhaomingkeji.xyz

================================================================================
来源：http://hvp.tanke756.top

[I01] 判断是否匹配
来源：http://jqy.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jne.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://xzw.redwolf501.top

JS:   /\d+/.test(s)
来源：http://nsz.yvedp.cn

TS:   /\d+/.test(s)
来源：http://jms.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dhr.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nra.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://tjo.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pfn.chenzaomai.com

[I02] 提取所有匹配
来源：http://rzw.smart0.xyz

Py:   re.findall(r"\d+", s)
来源：http://rvc.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://olq.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mla.316326.xyz

TS:   s.match(/\d+/g)
来源：http://lfq.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xwg.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://see.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://uff.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hgx.hfpthk.cn

[I03] 提取捕获分组
来源：http://qcx.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ozw.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kdy.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eos.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://amt.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mjl.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nwr.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://osl.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ehr.epnwcf.com

[I04] 正则替换
来源：http://gub.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vit.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ulj.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bjy.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ziu.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://fsw.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vqe.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xqt.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://czl.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://sdg.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ptw.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ffw.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ngs.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://pdp.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://arq.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ovl.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://scb.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rrm.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vvx.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qgc.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://myc.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oxc.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ase.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jeb.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://djy.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zlt.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fnj.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://wim.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://irf.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eoq.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://erv.snrcjt.cn

TS:   /error/gim
来源：http://kwo.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://prx.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xjv.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://atp.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dit.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://sqi.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tsu.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yxy.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iqq.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ptl.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://wga.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kxf.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rqy.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rrz.guowangkeji.top

================================================================================
来源：http://kcq.chenjidiqi.icu

J. 日期与时间
来源：http://rdc.xziqi.cn

================================================================================
来源：http://ewb.xylfe.cn

[J01] 获取当前时间
来源：http://tkg.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ztx.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bfj.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://vzr.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://wnm.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ryt.chenzaomai.com

Go:   time.Now()
来源：http://eov.zhaomingkeji.xyz

Ruby: Time.now
来源：http://afc.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ehh.9152youxi.cn

[J02] 格式化输出
来源：http://sxy.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bmt.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zeb.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qqo.fengsongda.top

TS:   d.toISOString()
来源：http://smj.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://khb.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tvh.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kkf.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yuv.jiagoushi.top

[J03] 字符串解析为日期
来源：http://csn.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gkz.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cza.pycfn.com

JS:   new Date("2024-01-02")
来源：http://ymx.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://uin.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xep.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fzx.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://hvw.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ecy.yfazqb.com

[J04] 时间戳与日期互转
来源：http://mem.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qvd.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mrv.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://asb.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ewk.xuetiantiany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kyl.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://enh.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ujc.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ziy.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://nhs.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://syz.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wli.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tfm.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ppl.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://han.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://loe.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://vaa.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://scx.nwbrower.top

[J06] 计算两时间之差
来源：http://deh.yj20258.top

Py:   (end - start).total_seconds()
来源：http://tbf.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://pjf.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xsb.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cfs.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://qgj.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://mry.shanyushiyangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://jrl.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://kja.bbcook.cn

[J07] 比较两个日期
来源：http://yjl.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://kxe.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mxd.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://uti.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://jdg.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xzr.316326.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mzc.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://bya.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://odg.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://wfo.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hca.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gev.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xze.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gzp.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wfh.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jcp.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ywo.shzxlz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yoa.cqqwz.cn

[J09] 时区处理
来源：http://qdt.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cae.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bdb.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hpk.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bqk.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://njf.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cxl.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://joz.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ody.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://yqx.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fet.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uzo.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ttc.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nyb.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ibt.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nef.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hmp.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://war.jlsjyb.cn

================================================================================
来源：http://new.bjfxy.top

K. JSON 与序列化
来源：http://qtn.ivvv.top

================================================================================
来源：http://ymi.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://wap.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ckp.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rek.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://xac.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://fzg.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://obc.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://hyw.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://fxx.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pfc.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://dyc.aizwys.cn

Py:   json.loads(s)
来源：http://mkk.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rmh.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://ord.yj202588.top

TS:   JSON.parse(s)
来源：http://ixv.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oen.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://bss.jianghu66.top

Ruby: JSON.parse(s)
来源：http://qne.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wol.cucudq.cn

[K03] JSON 美化输出（带缩进）
来源：http://uze.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ynk.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dyg.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://okf.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yyg.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pia.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eyl.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://xov.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://erj.jianghu66.top

[K04] 读取 JSON 文件
来源：http://bbf.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ouo.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xcv.gaohongyu789.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mmo.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gat.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rjr.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ghp.9152youxi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lbq.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tjz.sjlbkw.cn

[K05] 深拷贝对象
来源：http://ekk.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://tuo.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://qnj.yj20258.top

JS:   structuredClone(obj)
来源：http://rnq.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://pop.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bxn.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lln.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://orr.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://xpf.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://yzi.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mwv.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kqy.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fzj.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mua.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qyr.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://iaz.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://utf.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nnp.smart0.xyz

[K07] 进制转换
来源：http://qxi.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vuq.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://agm.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tof.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fnt.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xtg.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jcf.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zmu.hfpthk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://btm.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://mtb.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://uge.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://aor.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://zde.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://aaa.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ear.nanxuanxn.top

Go:   encoding/gob
来源：http://xqp.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://yrl.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iyl.yj20258.top

================================================================================
来源：http://vwo.yj202588.top

L. 网络请求
来源：http://ngd.316326.xyz

================================================================================
来源：http://wfe.nwbrower.top

[L01] 发送 GET 请求
来源：http://zri.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://buj.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vub.yongpay.top

JS:   await fetch(url)
来源：http://rzv.sysykeji.top

TS:   await fetch(url)
来源：http://jro.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tfy.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://xlh.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ryw.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rrq.vehdjk.com

[L02] 发送 POST JSON
来源：http://hgv.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://rdk.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ubl.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ciu.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kjy.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ury.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hcz.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pkv.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://czg.ybcxt.top

[L03] 设置自定义请求头
来源：http://ddq.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://foz.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xey.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mmw.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kre.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ihy.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rwh.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yth.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fam.dianchejie.cn

[L04] 设置超时
来源：http://tdu.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://hmg.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rtc.nanxuanxn.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ger.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zob.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://izx.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vvi.zhongyouzk.top


<!-- 参考信息 -->