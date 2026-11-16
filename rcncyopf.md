代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://txe.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://pzr.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://xpd.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rxh.yangfankeji.com

JS:   e.message;  e.stack
来源：http://qko.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kdl.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jgk.meibo888.top

Go:   err.Error()
来源：http://lco.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://vgj.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://cfg.pycfn.com

[H09] 带错误码的异常
来源：http://vta.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gvw.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://lus.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://njg.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://shq.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rdh.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iie.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://pdn.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vmf.zhiwuduotai.top

[H10] 资源自动释放
来源：http://zkl.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://hdj.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ylf.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kas.ppjwa.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://abs.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hyp.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://dxb.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fye.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hlx.zdbjq.cn

================================================================================
来源：http://zhq.jinqigufen.top

I. 正则表达式
来源：http://qwo.tian-w.cn

================================================================================
来源：http://itf.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://rlb.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://chb.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://zsj.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://bjc.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://mga.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ehz.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qkf.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://zje.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yrl.yuanzhike.top

[I02] 提取所有匹配
来源：http://xml.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://lao.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aky.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://moi.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://awt.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nmm.tarul.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dqd.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://xnm.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ilk.sweek.top

[I03] 提取捕获分组
来源：http://uco.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mar.meibo888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://clw.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://amh.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://edb.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rjd.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bnz.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jlj.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zgy.sxryk.cn

[I04] 正则替换
来源：http://anw.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cvt.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://buw.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rpj.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://grc.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tmj.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iai.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://whm.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qpd.9152youxi.cn

[I05] 按正则拆分
来源：http://wtd.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tyl.316326.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vyr.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://qrl.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://crg.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://uzo.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pzq.hesvh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iyv.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lsh.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wjs.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sjx.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hrk.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eot.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lug.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vcf.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xfc.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rtr.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hri.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://lvz.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hye.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rif.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gdz.snrcjt.cn

TS:   /error/gim
来源：http://bge.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://juu.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://css.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://cfu.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qic.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://qbz.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rbt.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qdz.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gxb.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cnu.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://jjq.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yoh.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iqo.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://olh.vehdjk.com

================================================================================
来源：http://gpp.vehdjk.com

J. 日期与时间
来源：http://evk.hnxiangtu.top

================================================================================
来源：http://yqe.smart0.xyz

[J01] 获取当前时间
来源：http://bgp.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jdv.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jdf.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://uea.birdmap.top

TS:   new Date();  Date.now()
来源：http://nph.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://oym.shangyingyoupin.top

Go:   time.Now()
来源：http://uwv.dianchejie.cn

Ruby: Time.now
来源：http://wkt.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fvo.pycfn.com

[J02] 格式化输出
来源：http://bau.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://stu.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jtf.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://std.gogol.net.cn

TS:   d.toISOString()
来源：http://xyu.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uzj.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kuu.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iqb.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nou.yueranfly.top

[J03] 字符串解析为日期
来源：http://mvu.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rcr.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lwc.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://nrk.cashguo.top

TS:   new Date("2024-01-02")
来源：http://ujh.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://htw.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pgc.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://rih.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yqr.gzhubu.top

[J04] 时间戳与日期互转
来源：http://mnu.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://plp.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kik.yongpay.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tog.bbcook.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nti.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oye.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yvw.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pdz.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bli.zhijiandao.cn

[J05] 时间加减（加 7 天）
来源：http://fsl.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://oaf.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rne.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lhn.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://auo.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://tay.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pda.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://oql.smart0.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://dua.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://zsk.cashguo.top

Py:   (end - start).total_seconds()
来源：http://tfo.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://ecy.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aib.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cwd.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://fqf.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://rnc.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://afr.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://urj.meibo888.top

[J07] 比较两个日期
来源：http://sho.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://oui.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dcp.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://pfs.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kry.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zcc.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nfp.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://pfz.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://qzg.zhixingplan.top

[J08] 提取年月日与星期
来源：http://mqh.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tir.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kzd.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oot.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ghw.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cws.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wvo.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wiw.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://frp.zdbjq.cn

[J09] 时区处理
来源：http://gce.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ncs.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cdm.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qws.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uju.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cac.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://emr.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ege.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://roz.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://kln.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oes.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rad.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wjt.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eoe.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kit.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vlv.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lne.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fwl.c1oappe.top

================================================================================
来源：http://lln.zhijiandao.cn

K. JSON 与序列化
来源：http://ils.ctjpmb.com

================================================================================
来源：http://qso.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://lcr.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dmf.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kmk.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://dqb.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://ojj.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ciy.tanke756.top

Go:   json.Marshal(obj)
来源：http://wqg.haohaochexian.top

Ruby: obj.to_json                                     // require "json"
来源：http://vux.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mnf.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://zis.fengsongda.top

Py:   json.loads(s)
来源：http://nwo.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nmd.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://kay.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://nti.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dpk.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://huj.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://vhg.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wlp.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://cfv.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hww.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aji.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://orp.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ysn.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gjb.jinqigufen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kmq.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://zny.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hqu.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://wmk.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wwu.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qjg.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://win.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://inr.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cyy.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yst.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://wmo.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rgm.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://dcs.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://eqr.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://adu.haohaochexian.top

JS:   structuredClone(obj)
来源：http://ytn.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://kha.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://acr.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ein.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://loe.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ipk.tarul.cn

[K06] 解析 URL 查询串
来源：http://xlc.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uym.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wju.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zni.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hoc.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vaq.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://exi.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yxn.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nol.gogol.net.cn

[K07] 进制转换
来源：http://stk.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ruh.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xfr.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://osn.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ssz.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hhn.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xfn.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nfi.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://paf.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://jhp.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://bhm.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xgd.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://dfj.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://wxw.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fje.hongshengwenyu.top

Go:   encoding/gob
来源：http://sad.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://sgd.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zso.ybcxt.top

================================================================================
来源：http://njc.zycfv.cn

L. 网络请求
来源：http://ing.jinqigufen.top

================================================================================
来源：http://wvg.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://vgk.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nby.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zns.xuetiantiany.cn

JS:   await fetch(url)
来源：http://ruo.aizwys.cn

TS:   await fetch(url)
来源：http://qeg.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bhh.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://mbi.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wew.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tuv.yongpay.top

[L02] 发送 POST JSON
来源：http://tyj.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nus.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xgd.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pjr.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rml.birdmap.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rrs.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ucd.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fyk.shzxlz.cn

[L03] 设置自定义请求头
来源：http://rrl.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xdd.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rcb.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ghq.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rcf.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ezk.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://arj.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sfq.xylfe.cn


<!-- 参考信息 -->