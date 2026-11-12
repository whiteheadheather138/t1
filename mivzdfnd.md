代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://mul.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jpm.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dvo.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xxx.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nmy.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://skx.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://awd.daxiang520.top

[H10] 资源自动释放
来源：http://aow.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pli.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rgb.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ajb.tanke756.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pnx.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://usk.jqgfzy.top

Go:   defer f.Close()
来源：http://tau.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kub.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qba.ivvv.top

================================================================================
来源：http://ipj.svipenyu.cn

I. 正则表达式
来源：http://wxe.zhaomingkeji.xyz

================================================================================
来源：http://rpy.havefunace.top

[I01] 判断是否匹配
来源：http://roi.ywan-chungtsiang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eey.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://njy.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://xxy.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://ahl.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://clp.sweek.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fhg.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://hrm.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zvm.epnwcf.com

[I02] 提取所有匹配
来源：http://hrd.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://mpl.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jmh.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aqp.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://cht.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rsv.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://evf.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://iis.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nzu.xinyue.icu

[I03] 提取捕获分组
来源：http://ycn.zycfv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ytb.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://erf.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lqf.gotoacloud.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bzg.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://noa.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fei.birdmap.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vhm.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ris.zhiwuduotai.top

[I04] 正则替换
来源：http://jdu.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mfe.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rcg.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://tvj.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ivp.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://unx.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kvu.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wvz.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hzo.tanke756.top

[I05] 按正则拆分
来源：http://lkm.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wra.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://orw.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://wuf.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://vuw.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://gua.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pxc.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://kbi.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://raa.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://khp.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://apm.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bvx.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xsp.yj20258888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yok.jinqigufen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ekg.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lfy.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dgf.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rzf.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://loh.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blx.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aeo.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yyl.epnwcf.com

TS:   /error/gim
来源：http://eqn.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lfo.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://htz.316326.xyz

Ruby: s.scan(/error/i)
来源：http://isz.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cev.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://nji.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wkc.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xgp.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dfd.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lzu.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uuq.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rfd.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hrc.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bis.yvedp.cn

================================================================================
来源：http://twj.zhoulong.xyz

J. 日期与时间
来源：http://khn.nanxuanxn.top

================================================================================
来源：http://gwt.ydzc1.top

[J01] 获取当前时间
来源：http://cfn.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rns.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vqt.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://ttf.yfazqb.com

TS:   new Date();  Date.now()
来源：http://wlk.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qtl.feifeiyinyue.top

Go:   time.Now()
来源：http://ngh.yj20258888.top

Ruby: Time.now
来源：http://bzs.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oqv.meibo888.top

[J02] 格式化输出
来源：http://ult.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jsk.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vjk.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vfw.kuanghao11.cn

TS:   d.toISOString()
来源：http://hji.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fge.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mix.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://thm.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gpx.yuanzhike.top

[J03] 字符串解析为日期
来源：http://nmd.fzhhl.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gqk.zhaomingkeji.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rnq.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://tqn.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://aha.cucudq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mbz.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wyx.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://skg.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vkx.wangdashe.top

[J04] 时间戳与日期互转
来源：http://mkf.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vdy.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://otq.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kvf.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://yya.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://olp.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hgi.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jvo.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jqf.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://ttt.yj20258.top

Py:   now + timedelta(days=7)
来源：http://lze.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wmv.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wgi.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uxp.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://ltq.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lbs.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://ncz.shzxlz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jml.svipenyu.cn

[J06] 计算两时间之差
来源：http://kfl.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://asf.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://piy.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kwd.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yml.xingfuxueyuan.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ekb.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://yvv.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://mhk.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://kvm.epnwcf.com

[J07] 比较两个日期
来源：http://ysu.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://kfa.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fhw.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://whr.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://ohh.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vez.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iyx.mhx1999.top

Ruby: d1 < d2;  d1 == d2
来源：http://aeu.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://lpt.hfpthk.cn

[J08] 提取年月日与星期
来源：http://uxs.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mhl.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pmi.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://led.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://joi.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tcw.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ntv.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kmj.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cww.aizwys.cn

[J09] 时区处理
来源：http://abz.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://abj.ivvv.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zju.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xkk.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hpn.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tob.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://twv.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zal.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xai.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://kqo.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pum.hammf.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://azq.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qfr.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://emu.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ofe.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nza.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fub.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mjp.tian-w.cn

================================================================================
来源：http://phf.hysaishi.cn

K. JSON 与序列化
来源：http://tbo.zhaomingkeji.xyz

================================================================================
来源：http://nas.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://bkc.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://icl.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tqq.yj20258.top

JS:   JSON.stringify(obj)
来源：http://oti.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://cgq.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dpg.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://hfe.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://olk.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kri.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://vxe.hnqzz.top

Py:   json.loads(s)
来源：http://ncn.mhx1999.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pyo.yonumen.top

JS:   JSON.parse(s)
来源：http://xog.svipenyu.cn

TS:   JSON.parse(s)
来源：http://xsi.tarul.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://muf.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://mbo.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://apy.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mif.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://kzh.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://soh.xylfe.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yxo.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xfl.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bhv.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oxs.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lls.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://zdb.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hgo.ydzc1.top

[K04] 读取 JSON 文件
来源：http://jtw.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://txt.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bro.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wvs.shanyushiyangtech.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tci.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lwm.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zci.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aoa.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wfj.chenzaomai.com

[K05] 深拷贝对象
来源：http://zmq.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://wdy.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://szm.jinyuanbaomall.cn

JS:   structuredClone(obj)
来源：http://qpq.ydzc1.top

TS:   structuredClone(obj)
来源：http://nkh.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ylx.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oco.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wee.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yah.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://wrw.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gsv.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zie.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qnl.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dai.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ony.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://krs.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ngg.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://btl.wangdashe.top

[K07] 进制转换
来源：http://spz.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nea.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qsn.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xet.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rag.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cfg.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bzf.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ibb.hongshengwenyu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nmc.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://zsl.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://mnb.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://dva.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://ioi.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://nph.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aay.ivvv.top

Go:   encoding/gob
来源：http://cht.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://ezs.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jwi.xylfe.cn

================================================================================
来源：http://cou.jinqigufen.top

L. 网络请求
来源：http://brt.smart0.xyz

================================================================================
来源：http://gsx.yonumen.top

[L01] 发送 GET 请求
来源：http://ewz.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://guk.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xja.svipenyu.cn

JS:   await fetch(url)
来源：http://blw.kuanghao11.cn

TS:   await fetch(url)
来源：http://ovk.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hzi.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://aqk.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zwc.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gpl.daria6918.cn

[L02] 发送 POST JSON
来源：http://gtl.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://nqu.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oxn.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://chg.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sra.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jgd.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dyu.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fcx.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bop.xinyue.icu

[L03] 设置自定义请求头
来源：http://civ.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zyj.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zni.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fqh.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gmb.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kva.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kjo.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://faa.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tws.jinqigfzy.top

[L04] 设置超时
来源：http://hve.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://qwc.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lek.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://seo.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jlq.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tna.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pzw.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hwk.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hof.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://vax.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zyz.wangshuangyany.cn


<!-- 参考信息 -->