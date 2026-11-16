代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://dxq.yj20258.top

C#:   e.Message;  e.StackTrace
来源：http://fge.zdbjq.cn

[H09] 带错误码的异常
来源：http://djy.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cst.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ymh.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mty.fanxiaobao.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pav.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kok.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pfd.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://eqc.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wte.cqqwz.cn

[H10] 资源自动释放
来源：http://hmx.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://znf.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mrk.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fhf.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ywy.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nnd.zdbjq.cn

Go:   defer f.Close()
来源：http://rjn.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mlb.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kcg.sxryk.cn

================================================================================
来源：http://fgc.yfazqb.com

I. 正则表达式
来源：http://rlp.aibaodan.cn

================================================================================
来源：http://nhz.shzxlz.cn

[I01] 判断是否匹配
来源：http://pou.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://frt.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://khd.jianghu66.top

JS:   /\d+/.test(s)
来源：http://lvq.yfazqb.com

TS:   /\d+/.test(s)
来源：http://pgm.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gje.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tpq.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://rig.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lfn.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://ybt.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://ule.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zdy.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gcl.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://mvd.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mfd.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://psa.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://ash.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ejc.redwolf501.top

[I03] 提取捕获分组
来源：http://btz.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xgq.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rqu.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://klf.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rkt.jlsjyb.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://spb.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jzl.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cvj.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pju.feifeiyinyue.top

[I04] 正则替换
来源：http://hcf.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kiy.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bep.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://rut.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://gwa.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://kyb.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yzz.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ugw.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jsy.quarkkingdee.top

[I05] 按正则拆分
来源：http://vnz.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dkr.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cvb.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://jyd.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://wjb.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://kcy.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jwx.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://mdb.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yrv.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gsu.andypj.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://agf.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lan.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yex.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xaj.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ape.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dts.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://prl.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dvu.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://xvb.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://whs.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eqx.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xxh.zhiwuduotai.top

TS:   /error/gim
来源：http://pid.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mmo.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vso.sweek.top

Ruby: s.scan(/error/i)
来源：http://nxa.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yll.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://skn.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ghn.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kko.yfazqb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://teo.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uxu.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zmq.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ikq.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tbm.daxiang520.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tsr.jinqigfzy.top

================================================================================
来源：http://xhz.yfazqb.com

J. 日期与时间
来源：http://dbl.sxryk.cn

================================================================================
来源：http://boe.yongpay.top

[J01] 获取当前时间
来源：http://bif.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ubn.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kqe.zhaomingkeji.xyz

JS:   new Date();  Date.now()
来源：http://trj.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://sed.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://usu.xingfuxueyuan.xyz

Go:   time.Now()
来源：http://gkn.shanyushiyangtech.top

Ruby: Time.now
来源：http://pna.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cst.shanyushiyangtech.top

[J02] 格式化输出
来源：http://iyo.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zvf.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kza.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hqm.xziqi.cn

TS:   d.toISOString()
来源：http://zpf.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ddr.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dso.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pve.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cov.yfazqb.com

[J03] 字符串解析为日期
来源：http://bni.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lkg.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cfj.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://ddc.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://kkq.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://jkb.cashguo.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jbx.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://tqx.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iea.jianghu66.top

[J04] 时间戳与日期互转
来源：http://uzr.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://evh.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lff.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sig.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uhp.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cpf.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tyi.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zlf.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mwl.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://ars.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://xks.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://fde.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uii.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wld.cashguo.top

Java: LocalDate.now().plusDays(7)
来源：http://biy.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://abr.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://rra.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://bcd.chenzaomai.com

[J06] 计算两时间之差
来源：http://ltk.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://sgv.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://pkt.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ypc.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aqe.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://gkc.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://str.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://esy.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://iou.jqgfzy.top

[J07] 比较两个日期
来源：http://cfc.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://pfn.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bng.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://xjz.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://xrw.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oib.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ogq.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tse.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://cdd.hnqzz.top

[J08] 提取年月日与星期
来源：http://uhj.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://avh.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jcu.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qvk.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://res.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kaj.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ygj.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ilg.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aqx.0kj1m.cn

[J09] 时区处理
来源：http://pzm.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xlr.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rbp.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mst.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eog.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jdh.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xcg.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ngm.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wfl.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://lhw.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wfa.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jzz.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ulh.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tvx.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zyu.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ufd.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ijr.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gyi.zhixingplan.top

================================================================================
来源：http://wph.ydjk.org.cn

K. JSON 与序列化
来源：http://zyg.bjfxy.top

================================================================================
来源：http://sth.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://pej.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sso.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mro.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://wsk.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://vhk.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ikk.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://jxp.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://kma.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://roo.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://giz.cucudq.cn

Py:   json.loads(s)
来源：http://lds.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iph.hcnkem.com

JS:   JSON.parse(s)
来源：http://jex.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://cti.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wmt.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://ztv.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://jei.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xnw.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://lvl.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qof.dianchejie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zgg.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jxs.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yrq.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nww.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qft.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://mpa.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xcq.sweek.top

[K04] 读取 JSON 文件
来源：http://wwq.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fen.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xsh.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iud.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zda.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eju.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hzt.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pcl.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ilt.yj20258888.top

[K05] 深拷贝对象
来源：http://jam.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://wmb.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://ipf.yueranfly.top

JS:   structuredClone(obj)
来源：http://zwv.jianghu66.top

TS:   structuredClone(obj)
来源：http://pqs.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nrq.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sri.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://imk.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hvd.hesvh.cn

[K06] 解析 URL 查询串
来源：http://gsc.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tkx.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ljl.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jhx.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qct.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nja.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mdc.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nbe.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yyj.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://nav.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vjo.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ave.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xds.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yex.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xps.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cwn.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://usr.hongshengwenyu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yex.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://ipn.yj202588.top

Py:   pickle.dumps(obj)
来源：http://wyq.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ftv.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://srz.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://dqz.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fzn.xziqi.cn

Go:   encoding/gob
来源：http://lik.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://ppw.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bqf.jqgufenzy.top

================================================================================
来源：http://wmm.cucudq.cn

L. 网络请求
来源：http://kgu.wangshuangyany.cn

================================================================================
来源：http://npx.jqgfzy.top

[L01] 发送 GET 请求
来源：http://knw.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vsc.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qvs.hesvh.cn

JS:   await fetch(url)
来源：http://vbq.xinyue.icu

TS:   await fetch(url)
来源：http://sfg.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cmq.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://mvp.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pmp.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dvh.hesvh.cn

[L02] 发送 POST JSON
来源：http://iil.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yjy.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wuo.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uge.ydjk.org.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cvv.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yhe.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zgp.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kyr.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xvb.fengsongda.top

[L03] 设置自定义请求头
来源：http://rxc.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ezf.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tif.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gcy.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://phm.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ukr.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rpu.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tar.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wig.cdnleiting.top

[L04] 设置超时
来源：http://jsj.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://fse.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://seh.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yfq.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qjm.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hmh.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eop.yfazqb.com


<!-- 参考信息 -->