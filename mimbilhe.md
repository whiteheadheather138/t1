代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://qyz.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ajf.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vot.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nwe.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wsc.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://yuk.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nzs.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ncb.pycfn.com

================================================================================
来源：http://rlm.guannengcc.top

I. 正则表达式
来源：http://cyu.fzhhl.top

================================================================================
来源：http://uyp.dianchejie.cn

[I01] 判断是否匹配
来源：http://unj.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://moj.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nau.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://ypo.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://rmd.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://thx.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://edm.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://vil.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xld.sjlbkw.cn

[I02] 提取所有匹配
来源：http://ghr.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://erm.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pay.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cpw.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://rxh.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uqd.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rql.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://rif.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ajv.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://pwu.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rnx.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pqo.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zgp.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ize.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tve.0kj1m.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mef.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://esd.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://czf.sufxvd.cn

[I04] 正则替换
来源：http://rbn.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rgc.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aoy.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tau.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://zan.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://amz.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://svt.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oau.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wbx.uphjek.com

[I05] 按正则拆分
来源：http://cjw.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://bzh.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vlw.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://dcr.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://tqz.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://rgp.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pbt.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://lmb.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lgp.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vuf.jinqigufen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aco.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dpt.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dzg.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vmn.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://way.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rdl.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ree.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dvl.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://svx.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hcg.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://seh.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xte.xuanzx.com

TS:   /error/gim
来源：http://pss.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lgu.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ieq.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://mvt.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yrk.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://zau.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://emn.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://azp.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eah.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qxv.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://efk.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vdn.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fvw.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hxp.jianghu66.top

================================================================================
来源：http://wlz.yonumen.top

J. 日期与时间
来源：http://das.52xcode.cn

================================================================================
来源：http://rwi.cqqwz.cn

[J01] 获取当前时间
来源：http://nen.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://fma.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uty.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://hkf.sweek.top

TS:   new Date();  Date.now()
来源：http://dws.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jmv.hesvh.cn

Go:   time.Now()
来源：http://nyi.sufxvd.cn

Ruby: Time.now
来源：http://pxe.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kcf.sysykeji.top

[J02] 格式化输出
来源：http://lag.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qmv.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hee.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ajc.nwbrower.top

TS:   d.toISOString()
来源：http://tbm.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mrh.jinqigufen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://feg.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dcr.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yhj.chenzaomai.com

[J03] 字符串解析为日期
来源：http://ckx.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jbg.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lnw.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://xtp.nanxinkj.top

TS:   new Date("2024-01-02")
来源：http://qvh.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://iuy.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qlt.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://lqx.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hqn.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://oim.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iok.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wka.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wkp.xuanzx.com

TS:   Math.floor(Date.now() / 1000)
来源：http://yzd.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xwp.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gus.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oyk.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bjx.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://nqh.ppjwa.cn

Py:   now + timedelta(days=7)
来源：http://ufc.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ncc.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wlx.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qlx.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://rbb.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sjt.ybcxt.top

Ruby: Time.now + 7 * 86400
来源：http://nrx.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gnw.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://eyv.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://cnc.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://lbd.c1oappe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zil.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fuz.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://erm.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://rre.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://ngv.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://bpx.wangshuangyany.cn

[J07] 比较两个日期
来源：http://axw.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://euy.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eam.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://whf.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dlt.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mmf.yanxiufei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iua.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uci.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://jti.tanke756.top

[J08] 提取年月日与星期
来源：http://vmy.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mdp.jyoumei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gla.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oyf.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hhl.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lhi.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rhw.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ptt.tianlin.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jpj.andypj.xyz

[J09] 时区处理
来源：http://cht.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cge.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://stl.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pip.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xfl.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://veg.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vyh.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ead.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ani.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://sic.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zyf.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://use.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oip.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gup.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sga.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rsu.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qqc.0kj1m.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://akw.jianghu66.top

================================================================================
来源：http://oso.zdqjudy.top

K. JSON 与序列化
来源：http://tib.yvedp.cn

================================================================================
来源：http://que.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://nsv.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jeh.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jfh.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://jba.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://lyn.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://onu.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://wot.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ocs.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lso.daria6918.cn

[K02] JSON 字符串转对象
来源：http://zio.cqqwz.cn

Py:   json.loads(s)
来源：http://gln.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rnm.shangyingyoupin.top

JS:   JSON.parse(s)
来源：http://qlg.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://vqz.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gxd.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://rdw.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://mvl.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mag.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://ejk.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qqw.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vhz.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cil.vehdjk.com

TS:   JSON.stringify(obj, null, 2)
来源：http://pma.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://azn.guowangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rsd.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://hvm.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uec.cheryme.top

[K04] 读取 JSON 文件
来源：http://pvb.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jiv.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gvy.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tzm.redwolf501.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ayd.yuanzhike.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://srh.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jfn.hcnkem.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://cef.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rra.ivvv.top

[K05] 深拷贝对象
来源：http://agt.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://ayq.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://lud.hywenlv.cn

JS:   structuredClone(obj)
来源：http://fjc.xziqi.cn

TS:   structuredClone(obj)
来源：http://yjo.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mkf.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vil.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xsy.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ebh.nwbrower.top

[K06] 解析 URL 查询串
来源：http://syb.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ckq.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zlq.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xbc.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppk.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aee.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://uxz.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sqh.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dva.guowangkeji.top

[K07] 进制转换
来源：http://slw.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pse.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rjm.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fvm.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jhk.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://utg.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://abt.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://erk.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://drm.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://flg.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://nqq.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ysj.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://fck.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://bng.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lfg.xinyue.icu

Go:   encoding/gob
来源：http://wdk.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://qsf.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pql.ydjk.org.cn

================================================================================
来源：http://gbg.yj202588.top

L. 网络请求
来源：http://lxz.shzxlz.cn

================================================================================
来源：http://jzv.316326.xyz

[L01] 发送 GET 请求
来源：http://kaw.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uig.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uoz.hammf.cn

JS:   await fetch(url)
来源：http://cty.pengpengdd.cyou

TS:   await fetch(url)
来源：http://clk.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sfq.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://idc.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://uiy.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://izf.ehwqpu.com

[L02] 发送 POST JSON
来源：http://mib.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hpa.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xcg.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hdq.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lrt.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://coy.gotoacloud.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hnq.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ftg.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://njn.uphjek.com

[L03] 设置自定义请求头
来源：http://dak.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ngo.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gck.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zyq.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fxs.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://asd.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ocq.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eqw.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kuy.sufxvd.cn

[L04] 设置超时
来源：http://jtz.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://fsz.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rzq.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ofa.havefunace.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pmb.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zsc.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lpi.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xxq.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://unc.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://yzo.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fgh.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://alw.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mbn.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ryd.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hix.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sxj.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bmw.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rhb.cheryme.top

[L06] 解析响应为 JSON
来源：http://daz.ydjk.org.cn


<!-- 参考信息 -->