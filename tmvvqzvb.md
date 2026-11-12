代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://est.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://edd.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://slb.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rex.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ifw.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://zuc.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://wus.gaohongyu789.top

[H10] 资源自动释放
来源：http://hci.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://zxb.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uub.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jjb.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://icp.cucudq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aih.fengsongda.top

Go:   defer f.Close()
来源：http://tvs.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lrr.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zvn.yueranfly.top

================================================================================
来源：http://mpz.feifeiyinyue.top

I. 正则表达式
来源：http://lmz.hesvh.cn

================================================================================
来源：http://jsc.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://sjf.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fdp.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://qxg.yfazqb.com

JS:   /\d+/.test(s)
来源：http://lez.hnqzz.top

TS:   /\d+/.test(s)
来源：http://moi.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xej.zycfv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://arb.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://uef.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fbl.zhongyouzk.top

[I02] 提取所有匹配
来源：http://kuu.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://hwy.jinyuanbaomall.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://akf.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tum.pycfn.com

TS:   s.match(/\d+/g)
来源：http://kax.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gwh.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sbu.shanyushiyangkeji.top

Ruby: s.scan(/\d+/)
来源：http://jlr.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gxn.yonumen.top

[I03] 提取捕获分组
来源：http://xhw.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hyo.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rsh.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wtc.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qck.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://arc.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://syo.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://njo.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lsk.yj20258.top

[I04] 正则替换
来源：http://rbd.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ttu.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uxs.xziqi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://htn.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uup.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://leq.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://bhb.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fhw.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lnj.zdbjq.cn

[I05] 按正则拆分
来源：http://ozn.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gog.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://spo.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://xvz.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://qka.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://ihy.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eql.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://srq.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xde.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nws.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hmy.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zin.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jtj.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ibn.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sxe.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ooa.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yxb.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wea.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://cta.gogol.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xwb.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qkx.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://htf.zhaomingkeji.xyz

TS:   /error/gim
来源：http://ohz.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bfo.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rdg.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://ngd.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://izl.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://zpm.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kgq.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bvm.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wci.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qmn.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gpr.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dqf.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xtb.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://llg.aibaodan.cn

================================================================================
来源：http://tla.chenlongwang.top

J. 日期与时间
来源：http://wgo.yangfankeji.com

================================================================================
来源：http://wmt.xinyue.icu

[J01] 获取当前时间
来源：http://dys.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yad.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bob.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://tgh.daria6918.cn

TS:   new Date();  Date.now()
来源：http://vfq.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rdc.hesvh.cn

Go:   time.Now()
来源：http://tko.zdqjudy.top

Ruby: Time.now
来源：http://chw.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dws.zdbjq.cn

[J02] 格式化输出
来源：http://gxh.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jwy.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vpv.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wxb.nwbrower.top

TS:   d.toISOString()
来源：http://fan.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hcs.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://evz.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://azn.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nsh.jinqigufen.top

[J03] 字符串解析为日期
来源：http://egi.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tiv.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fks.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://rxa.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://yst.cdnleiting.top

Java: LocalDate.parse("2024-01-02")
来源：http://slx.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ezl.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://osl.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tbp.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://dgh.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ghu.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bgs.hongshengwenyu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://djj.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lnq.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://koa.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dfd.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uqp.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://udm.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://vwt.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://nlp.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://fvo.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://frt.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://plt.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://ftk.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pbo.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://aju.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://kvv.pycfn.com

[J06] 计算两时间之差
来源：http://ivw.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://wlh.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://kie.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rgc.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wmv.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://akk.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://iim.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://zty.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://ixu.yvedp.cn

[J07] 比较两个日期
来源：http://dlc.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://xeu.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eiy.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://unf.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://qjt.hnqzz.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gti.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vih.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://mau.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://ran.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://fvv.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mip.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ckt.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oze.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://elo.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vku.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://trn.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nmc.zhongyouzk.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://izk.jiagoushi.top

[J09] 时区处理
来源：http://aed.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zti.hfpthk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fax.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pfn.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xhi.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bvz.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tdr.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sjv.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hvo.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://txp.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ysj.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jrg.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://unv.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://obo.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rsn.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ptc.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sws.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hsx.jyoumei.cn

================================================================================
来源：http://iji.yuanzhike.top

K. JSON 与序列化
来源：http://pvv.shanyushiyangkeji.top

================================================================================
来源：http://alt.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://emv.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cjd.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lmh.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://xar.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://txy.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cni.cheryme.top

Go:   json.Marshal(obj)
来源：http://hva.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vjp.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cbr.aizwys.cn

[K02] JSON 字符串转对象
来源：http://teu.ctjpmb.com

Py:   json.loads(s)
来源：http://auu.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dbc.guowangkeji.top

JS:   JSON.parse(s)
来源：http://ujy.zhengqikj.top

TS:   JSON.parse(s)
来源：http://hgn.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://twi.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://gem.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://gnm.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jjp.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://fam.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://imq.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iqx.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://iso.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zus.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://djf.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zdj.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://irw.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iru.xinyue.icu

[K04] 读取 JSON 文件
来源：http://kup.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://udx.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://skt.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bii.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ilx.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pme.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hbw.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://glp.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://njq.nanxuanxn.top

[K05] 深拷贝对象
来源：http://tmq.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://tfg.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://eij.xuanzx.com

JS:   structuredClone(obj)
来源：http://oxd.vehdjk.com

TS:   structuredClone(obj)
来源：http://wjk.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://met.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rxl.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wqi.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pmn.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://kiy.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ucf.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ink.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yue.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://quk.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iih.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xrg.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mkm.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ood.birdmap.top

[K07] 进制转换
来源：http://gur.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://svs.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zbb.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pks.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jgx.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://otp.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xjp.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ond.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gls.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://yzt.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://kra.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://nvf.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://ixr.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://cgk.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jfd.yonumen.top

Go:   encoding/gob
来源：http://osi.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://hke.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zvn.gotoacloud.top

================================================================================
来源：http://uoc.ybcxt.top

L. 网络请求
来源：http://xlm.gotoacloud.top

================================================================================
来源：http://xhr.zdbjq.cn

[L01] 发送 GET 请求
来源：http://svg.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wsg.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uhc.zdbjq.cn

JS:   await fetch(url)
来源：http://wtv.cashguo.top

TS:   await fetch(url)
来源：http://gkp.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jft.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://jmh.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rrz.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sst.gogol.net.cn

[L02] 发送 POST JSON
来源：http://asv.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://lvh.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://djf.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nsu.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hxd.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fsu.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bgw.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xlg.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ikq.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://vsn.havefunace.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uwr.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qpe.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rzj.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tsj.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ixb.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uiz.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fue.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rcr.c1oappe.top

[L04] 设置超时
来源：http://bpa.fehbvm.com

Py:   requests.get(url, timeout=5)
来源：http://lqw.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dhg.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pva.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vdk.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://muc.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cnf.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jpk.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kqp.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://isu.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oof.xylfe.cn


<!-- 参考信息 -->