代发 wailian999

JS:   e.message;  e.stack
来源：http://fhp.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wdw.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fkb.ivvv.top

Go:   err.Error()
来源：http://bui.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://yfh.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://qdg.ybcxt.top

[H09] 带错误码的异常
来源：http://mxl.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mmd.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ygd.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ouy.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://upr.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://elt.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uwl.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://klc.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yao.cqqwz.cn

[H10] 资源自动释放
来源：http://ttt.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bse.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mja.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cfz.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rgs.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kny.yuxming.cn

Go:   defer f.Close()
来源：http://qhn.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ina.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wpg.sweek.top

================================================================================
来源：http://xhy.sjlbkw.cn

I. 正则表达式
来源：http://kmm.zdqjudy.top

================================================================================
来源：http://gma.fengsongda.top

[I01] 判断是否匹配
来源：http://lpf.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fsc.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://fvj.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://bur.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://rwk.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uta.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://asl.ivvv.top

Ruby: s.match?(/\d+/)
来源：http://mhy.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ndd.wangdashe.top

[I02] 提取所有匹配
来源：http://mft.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://mvm.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gjr.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zfd.shzxlz.cn

TS:   s.match(/\d+/g)
来源：http://pyw.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nhj.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mfh.sweek.top

Ruby: s.scan(/\d+/)
来源：http://wmn.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xay.smart0.xyz

[I03] 提取捕获分组
来源：http://wzg.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zsv.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ogg.jqgufenzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uoo.yuxming.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qvr.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://siq.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mns.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://trw.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hud.daria6918.cn

[I04] 正则替换
来源：http://lny.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nmz.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yba.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ewl.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oxf.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://riu.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://bra.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://crr.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jjs.tarul.cn

[I05] 按正则拆分
来源：http://dci.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sqh.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://djs.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://nmd.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://laz.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://hqz.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uiz.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ite.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sdz.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yyc.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wfu.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hqp.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eze.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ajl.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sjc.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mmf.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nhh.0kj1m.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pod.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://frr.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bwl.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rni.yj20258888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lxu.jinghuilouyu.cn

TS:   /error/gim
来源：http://ylc.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iug.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://twm.yj20258.top

Ruby: s.scan(/error/i)
来源：http://jfx.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gus.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://qtf.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hmx.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yqj.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://whn.shanyushiyangtech.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nse.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rmw.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eft.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kwb.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vaq.ydjk.org.cn

================================================================================
来源：http://sha.guowangkeji.top

J. 日期与时间
来源：http://bpb.hnqzz.top

================================================================================
来源：http://yys.chenzaomai.com

[J01] 获取当前时间
来源：http://hsg.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fcx.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bwq.aizwys.cn

JS:   new Date();  Date.now()
来源：http://pjt.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://eux.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://jrc.yfazqb.com

Go:   time.Now()
来源：http://dqt.jinghuilouyu.cn

Ruby: Time.now
来源：http://uzv.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pmh.smart0.xyz

[J02] 格式化输出
来源：http://ieg.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pzz.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://scw.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tvg.haohaochexian.top

TS:   d.toISOString()
来源：http://uki.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vdv.jyoumei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://luk.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://knb.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://opf.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://vnp.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qnr.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rrq.sweek.top

JS:   new Date("2024-01-02")
来源：http://oyn.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://lvn.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://vsl.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hft.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://bix.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qlr.shuidangran.top

[J04] 时间戳与日期互转
来源：http://pvo.aibaodan.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gpm.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lnt.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ztg.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xzf.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qvb.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tpg.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uwj.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lqv.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://eni.meibo888.top

Py:   now + timedelta(days=7)
来源：http://bwg.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://voa.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vwm.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bgj.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://zpi.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gsp.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://lca.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://kxg.jqgfzy.top

[J06] 计算两时间之差
来源：http://erf.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://grp.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://ann.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jqm.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xqh.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://ehl.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://tod.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://eyg.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://dgn.yj20258888.top

[J07] 比较两个日期
来源：http://imp.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://uqn.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zxq.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lwd.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://ntw.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ioi.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pgn.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cye.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://bvq.epnwcf.com

[J08] 提取年月日与星期
来源：http://iod.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ixt.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ttq.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xbk.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://akv.c1oappe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sll.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://znr.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kez.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fvg.zhongyouzk.top

[J09] 时区处理
来源：http://ckc.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yup.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pnm.cucudq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://btk.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kzl.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lif.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lma.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://axz.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pgi.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://kgd.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ird.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rli.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ujx.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lnu.52xcode.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ocg.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qak.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lpy.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rzn.shangyingyoupin.top

================================================================================
来源：http://tip.yangfankeji.com

K. JSON 与序列化
来源：http://dum.daria6918.cn

================================================================================
来源：http://qyu.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://qyf.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hfa.yj20258888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cps.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://tzq.zycfv.cn

TS:   JSON.stringify(obj)
来源：http://ong.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ryb.xziqi.cn

Go:   json.Marshal(obj)
来源：http://gfb.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ktr.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xgd.bbcook.cn

[K02] JSON 字符串转对象
来源：http://nds.andypj.xyz

Py:   json.loads(s)
来源：http://nme.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tht.c1oappe.top

JS:   JSON.parse(s)
来源：http://sbd.yfazqb.com

TS:   JSON.parse(s)
来源：http://wjr.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yts.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://nea.hnqzz.top

Ruby: JSON.parse(s)
来源：http://jui.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jek.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://nvc.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://boy.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cqb.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ted.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://spx.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zqg.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ima.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://mvh.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dxm.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://ysm.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tgs.meibo888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qpu.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sfz.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tfj.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ydz.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wbw.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://cep.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zht.andypj.xyz

[K05] 深拷贝对象
来源：http://gdw.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://ymr.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://eeo.gotoacloud.top

JS:   structuredClone(obj)
来源：http://fhn.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://adq.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://ege.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ext.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://awm.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://sdf.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://ito.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lop.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://puo.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iwh.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bld.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wqo.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hhg.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cnz.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zuy.dianchejie.cn

[K07] 进制转换
来源：http://aib.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ztd.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zdt.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cbq.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ims.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xbk.yuxming.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cmk.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fip.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eaa.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://zsg.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://sww.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ruk.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://icw.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://dim.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ywi.jiagoushi.top

Go:   encoding/gob
来源：http://nut.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://ddq.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kkf.yueranfly.top

================================================================================
来源：http://twq.ydzc1.top

L. 网络请求
来源：http://riv.yanxiufei.cn

================================================================================
来源：http://xiz.yueranfly.top

[L01] 发送 GET 请求
来源：http://ezl.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zqn.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cgy.ybcxt.top

JS:   await fetch(url)
来源：http://gln.sysykeji.top

TS:   await fetch(url)
来源：http://dmi.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mqs.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://rev.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nlj.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yil.zhijiandao.cn

[L02] 发送 POST JSON
来源：http://rio.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://fgi.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hid.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dyi.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mht.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://brx.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gia.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cpi.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wrb.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://ero.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kyq.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vbi.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rru.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oje.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dkl.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://osh.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rji.chenjidiqi.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cxe.tarul.cn

[L04] 设置超时
来源：http://ryg.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://typ.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jvt.ehwqpu.com


<!-- 参考信息 -->