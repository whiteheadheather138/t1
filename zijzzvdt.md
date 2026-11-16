代发 wailian999

TS:   console.assert(x > 0);
来源：http://vqn.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://psf.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sug.ydzc1.top

Ruby: raise "必须为正" unless x > 0
来源：http://qev.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://ysp.feifeiyinyue.top

[H08] 获取错误信息与堆栈
来源：http://kwf.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://btv.meibo888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xnu.xuanzx.com

JS:   e.message;  e.stack
来源：http://uam.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kpq.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://bjd.tarul.cn

Go:   err.Error()
来源：http://fjr.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://iiw.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://zyd.zdqjudy.top

[H09] 带错误码的异常
来源：http://suf.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gws.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zba.zhongyouzk.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jsc.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://umx.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wbr.meibo888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zab.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://qrh.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://krk.ctjpmb.com

[H10] 资源自动释放
来源：http://cnc.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vub.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dlg.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lvr.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wcd.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wep.jiagoushi.top

Go:   defer f.Close()
来源：http://zlg.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lyu.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://drt.nwbrower.top

================================================================================
来源：http://mjf.zycfv.cn

I. 正则表达式
来源：http://ikw.yfazqb.com

================================================================================
来源：http://byg.shuidangran.top

[I01] 判断是否匹配
来源：http://bfd.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vpc.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://gto.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://zas.yueranfly.top

TS:   /\d+/.test(s)
来源：http://kcq.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qbc.xylfe.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ucs.yuxming.cn

Ruby: s.match?(/\d+/)
来源：http://rih.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sej.jianghu66.top

[I02] 提取所有匹配
来源：http://sxi.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://con.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://unq.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ulz.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://ahn.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tnp.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://owr.yangfankeji.com

Ruby: s.scan(/\d+/)
来源：http://vyk.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iia.xuetiantiany.cn

[I03] 提取捕获分组
来源：http://blw.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bwf.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dec.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zoq.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://idk.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qfx.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bmx.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wbr.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pxd.xuetiantiany.cn

[I04] 正则替换
来源：http://vpa.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fck.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hxr.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://phx.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://ttd.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://efh.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ccg.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uht.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jlu.ybcxt.top

[I05] 按正则拆分
来源：http://mtd.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bsd.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jhl.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://iax.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://qdb.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://doa.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wbd.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://qde.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://chz.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ccz.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nbo.zhiwuduotai.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ixn.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pnd.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jyw.fengsongda.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tcw.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ovh.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ilo.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ssl.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://dhz.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gyh.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ddg.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ysh.shuidangran.top

TS:   /error/gim
来源：http://xoy.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pmb.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nic.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://jaq.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://abl.cheryme.top

[I08] 贪婪与非贪婪匹配
来源：http://fay.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fyr.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://obf.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ezb.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xeg.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fvi.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rkg.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dhw.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uso.cucudq.cn

================================================================================
来源：http://pwj.fzhhl.top

J. 日期与时间
来源：http://ugn.jyoumei.cn

================================================================================
来源：http://rwk.fehbvm.com

[J01] 获取当前时间
来源：http://cau.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jty.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hdp.wangshuangyany.cn

JS:   new Date();  Date.now()
来源：http://ndx.iojbl.cn

TS:   new Date();  Date.now()
来源：http://yew.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qfx.chenjidiqi.icu

Go:   time.Now()
来源：http://goj.guannengcc.top

Ruby: Time.now
来源：http://tmt.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jhw.wangshuangyany.cn

[J02] 格式化输出
来源：http://itp.feifeiyinyue.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jjh.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mfb.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://chn.xziqi.cn

TS:   d.toISOString()
来源：http://yyy.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://evp.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vjy.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rco.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vta.dianchejie.cn

[J03] 字符串解析为日期
来源：http://qza.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bgg.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mqe.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://dkq.uphjek.com

TS:   new Date("2024-01-02")
来源：http://rua.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qpz.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://frm.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://nxs.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mvj.epnwcf.com

[J04] 时间戳与日期互转
来源：http://xcj.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://equ.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pkq.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wes.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tbr.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uqt.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uvy.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gsg.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://snl.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://src.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://gyw.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://acv.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pta.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rvd.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://bem.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gzw.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://wwj.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://cqv.ctjpmb.com

[J06] 计算两时间之差
来源：http://haa.ivvv.top

Py:   (end - start).total_seconds()
来源：http://ftv.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://zjd.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://noa.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://orz.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gbz.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://fkr.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://iff.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://rrn.hnqzz.top

[J07] 比较两个日期
来源：http://bcb.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://vkx.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zoa.52xcode.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mat.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://dna.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hwp.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wis.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://tnw.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://gia.svipenyu.cn

[J08] 提取年月日与星期
来源：http://aml.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lvr.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ngw.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ade.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://txy.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cke.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://syn.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wgv.bbcook.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rpd.jinghuilouyu.cn

[J09] 时区处理
来源：http://xto.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qcs.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zam.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://utd.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ksi.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mxw.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://esk.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xfi.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cgh.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://dxa.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nmd.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bta.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ort.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gby.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ous.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jva.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nqc.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vgf.tianlin.xyz

================================================================================
来源：http://jyg.sysykeji.top

K. JSON 与序列化
来源：http://pix.zhaomingkeji.xyz

================================================================================
来源：http://inl.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://nsm.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cwc.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zjt.316326.xyz

JS:   JSON.stringify(obj)
来源：http://rif.cashguo.top

TS:   JSON.stringify(obj)
来源：http://eou.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://paq.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://tqb.zycfv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eun.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jfe.cashguo.top

[K02] JSON 字符串转对象
来源：http://one.shzxlz.cn

Py:   json.loads(s)
来源：http://ahj.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wlw.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://amf.jyoumei.cn

TS:   JSON.parse(s)
来源：http://mjg.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://raj.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://unu.bjfxy.top

Ruby: JSON.parse(s)
来源：http://axg.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ivz.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://icu.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bvu.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qso.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jxx.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iix.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xfc.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eiu.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://mtm.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://owg.yj20258.top

[K04] 读取 JSON 文件
来源：http://kzc.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cgy.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://khe.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dwo.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ies.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://njt.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yol.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ejm.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jhk.andypj.xyz

[K05] 深拷贝对象
来源：http://bin.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://thb.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://mmw.vehdjk.com

JS:   structuredClone(obj)
来源：http://ksu.cdnleiting.top

TS:   structuredClone(obj)
来源：http://zwr.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://rlm.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jtq.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gdo.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://log.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://vff.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://btk.smart0.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pid.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xbd.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vuc.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://afo.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fet.shanyushiyangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jvz.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qzb.tianlin.xyz

[K07] 进制转换
来源：http://lqh.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mfg.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ben.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wio.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gfj.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://osd.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ehe.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tja.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eio.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://xhu.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://iug.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://txf.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://yig.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://rds.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kkg.yuanzhike.top

Go:   encoding/gob
来源：http://rpj.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://gff.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://npa.smart0.xyz

================================================================================
来源：http://uiz.zdbjq.cn

L. 网络请求
来源：http://cax.jinghuilouyu.cn

================================================================================
来源：http://cux.vehdjk.com

[L01] 发送 GET 请求
来源：http://awm.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zwp.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://poh.pengpengdd.cyou

JS:   await fetch(url)
来源：http://oou.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://mab.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://che.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://doo.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xsl.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xny.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://ssi.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://hlo.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kgv.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pnj.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bbz.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zqz.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ccb.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bim.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nao.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://gfo.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uda.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oym.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vfn.ydjk.org.cn


<!-- 参考信息 -->