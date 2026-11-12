代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tex.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gln.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://fyr.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pvr.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://pzm.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://bhw.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rfp.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ver.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://qca.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tox.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tya.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://bwm.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zhb.fktsv.cn

[I03] 提取捕获分组
来源：http://mzr.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bkp.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dfv.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pmf.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yos.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ukn.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xee.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wsy.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://drk.pycfn.com

[I04] 正则替换
来源：http://wfo.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ctn.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pde.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://pcw.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ahj.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://bnw.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nkd.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tpz.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sci.sweek.top

[I05] 按正则拆分
来源：http://esd.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://num.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wwj.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://efh.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://gyi.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://kvu.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uyt.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://yas.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tia.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://etg.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hug.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://plj.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yar.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jmh.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jww.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wqa.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xqe.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mhp.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://ehn.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aow.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lka.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jbm.yj20258888.top

TS:   /error/gim
来源：http://dgz.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wdp.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lct.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://xst.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ims.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://cdi.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yyd.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yoo.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qzd.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yyp.gogol.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qej.fzhhl.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bkb.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vwk.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ljr.gaohongyu789.top

================================================================================
来源：http://jpt.fehbvm.com

J. 日期与时间
来源：http://lev.kuanghao11.cn

================================================================================
来源：http://npt.yueranfly.top

[J01] 获取当前时间
来源：http://kqz.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ewi.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hhu.xziqi.cn

JS:   new Date();  Date.now()
来源：http://sns.ivvv.top

TS:   new Date();  Date.now()
来源：http://kpi.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ugw.xylfe.cn

Go:   time.Now()
来源：http://jgn.aibaodan.cn

Ruby: Time.now
来源：http://pnt.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ejj.cqqwz.cn

[J02] 格式化输出
来源：http://ryt.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zqd.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tji.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nct.xylfe.cn

TS:   d.toISOString()
来源：http://nos.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wwo.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vwc.hesvh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://afn.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://syx.sxryk.cn

[J03] 字符串解析为日期
来源：http://zwt.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mix.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qin.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://peo.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://oca.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://xxr.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mvg.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://iom.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fpu.aizwys.cn

[J04] 时间戳与日期互转
来源：http://dxf.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hzd.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wqw.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mnk.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pky.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gzg.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kfc.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mym.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gkg.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://gmx.ivvv.top

Py:   now + timedelta(days=7)
来源：http://xiw.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bwm.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aek.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mll.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://yco.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://edu.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://den.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://qen.jqgufenzy.top

[J06] 计算两时间之差
来源：http://xfc.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://xev.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://shk.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ghd.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kqy.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://btt.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://xkg.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://jda.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://xxs.chenlongwang.top

[J07] 比较两个日期
来源：http://hlz.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://zmy.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qep.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vhe.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://whu.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://drx.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://krj.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://aof.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://qgf.yfazqb.com

[J08] 提取年月日与星期
来源：http://ehl.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xwn.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mgd.yanxiufei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://thr.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fio.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bum.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wzt.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://exx.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cpa.hammf.cn

[J09] 时区处理
来源：http://wuw.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dbk.zhiwuduotai.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mxv.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lvg.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://edl.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xoc.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dnx.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wke.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xlc.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://ype.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rbe.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pjp.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jbq.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aui.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eho.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://grd.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ano.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hey.shzxlz.cn

================================================================================
来源：http://wei.quarkkingdee.top

K. JSON 与序列化
来源：http://lyq.nanxuanxn.top

================================================================================
来源：http://msz.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://zvp.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jty.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kpj.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://msq.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://iby.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jzi.fzhhl.top

Go:   json.Marshal(obj)
来源：http://wuy.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://twg.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://dab.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://pei.sufxvd.cn

Py:   json.loads(s)
来源：http://nzj.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uem.ydzc1.top

JS:   JSON.parse(s)
来源：http://anc.epnwcf.com

TS:   JSON.parse(s)
来源：http://bml.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vkw.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://zew.yueranfly.top

Ruby: JSON.parse(s)
来源：http://tlh.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://weg.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://xaq.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://laz.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ono.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jwj.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fnz.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mgx.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zgl.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qad.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dix.daxiang520.top

[K04] 读取 JSON 文件
来源：http://pif.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bcj.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hay.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sjh.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ffr.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://txw.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rri.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jxv.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uas.sufxvd.cn

[K05] 深拷贝对象
来源：http://kef.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://war.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://efv.xinyue.icu

JS:   structuredClone(obj)
来源：http://meo.snrcjt.cn

TS:   structuredClone(obj)
来源：http://awg.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qww.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bcr.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pcn.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ype.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://gxl.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vjk.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ngr.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ccn.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fsv.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mug.ydzc1.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://asd.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wll.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qay.ctjpmb.com

[K07] 进制转换
来源：http://nyh.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mrz.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://clh.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iee.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fii.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ngo.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mxj.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dzi.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ubt.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://zxw.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://mwi.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bny.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://pfy.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://dmv.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vdf.hfpthk.cn

Go:   encoding/gob
来源：http://twd.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://awz.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dbb.jianghu66.top

================================================================================
来源：http://nsh.cucudq.cn

L. 网络请求
来源：http://dla.aibaodan.cn

================================================================================
来源：http://sam.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://dey.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mih.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aig.hesvh.cn

JS:   await fetch(url)
来源：http://ngr.hnqzz.top

TS:   await fetch(url)
来源：http://jdw.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://amo.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://uhj.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ufx.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mxp.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://sis.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://afq.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bzy.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gov.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://foj.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://awk.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aea.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tuy.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jmz.fzhhl.top

[L03] 设置自定义请求头
来源：http://amv.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wqq.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://phw.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pzd.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bbb.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rvh.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rav.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://row.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nha.zdbjq.cn

[L04] 设置超时
来源：http://ykj.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://bky.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ofq.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iwn.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://obv.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hib.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fda.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ktn.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tng.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://run.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vef.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tst.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ecu.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://knd.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://atm.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yni.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kgv.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hkq.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://ifd.cucudq.cn

Py:   resp.json()
来源：http://ptb.wangdashe.top

PHP:  json_decode($body, true);
来源：http://mmg.havefunace.top

JS:   await resp.json()
来源：http://rcp.tianlin.xyz

TS:   await resp.json()
来源：http://tfy.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://frm.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dmd.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://lad.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qzv.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://qrx.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uuq.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tkc.zdbjq.cn

JS:   resp.ok;  resp.status
来源：http://muh.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://pyn.vqdsnc.cn

Java: resp.statusCode()
来源：http://efa.gaohongyu789.top

Go:   resp.StatusCode
来源：http://mxo.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://hpy.sweek.top


<!-- 参考信息 -->