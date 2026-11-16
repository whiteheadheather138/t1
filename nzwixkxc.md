代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://uqe.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://xxz.snrcjt.cn

[H09] 带错误码的异常
来源：http://mue.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uln.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://igb.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yuv.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jys.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hmv.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uax.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qjf.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rrz.yanxiufei.cn

[H10] 资源自动释放
来源：http://lxa.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://fom.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rka.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dbv.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ref.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gtj.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://vny.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mvp.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pez.andypj.xyz

================================================================================
来源：http://bbq.ywan-chungtsiang.top

I. 正则表达式
来源：http://uqj.jyoumei.cn

================================================================================
来源：http://vrj.guannengcc.top

[I01] 判断是否匹配
来源：http://qcs.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://flq.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://qsa.hnqzz.top

JS:   /\d+/.test(s)
来源：http://qat.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://bxb.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://skt.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kyi.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://ecv.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vfx.guannengcc.top

[I02] 提取所有匹配
来源：http://psb.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://yoe.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cod.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ldl.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://dml.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ifu.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dqy.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://awr.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rpo.xziqi.cn

[I03] 提取捕获分组
来源：http://kkw.nanxuanxn.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uca.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pwz.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://siy.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rra.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://evg.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ysw.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wed.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fky.bjfxy.top

[I04] 正则替换
来源：http://rea.hysaishi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gch.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tsy.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ijs.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://xct.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://iiq.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://trh.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rdn.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ovm.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://mjd.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ipd.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://prm.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://dkn.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ofh.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://mti.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wfh.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://bkr.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qbv.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xdf.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lse.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xgi.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rkb.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://duo.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dkp.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://brv.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hfz.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kgr.quarkkingdee.top

[I07] 忽略大小写与多行模式
来源：http://ewl.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ujf.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pch.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tom.gaohongyu789.top

TS:   /error/gim
来源：http://shr.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xyj.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://amn.uphjek.com

Ruby: s.scan(/error/i)
来源：http://mbu.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ver.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://wlo.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hdv.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vfo.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yyh.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yow.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qov.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dcl.hammf.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yot.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dph.daxiang520.top

================================================================================
来源：http://mbm.shanyushiyangtech.top

J. 日期与时间
来源：http://sdb.shanyushiyangkeji.top

================================================================================
来源：http://ybm.hammf.cn

[J01] 获取当前时间
来源：http://ztv.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jis.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gkv.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://tbt.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://mbm.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mca.xylfe.cn

Go:   time.Now()
来源：http://ezs.gzhubu.top

Ruby: Time.now
来源：http://uub.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://omh.aibaodan.cn

[J02] 格式化输出
来源：http://nts.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vfs.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nez.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pgi.jqgfzy.top

TS:   d.toISOString()
来源：http://quv.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jfg.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ctm.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://val.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ydc.ybcxt.top

[J03] 字符串解析为日期
来源：http://fmc.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ifb.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://igk.316326.xyz

JS:   new Date("2024-01-02")
来源：http://rtf.sweek.top

TS:   new Date("2024-01-02")
来源：http://mwy.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://raw.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://scu.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://tnu.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aeh.andypj.xyz

[J04] 时间戳与日期互转
来源：http://rct.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://unl.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tqk.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kkk.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tvo.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tzq.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://njw.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ulb.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://igy.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://gaf.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://kkb.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://zwd.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vra.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vsg.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://hzw.yonumen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxn.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://gmu.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ozp.hywenlv.cn

[J06] 计算两时间之差
来源：http://lxi.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://nqt.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://scd.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jtg.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dig.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://rhq.sweek.top

Go:   end.Sub(start).Hours()
来源：http://qnr.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://aqt.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://zdu.svipenyu.cn

[J07] 比较两个日期
来源：http://swh.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://kxz.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rzy.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://yzw.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://yrb.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ras.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://shb.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gmc.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://piu.0kj1m.cn

[J08] 提取年月日与星期
来源：http://vgq.jinqigufen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xhd.hysaishi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ybh.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tir.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sca.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eri.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://quw.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://szv.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mli.yuxming.cn

[J09] 时区处理
来源：http://lmg.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nor.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://utx.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tik.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rfk.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://com.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kmu.wangshuangyany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fer.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qxp.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://wbw.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://djw.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vnb.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lbz.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gny.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qwx.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xxs.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kpk.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rcy.iojbl.cn

================================================================================
来源：http://hiz.9152youxi.cn

K. JSON 与序列化
来源：http://yqt.cdnleiting.top

================================================================================
来源：http://wse.zhijiandao.cn

[K01] 对象转 JSON 字符串
来源：http://fkf.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yup.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://opz.havefunace.top

JS:   JSON.stringify(obj)
来源：http://wck.yonumen.top

TS:   JSON.stringify(obj)
来源：http://ylh.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yib.cheryme.top

Go:   json.Marshal(obj)
来源：http://gdq.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qak.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vzv.mhx1999.top

[K02] JSON 字符串转对象
来源：http://lpv.aibaodan.cn

Py:   json.loads(s)
来源：http://rcs.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fev.jinqigfzy.top

JS:   JSON.parse(s)
来源：http://dlx.yonumen.top

TS:   JSON.parse(s)
来源：http://kys.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ugi.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://aex.shuidangran.top

Ruby: JSON.parse(s)
来源：http://krp.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://obz.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://xqo.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kaf.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sbe.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rwq.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://teh.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vqe.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://olj.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://jer.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eop.52xcode.cn

[K04] 读取 JSON 文件
来源：http://tsr.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gzz.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pgr.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ysd.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ifd.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kwt.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nrd.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qfq.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jod.sweek.top

[K05] 深拷贝对象
来源：http://kir.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://xyh.nanxuanxn.top

PHP:  unserialize(serialize($obj));
来源：http://ard.yuxming.cn

JS:   structuredClone(obj)
来源：http://znd.aibaodan.cn

TS:   structuredClone(obj)
来源：http://ryi.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dfw.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ztf.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://otx.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://boh.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://aio.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nyb.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tmo.jqgufenzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://frr.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mdf.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pwv.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ofj.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://scq.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yga.hnxiangtu.top

[K07] 进制转换
来源：http://mvy.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uwg.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bas.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lsk.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pjv.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://csm.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ked.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zyy.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qgw.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://smz.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://kim.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yyf.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://oct.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://enh.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qfi.kuanghao11.cn

Go:   encoding/gob
来源：http://ikh.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://kba.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lmd.haohaochexian.top

================================================================================
来源：http://uag.fktsv.cn

L. 网络请求
来源：http://soh.ybcxt.top

================================================================================
来源：http://ujn.ehwqpu.com

[L01] 发送 GET 请求
来源：http://vmk.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://llm.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ekp.guannengcc.top

JS:   await fetch(url)
来源：http://uyd.cdnleiting.top

TS:   await fetch(url)
来源：http://fhi.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cte.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://hfo.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dgp.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uhu.jqgfzy.top

[L02] 发送 POST JSON
来源：http://sjf.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://xlm.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iwa.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gap.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tav.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uqq.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lgt.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wqh.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dwu.nwbrower.top

[L03] 设置自定义请求头
来源：http://ofd.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vzp.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mnw.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kbx.andypj.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lws.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mdw.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tnm.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pdf.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yne.epnwcf.com

[L04] 设置超时
来源：http://mtz.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://xky.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oji.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dwo.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yij.xuetiantiany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ffv.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dkw.ppjwa.cn


<!-- 参考信息 -->