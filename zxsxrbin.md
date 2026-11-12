代发 wailian999

JS:   e.message;  e.stack
来源：http://qaa.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yqn.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mgh.pycfn.com

Go:   err.Error()
来源：http://waw.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://uhn.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://ugp.nanxinkj.top

[H09] 带错误码的异常
来源：http://sta.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iho.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ubx.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bpe.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tad.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ucj.yj20258888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kvv.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jiq.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ctq.gotoacloud.top

[H10] 资源自动释放
来源：http://yxx.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://xfm.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ihl.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zdv.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jky.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://btx.zhijiandao.cn

Go:   defer f.Close()
来源：http://hkc.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ezv.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dhq.zhixingplan.top

================================================================================
来源：http://swi.shangyingyoupin.top

I. 正则表达式
来源：http://ivt.xuetiantiany.cn

================================================================================
来源：http://pxl.cqqwz.cn

[I01] 判断是否匹配
来源：http://nju.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jzs.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://vbd.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://qws.sweek.top

TS:   /\d+/.test(s)
来源：http://nmx.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jkn.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://buf.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://rix.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pge.jinqigufen.top

[I02] 提取所有匹配
来源：http://lfk.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://akk.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://moz.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nqw.sweek.top

TS:   s.match(/\d+/g)
来源：http://pvx.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mug.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wcg.aibaodan.cn

Ruby: s.scan(/\d+/)
来源：http://ydo.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yys.hcnkem.com

[I03] 提取捕获分组
来源：http://xbm.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eyn.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://orw.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://khw.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qnq.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iqc.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yhs.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mrd.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oxs.pycfn.com

[I04] 正则替换
来源：http://aun.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://kkt.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iby.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ahx.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lzb.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://qhf.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ajl.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oao.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kuz.52xcode.cn

[I05] 按正则拆分
来源：http://heh.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rdh.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fte.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://hsh.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://vol.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://xlu.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fkv.yuanzhike.top

Ruby: s.split(/\s*,\s*/)
来源：http://msh.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xfq.c1oappe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vkw.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdp.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lzk.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ges.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ytd.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ljd.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ktv.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iuw.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yvt.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://opi.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hlz.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pyo.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bdb.shangyingyoupin.top

TS:   /error/gim
来源：http://tpp.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://say.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cgh.havefunace.top

Ruby: s.scan(/error/i)
来源：http://xer.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zgh.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://vpl.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cus.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://llj.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lzz.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ttm.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nat.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://etc.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eio.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yow.xylfe.cn

================================================================================
来源：http://efa.dianchejie.cn

J. 日期与时间
来源：http://cqq.sufxvd.cn

================================================================================
来源：http://kaj.cqqwz.cn

[J01] 获取当前时间
来源：http://avy.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://fcl.tarul.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qdy.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://kes.xziqi.cn

TS:   new Date();  Date.now()
来源：http://htc.sysykeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lks.gotoacloud.top

Go:   time.Now()
来源：http://tom.shanyushiyangkeji.top

Ruby: Time.now
来源：http://rvn.yvedp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vzi.xylfe.cn

[J02] 格式化输出
来源：http://bdi.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://asp.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://boa.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aqo.0kj1m.cn

TS:   d.toISOString()
来源：http://vdd.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hur.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dql.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gft.zdbjq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nzz.uphjek.com

[J03] 字符串解析为日期
来源：http://ymy.zhijiandao.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://djm.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mqe.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://oyy.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://aip.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jzo.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iyd.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://vcq.jinqigufen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://smz.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://eai.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gtc.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ioi.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rft.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xfl.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://odd.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qct.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fmr.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yzf.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://yiz.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://uhr.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qyz.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ibu.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lnf.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://cne.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mbm.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://eps.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://hoi.ehwqpu.com

[J06] 计算两时间之差
来源：http://ras.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://abf.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://fgy.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nun.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bsz.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://flt.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://rai.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://pir.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://fxn.jianghu66.top

[J07] 比较两个日期
来源：http://vwo.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://mgs.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dmy.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://ypj.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ehs.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nnn.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://thm.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://gqg.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://fgf.cqqwz.cn

[J08] 提取年月日与星期
来源：http://twg.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qul.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nxz.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lnv.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kto.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mzm.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uta.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lyo.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jxd.mhx1999.top

[J09] 时区处理
来源：http://amp.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rfk.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wpp.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tqv.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wmy.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://frn.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xtm.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kts.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hen.0kj1m.cn

[J10] 取今天 / 本月第一天
来源：http://yjf.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ryk.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xnb.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fkl.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qmc.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cre.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xhj.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tcl.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eni.chenjidiqi.icu

================================================================================
来源：http://vxk.shuidangran.top

K. JSON 与序列化
来源：http://mip.xziqi.cn

================================================================================
来源：http://xjh.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://vps.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vjp.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gna.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://qca.birdmap.top

TS:   JSON.stringify(obj)
来源：http://dzj.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sle.yanxiufei.cn

Go:   json.Marshal(obj)
来源：http://nhy.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://kiv.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jbi.hcnkem.com

[K02] JSON 字符串转对象
来源：http://ebl.mhx1999.top

Py:   json.loads(s)
来源：http://oym.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bnl.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://iva.yj20258888.top

TS:   JSON.parse(s)
来源：http://udc.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://buq.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://yvg.c1oappe.top

Ruby: JSON.parse(s)
来源：http://ruz.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://log.shuidangran.top

[K03] JSON 美化输出（带缩进）
来源：http://mxr.hnxiangtu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wcy.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tiw.uphjek.com

JS:   JSON.stringify(obj, null, 2)
来源：http://gle.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://oki.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wnc.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ryi.shangyingyoupin.top

Ruby: JSON.pretty_generate(obj)
来源：http://vxx.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://reh.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://xhb.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dmj.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kse.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lje.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mwm.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fgo.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lxh.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mla.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yer.cashguo.top

[K05] 深拷贝对象
来源：http://jzs.tian-w.cn

Py:   copy.deepcopy(obj)
来源：http://kha.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://nxx.yuanzhike.top

JS:   structuredClone(obj)
来源：http://gib.nanxinkj.top

TS:   structuredClone(obj)
来源：http://mod.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ylz.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nwg.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vhu.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rpv.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://bdj.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eio.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wgu.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://icm.yj20258888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://snp.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rxb.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://seg.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zod.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kau.dianchejie.cn

[K07] 进制转换
来源：http://jdu.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tyb.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fxi.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qum.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pfe.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jog.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rbv.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qhf.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oui.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://uwq.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://psd.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jzq.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ivg.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://vac.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wgz.quarkkingdee.top

Go:   encoding/gob
来源：http://otz.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://jcm.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rfn.zycfv.cn

================================================================================
来源：http://cpv.chenzaomai.com

L. 网络请求
来源：http://exq.zhoulong.xyz

================================================================================
来源：http://gbw.dashuyun.cn

[L01] 发送 GET 请求
来源：http://ill.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jlj.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rvi.pycfn.com

JS:   await fetch(url)
来源：http://jmf.dianchejie.cn

TS:   await fetch(url)
来源：http://dok.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qzp.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://kyk.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oop.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://idw.yuanzhike.top

[L02] 发送 POST JSON
来源：http://pek.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ggg.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://owy.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ttd.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ffp.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fkw.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cij.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tfa.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tbu.xinyue.icu

[L03] 设置自定义请求头
来源：http://ufa.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pho.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://frh.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xwt.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vac.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://flp.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lwl.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qgh.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://txp.nanxuanxn.top

[L04] 设置超时
来源：http://kst.meibo888.top

Py:   requests.get(url, timeout=5)
来源：http://zgo.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xjc.guannengcc.top


<!-- 参考信息 -->