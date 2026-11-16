代发 wailian999

================================================================================
来源：http://lsm.smart0.xyz

I. 正则表达式
来源：http://sbp.bjfxy.top

================================================================================
来源：http://roz.yj20258.top

[I01] 判断是否匹配
来源：http://hta.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qhx.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cij.havefunace.top

JS:   /\d+/.test(s)
来源：http://zyj.xuanzx.com

TS:   /\d+/.test(s)
来源：http://vlc.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pwr.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rmy.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://yny.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pyx.zhijiandao.cn

[I02] 提取所有匹配
来源：http://llg.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://hfb.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tax.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qju.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://fcb.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tua.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vve.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://mgq.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hzc.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://cji.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xku.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yug.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ngc.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pqg.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://onx.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rol.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sxh.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gfc.yongpay.top

[I04] 正则替换
来源：http://aty.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qpg.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iqk.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://owo.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://mzj.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://osi.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://elr.ivvv.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tnw.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fvc.vehdjk.com

[I05] 按正则拆分
来源：http://sgy.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zab.zhixingplan.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ybt.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://oep.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://dtl.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://wyr.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pzx.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://rmd.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ngt.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ovc.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ihe.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://woq.0kj1m.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tel.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kpj.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jxe.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sas.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xlj.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pfm.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://cuq.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ukw.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xax.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://atu.hysaishi.cn

TS:   /error/gim
来源：http://zzq.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ydl.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qhe.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://dbt.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cvy.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://lbt.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eug.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://spq.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bos.sufxvd.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ycm.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://juh.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dtr.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kdt.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hnw.zdqjudy.top

================================================================================
来源：http://jgz.zhengqikj.top

J. 日期与时间
来源：http://jam.jinqigufen.top

================================================================================
来源：http://aek.hfpthk.cn

[J01] 获取当前时间
来源：http://pzx.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tdj.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gfn.fehbvm.com

JS:   new Date();  Date.now()
来源：http://gxq.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://cqu.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cmv.aizwys.cn

Go:   time.Now()
来源：http://vpq.c1oappe.top

Ruby: Time.now
来源：http://gjx.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vnq.sxryk.cn

[J02] 格式化输出
来源：http://ojh.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bib.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qqd.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tib.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://phb.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://chg.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bxy.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dud.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ezh.yj20258.top

[J03] 字符串解析为日期
来源：http://mph.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xhz.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rgf.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://yqq.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://fkq.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bdg.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wot.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://yio.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qig.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://jrk.yangfankeji.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tra.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wbf.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://acc.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://msm.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://alw.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://itx.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vfy.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wma.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://ttt.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://hhp.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tfk.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hmp.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zte.xingfuxueyuan.xyz

Java: LocalDate.now().plusDays(7)
来源：http://qmb.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xon.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://cni.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://fdi.gotoacloud.top

[J06] 计算两时间之差
来源：http://zdo.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://fer.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://mjg.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eph.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vzk.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://ylo.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://kzj.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://suh.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://bcb.zdbjq.cn

[J07] 比较两个日期
来源：http://emm.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://smv.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://quo.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qqa.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ymd.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ldu.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://scv.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://hnv.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://ick.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://lwf.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cjr.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ltm.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://emx.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mno.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sot.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gsg.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ffp.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sot.iojbl.cn

[J09] 时区处理
来源：http://pkk.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ade.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://adf.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ous.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vnr.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xpa.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ydn.hywenlv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://njd.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zhz.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://web.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rcz.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qam.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://loc.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://awk.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jtk.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rnt.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ywr.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jxg.shanyushiyangtech.top

================================================================================
来源：http://yil.ehwqpu.com

K. JSON 与序列化
来源：http://jqn.ivvv.top

================================================================================
来源：http://dsg.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://hjm.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bss.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hnd.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://rhv.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://apb.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ran.xinyue.icu

Go:   json.Marshal(obj)
来源：http://uzu.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://rvq.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ytb.birdmap.top

[K02] JSON 字符串转对象
来源：http://eqp.zhengqikj.top

Py:   json.loads(s)
来源：http://orw.ydzc1.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pca.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://rzx.zhixingplan.top

TS:   JSON.parse(s)
来源：http://bjq.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qfm.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://bnu.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://gwr.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cge.hywenlv.cn

[K03] JSON 美化输出（带缩进）
来源：http://xua.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zky.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lmv.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nsu.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qxg.0kj1m.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yme.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wzo.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://gdl.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hcf.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://ing.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rdf.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dxa.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvn.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bro.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://axq.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pfj.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qjt.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wba.nanxuanxn.top

[K05] 深拷贝对象
来源：http://nbq.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://riq.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://dif.redwolf501.top

JS:   structuredClone(obj)
来源：http://emf.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://twa.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ptm.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vso.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ekq.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vjj.yueranfly.top

[K06] 解析 URL 查询串
来源：http://opg.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fsn.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gyt.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://knu.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ggg.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zko.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://svi.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ryw.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://isd.hysaishi.cn

[K07] 进制转换
来源：http://dxc.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://znr.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://itk.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kin.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sct.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vzy.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yns.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qou.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blj.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://viz.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://drx.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qkr.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://cqa.sweek.top

TS:   v8.serialize(obj)        // Node
来源：http://xap.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ynm.hywenlv.cn

Go:   encoding/gob
来源：http://xxa.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://vml.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gmc.yuanzhike.top

================================================================================
来源：http://qit.hywenlv.cn

L. 网络请求
来源：http://wuh.sjlbkw.cn

================================================================================
来源：http://cls.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://wys.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dsy.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ajn.hysaishi.cn

JS:   await fetch(url)
来源：http://hzp.nwbrower.top

TS:   await fetch(url)
来源：http://kfo.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pfx.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://lqc.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://alf.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pzz.yvedp.cn

[L02] 发送 POST JSON
来源：http://gyp.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://loz.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dev.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osc.tianlin.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mjk.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://atz.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hmp.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bpj.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fuu.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://jxx.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fzq.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://imq.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jvm.jianghu66.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://coc.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qxn.yangfankeji.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nqu.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iph.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://syi.yonumen.top

[L04] 设置超时
来源：http://ggf.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://pah.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fbi.c1oappe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oun.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zqo.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://biy.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xjt.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dhf.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://grj.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://fje.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gmm.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gbp.fzhhl.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://isj.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ots.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dmy.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://caf.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vyu.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tjj.epnwcf.com

[L06] 解析响应为 JSON
来源：http://agj.fengsongda.top

Py:   resp.json()
来源：http://kun.havefunace.top

PHP:  json_decode($body, true);
来源：http://jvz.smart0.xyz

JS:   await resp.json()
来源：http://ied.ydzc1.top

TS:   await resp.json()
来源：http://uzo.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://znv.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xih.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://cjr.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pzm.xinyue.icu


<!-- 参考信息 -->