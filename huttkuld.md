代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eod.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://zzt.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yah.zycfv.cn

[H10] 资源自动释放
来源：http://mkj.zycfv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kdt.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ian.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bvd.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gar.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ccp.yuxming.cn

Go:   defer f.Close()
来源：http://woo.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dmw.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aaq.redwolf501.top

================================================================================
来源：http://swy.havefunace.top

I. 正则表达式
来源：http://ofv.nanxinkj.top

================================================================================
来源：http://vsl.sufxvd.cn

[I01] 判断是否匹配
来源：http://prz.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nng.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oei.meibo888.top

JS:   /\d+/.test(s)
来源：http://nzc.yuxming.cn

TS:   /\d+/.test(s)
来源：http://kld.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gow.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ffg.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://pma.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kui.daxiang520.top

[I02] 提取所有匹配
来源：http://aig.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://byx.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pxc.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ycs.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://fxq.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kgk.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qtv.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://lxg.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dcy.52xcode.cn

[I03] 提取捕获分组
来源：http://osm.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nqg.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ipp.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xnz.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://myk.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kpv.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ywv.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dfp.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xwf.birdmap.top

[I04] 正则替换
来源：http://pzx.jiagoushi.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nkr.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jzk.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://jft.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://fzo.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://bxg.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lik.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://aqz.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fna.0kj1m.cn

[I05] 按正则拆分
来源：http://tpg.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ffm.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ivi.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://oku.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://gvj.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://tab.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ydx.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dtr.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fta.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cqn.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://evh.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jlk.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ysb.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xly.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dpz.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hpa.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fed.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://izj.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://doa.yangfankeji.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xfl.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hxm.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mmy.tian-w.cn

TS:   /error/gim
来源：http://vgm.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lfv.uphjek.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dwp.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://lud.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tjc.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://gpr.snrcjt.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lle.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lbm.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gdb.hywenlv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ezq.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://iyn.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kcp.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fbi.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://keh.pycfn.com

================================================================================
来源：http://sku.guannengcc.top

J. 日期与时间
来源：http://con.jyoumei.cn

================================================================================
来源：http://ilv.hfpthk.cn

[J01] 获取当前时间
来源：http://bll.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tgz.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bvz.zhijiandao.cn

JS:   new Date();  Date.now()
来源：http://lda.hammf.cn

TS:   new Date();  Date.now()
来源：http://wza.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://shj.zhaomingkeji.xyz

Go:   time.Now()
来源：http://fxy.316326.xyz

Ruby: Time.now
来源：http://kvt.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://msq.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://naf.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sfm.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mhf.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gbv.pycfn.com

TS:   d.toISOString()
来源：http://gih.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fdc.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qgu.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lep.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yxl.hfpthk.cn

[J03] 字符串解析为日期
来源：http://mkk.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fxt.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nkc.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://hah.jiagoushi.top

TS:   new Date("2024-01-02")
来源：http://mrj.bjfxy.top

Java: LocalDate.parse("2024-01-02")
来源：http://kxe.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vhw.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://svd.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ymu.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://yxo.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://efe.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cva.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qht.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ppk.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wom.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vpe.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yep.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fyp.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://nbh.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://tad.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ija.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sbj.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tzu.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://osy.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dtm.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://bfr.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://fde.chenlongwang.top

[J06] 计算两时间之差
来源：http://jxh.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://qik.wangdashe.top

PHP:  $end->diff($start)->days;
来源：http://hzm.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dso.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uqc.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hix.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://buk.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://zzc.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://owd.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://tfk.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://qxn.jianghu66.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dzk.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://djy.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zyi.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://stm.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rov.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://tfs.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://inw.mhx1999.top

[J08] 提取年月日与星期
来源：http://itz.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wts.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://opj.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zrn.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fvj.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lwd.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rss.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://csy.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hvz.feifeiyinyue.top

[J09] 时区处理
来源：http://pcy.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hks.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pqb.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cvy.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rkp.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ipg.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jyj.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wfa.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ljy.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://hxd.epnwcf.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ypi.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://naz.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lek.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tnf.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rrj.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mbs.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://efg.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lag.ydjk.org.cn

================================================================================
来源：http://mzt.daxiang520.top

K. JSON 与序列化
来源：http://gpk.smart0.xyz

================================================================================
来源：http://hig.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://phq.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cco.cashguo.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zrj.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://lqd.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://ebu.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bgt.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://dwa.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pxr.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hpr.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://wjp.dashuyun.cn

Py:   json.loads(s)
来源：http://jnv.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://njp.nanxinkj.top

JS:   JSON.parse(s)
来源：http://uev.xinyue.icu

TS:   JSON.parse(s)
来源：http://uww.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gcm.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://jpi.yueranfly.top

Ruby: JSON.parse(s)
来源：http://lou.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wtf.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://kjv.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zcu.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://klm.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://njp.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ilg.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fmy.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://prf.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://cmx.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yta.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://ahy.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sai.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jfw.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ifn.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rot.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tnc.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rrs.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ngq.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sjb.yanxiufei.cn

[K05] 深拷贝对象
来源：http://emr.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://rzs.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://zrs.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://cnl.xziqi.cn

TS:   structuredClone(obj)
来源：http://csr.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ljv.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zpc.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://udb.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://htb.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://rxl.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sxs.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tll.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jmb.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yrb.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lxc.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yaw.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qib.zhengqikj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nmc.hfpthk.cn

[K07] 进制转换
来源：http://isq.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nwx.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://byg.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bck.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://smy.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oas.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zbl.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rzn.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lfx.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://pim.birdmap.top

Py:   pickle.dumps(obj)
来源：http://ide.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iqu.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://ckp.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://tbd.yj202588.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://unc.xziqi.cn

Go:   encoding/gob
来源：http://jsy.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://xay.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zzo.redwolf501.top

================================================================================
来源：http://vlv.gogol.net.cn

L. 网络请求
来源：http://gem.ydzc1.top

================================================================================
来源：http://xge.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://cuf.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://irj.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://inx.chenjidiqi.icu

JS:   await fetch(url)
来源：http://mfo.yueranfly.top

TS:   await fetch(url)
来源：http://ngj.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ndh.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://hqp.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wvq.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://acp.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://cnd.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://tiu.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mub.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vcf.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hoz.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zjx.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vth.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hax.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qmi.andypj.xyz

[L03] 设置自定义请求头
来源：http://gku.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xtn.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://afd.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hes.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pqb.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wzc.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://khb.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bim.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://beu.hcnkem.com

[L04] 设置超时
来源：http://btg.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://uge.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rme.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gwn.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ckr.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kzk.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kxa.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ryp.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kqh.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://agp.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qhp.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jox.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nkr.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vcs.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ogs.xinyue.icu


<!-- 参考信息 -->