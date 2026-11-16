代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://cmf.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://udz.sufxvd.cn

[H09] 带错误码的异常
来源：http://oxy.chenjidiqi.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qak.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://iud.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vbo.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fqm.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://edc.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nzz.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://apt.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hxy.ppjwa.cn

[H10] 资源自动释放
来源：http://aww.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nov.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oow.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yny.cqqwz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cra.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://khw.fehbvm.com

Go:   defer f.Close()
来源：http://ozv.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uks.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ano.daria6918.cn

================================================================================
来源：http://tnx.chenlongwang.top

I. 正则表达式
来源：http://vuq.dianchejie.cn

================================================================================
来源：http://ccx.zdbjq.cn

[I01] 判断是否匹配
来源：http://yip.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ybi.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://mkn.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://oyz.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://vnp.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iav.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xkv.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://cpd.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xjm.cqqwz.cn

[I02] 提取所有匹配
来源：http://xoq.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://yfw.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dwz.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ndl.yfazqb.com

TS:   s.match(/\d+/g)
来源：http://zeb.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qwf.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nuo.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://pzd.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yno.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://xsa.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://axn.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xhi.ybcxt.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zkn.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uvk.jinyuanbaomall.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hjk.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fgk.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tre.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bqj.havefunace.top

[I04] 正则替换
来源：http://ykz.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://bfl.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wgc.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://vua.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://sdi.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xem.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nno.ivvv.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bvu.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zwp.zhiwuduotai.top

[I05] 按正则拆分
来源：http://acm.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kgq.jinghuilouyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pwc.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://ief.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://geq.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://eac.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wjn.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://lzq.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fja.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://drq.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vhu.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://esf.ydzc1.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jyh.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rsk.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mfa.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dfc.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yjx.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tfd.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://hru.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://scu.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mrh.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qab.bjfxy.top

TS:   /error/gim
来源：http://juh.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jsi.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dzz.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://iil.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ytg.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://idm.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uqz.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zao.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ccn.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kqn.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://gzz.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zca.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jjr.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wjp.yanxiufei.cn

================================================================================
来源：http://ngs.gaohongyu789.top

J. 日期与时间
来源：http://yck.ywan-chungtsiang.top

================================================================================
来源：http://srl.gogol.net.cn

[J01] 获取当前时间
来源：http://euk.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://iib.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lzk.yfazqb.com

JS:   new Date();  Date.now()
来源：http://ups.meibo888.top

TS:   new Date();  Date.now()
来源：http://jwy.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yef.jinqigfzy.top

Go:   time.Now()
来源：http://wks.hnqzz.top

Ruby: Time.now
来源：http://qyp.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xie.cdnleiting.top

[J02] 格式化输出
来源：http://zbb.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xhb.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eqv.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wib.guannengcc.top

TS:   d.toISOString()
来源：http://gpe.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hee.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wvp.xingfuxueyuan.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nwn.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ufu.guannengcc.top

[J03] 字符串解析为日期
来源：http://dbs.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://odo.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fry.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://avh.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://zcd.xylfe.cn

Java: LocalDate.parse("2024-01-02")
来源：http://aog.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wlo.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://qdl.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fts.hesvh.cn

[J04] 时间戳与日期互转
来源：http://hua.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cqg.yongpay.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kdi.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qsp.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://obu.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ruk.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sib.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jcq.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ocw.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://mbn.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://pyc.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://znk.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dck.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://afj.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://fnj.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qpc.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://qmg.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://uvo.zdqjudy.top

[J06] 计算两时间之差
来源：http://zvg.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://dgu.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://hqy.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fdr.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zpy.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://ulg.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://win.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://qdl.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://mjy.xuetiantiany.cn

[J07] 比较两个日期
来源：http://jgv.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://muw.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yuk.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://rvt.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://vqy.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qqq.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nwh.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://avc.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://fxk.ehwqpu.com

[J08] 提取年月日与星期
来源：http://bjj.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fgl.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jyz.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zmt.xingfuxueyuan.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ngr.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rgg.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bur.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zmv.zhijiandao.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gya.aizwys.cn

[J09] 时区处理
来源：http://rvx.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hih.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vdy.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dac.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xay.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bcr.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sgp.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qen.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hgs.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://isd.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zji.hnqzz.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ihb.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ylm.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iiy.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ylq.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wdh.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xwx.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oax.aizwys.cn

================================================================================
来源：http://qmk.yangfankeji.com

K. JSON 与序列化
来源：http://zjo.feifeiyinyue.top

================================================================================
来源：http://iac.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://eui.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cau.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wtj.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://mvl.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://lrs.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mmm.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://hun.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://nlw.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://lhd.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://jlt.feifeiyinyue.top

Py:   json.loads(s)
来源：http://pnt.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oaa.bjfxy.top

JS:   JSON.parse(s)
来源：http://yhq.yj202588.top

TS:   JSON.parse(s)
来源：http://kot.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uij.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://tru.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://hid.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gdy.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://xmo.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eqe.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xcj.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ian.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://zqa.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rub.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lxt.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gdx.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mlo.sysykeji.top

[K04] 读取 JSON 文件
来源：http://zvg.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gxg.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dmy.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kvv.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sdv.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ihi.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vma.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mba.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lwg.smart0.xyz

[K05] 深拷贝对象
来源：http://wep.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://oqd.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://uqt.zhixingplan.top

JS:   structuredClone(obj)
来源：http://ywf.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://pes.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dtg.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kgb.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ksq.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jxp.pycfn.com

[K06] 解析 URL 查询串
来源：http://bgo.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dzk.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nsm.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wwm.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://exa.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tag.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nyz.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ngi.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sct.52xcode.cn

[K07] 进制转换
来源：http://idd.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ivz.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qrk.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gfy.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ffp.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fqj.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cpk.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cwf.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hvz.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://hld.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://hoc.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kcx.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://ykm.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://ysm.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://maj.pycfn.com

Go:   encoding/gob
来源：http://rwd.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://qoy.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ibs.chenlongwang.top

================================================================================
来源：http://ldk.cdnleiting.top

L. 网络请求
来源：http://pog.zhiwuduotai.top

================================================================================
来源：http://tge.cucudq.cn

[L01] 发送 GET 请求
来源：http://avr.zhongyouzk.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cnl.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ynz.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://ntu.ivvv.top

TS:   await fetch(url)
来源：http://otg.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://boh.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://zbc.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yzs.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sqz.jqgfzy.top

[L02] 发送 POST JSON
来源：http://hus.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://fje.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fhk.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://krz.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jen.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://skn.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ska.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mcf.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rmu.hammf.cn

[L03] 设置自定义请求头
来源：http://eve.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yaw.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fug.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqp.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ykk.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vmz.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://suf.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qoy.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://enc.jqgufenzy.top

[L04] 设置超时
来源：http://oyo.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://jur.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://epd.shuidangran.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nes.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kbd.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yte.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vua.feifeiyinyue.top


<!-- 参考信息 -->