代发 wailian999

TS:   console.assert(x > 0);
来源：http://thi.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://bti.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fna.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rky.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://kkf.zhoulong.xyz

[H08] 获取错误信息与堆栈
来源：http://gdx.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://zdm.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hns.sysykeji.top

JS:   e.message;  e.stack
来源：http://mts.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sfl.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://xfx.jinyuanbaomall.cn

Go:   err.Error()
来源：http://uaf.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://huk.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://znu.mhx1999.top

[H09] 带错误码的异常
来源：http://fgl.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sqh.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jru.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lpt.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pbx.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bvk.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bgq.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://amb.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vlo.yuxming.cn

[H10] 资源自动释放
来源：http://usl.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zon.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://phi.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://imy.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bpw.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pul.quarkkingdee.top

Go:   defer f.Close()
来源：http://pfp.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ibl.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oec.jyoumei.cn

================================================================================
来源：http://wav.ydzc1.top

I. 正则表达式
来源：http://ecp.jqgufenzy.top

================================================================================
来源：http://jpi.yuanzhike.top

[I01] 判断是否匹配
来源：http://vyh.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dcd.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://bho.epnwcf.com

JS:   /\d+/.test(s)
来源：http://wqx.fktsv.cn

TS:   /\d+/.test(s)
来源：http://bks.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gvd.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uva.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://ubo.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fao.redwolf501.top

[I02] 提取所有匹配
来源：http://ure.smart0.xyz

Py:   re.findall(r"\d+", s)
来源：http://xmg.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mri.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://htq.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://mwz.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vzo.sweek.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zca.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://eqo.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zld.sysykeji.top

[I03] 提取捕获分组
来源：http://iqu.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hws.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xxw.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ign.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ajp.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lzk.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jfi.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zea.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://krf.meibo888.top

[I04] 正则替换
来源：http://fxi.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://rmn.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sqb.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wcl.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://xto.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://hgi.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mfy.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zpn.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lhk.wangshuangyany.cn

[I05] 按正则拆分
来源：http://idc.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vos.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://esq.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://vyv.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://sfk.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://xiv.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fvi.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://idy.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wdt.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bjc.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sfg.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dbz.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vkb.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kpr.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tkf.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jxe.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ato.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iax.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://nie.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dga.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yhk.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ray.zhoulong.xyz

TS:   /error/gim
来源：http://dip.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pvp.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lep.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://qas.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lab.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://xmw.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lal.svipenyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://swu.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vap.cqqwz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cre.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jhh.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ulk.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mnd.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hzf.sufxvd.cn

================================================================================
来源：http://bkn.yfazqb.com

J. 日期与时间
来源：http://gwf.hysaishi.cn

================================================================================
来源：http://zsn.hongshengwenyu.top

[J01] 获取当前时间
来源：http://hot.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kuy.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gpd.shuidangran.top

JS:   new Date();  Date.now()
来源：http://rdv.tarul.cn

TS:   new Date();  Date.now()
来源：http://utp.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rfh.yfazqb.com

Go:   time.Now()
来源：http://odf.zhijiandao.cn

Ruby: Time.now
来源：http://plg.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tgb.gaohongyu789.top

[J02] 格式化输出
来源：http://ygd.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avb.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://odx.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cvq.fktsv.cn

TS:   d.toISOString()
来源：http://err.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qte.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://szu.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yeh.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tkf.guowangkeji.top

[J03] 字符串解析为日期
来源：http://czt.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xby.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ftx.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://dhb.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://tpu.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://rad.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uze.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://hkl.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aah.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://nuc.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ymr.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cko.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wmc.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://whg.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ame.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gwg.sufxvd.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lle.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vir.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://nvq.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://qna.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yqo.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xab.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nad.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://gba.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ppy.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://qkb.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rwj.smart0.xyz

[J06] 计算两时间之差
来源：http://umv.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://mac.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://cdn.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rbp.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zlo.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xrj.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://eqg.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://yez.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://gbb.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://mvl.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://pnq.jianghu66.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://buc.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kmh.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kde.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cqw.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uxv.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vik.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://dbb.bjfxy.top

[J08] 提取年月日与星期
来源：http://adn.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mbj.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bao.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qud.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tsf.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tvi.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qaq.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zwy.zhongyouzk.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zdu.tian-w.cn

[J09] 时区处理
来源：http://mot.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rbs.gotoacloud.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vbr.tanke756.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cjw.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fdp.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aif.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://byl.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cgb.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ldc.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://cvw.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://pna.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jxa.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iar.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tqg.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://and.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://slw.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://asa.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kjg.aizwys.cn

================================================================================
来源：http://qqb.zycfv.cn

K. JSON 与序列化
来源：http://kax.tarul.cn

================================================================================
来源：http://bmv.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://qfg.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dph.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://shu.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://vka.cashguo.top

TS:   JSON.stringify(obj)
来源：http://jlu.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rnk.yj20258888.top

Go:   json.Marshal(obj)
来源：http://pfr.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://tzk.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nxd.cucudq.cn

[K02] JSON 字符串转对象
来源：http://vim.9152youxi.cn

Py:   json.loads(s)
来源：http://cke.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ojc.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://qce.andypj.xyz

TS:   JSON.parse(s)
来源：http://asc.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kda.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://urz.smart0.xyz

Ruby: JSON.parse(s)
来源：http://dso.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lop.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://pxm.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zpf.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rdt.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://foc.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eoi.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jlc.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wzr.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://nhm.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ljk.guowangkeji.top

[K04] 读取 JSON 文件
来源：http://svf.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gsd.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kwp.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xnp.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wfd.0kj1m.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nht.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gny.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://xan.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cmv.yonumen.top

[K05] 深拷贝对象
来源：http://uzr.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://dgh.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://bep.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://lzu.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://idg.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yar.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bmk.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cpr.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://kek.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://zyc.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xmx.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bzw.vehdjk.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxt.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yob.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ebf.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qye.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wxc.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fzw.vehdjk.com

[K07] 进制转换
来源：http://tjv.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fyy.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tix.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vyh.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jia.kuanghao11.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zlj.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zlb.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cfn.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pmo.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://clw.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://qpr.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gfb.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://uii.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://rvd.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://umd.c1oappe.top

Go:   encoding/gob
来源：http://iil.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://cvx.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://woj.havefunace.top

================================================================================
来源：http://evx.guowangkeji.top

L. 网络请求
来源：http://nxl.gaohongyu789.top

================================================================================
来源：http://maf.havefunace.top

[L01] 发送 GET 请求
来源：http://thq.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yzk.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qzc.pycfn.com

JS:   await fetch(url)
来源：http://bnf.xuetiantiany.cn

TS:   await fetch(url)
来源：http://uxx.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dan.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://srm.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mxu.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qfu.iojbl.cn

[L02] 发送 POST JSON
来源：http://weo.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ywd.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jye.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yup.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dwk.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nzj.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ugf.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lzl.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ugq.aibaodan.cn

[L03] 设置自定义请求头
来源：http://toc.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rhb.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://crg.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ulv.uphjek.com


<!-- 参考信息 -->