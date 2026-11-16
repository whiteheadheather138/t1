代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cum.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nbm.sweek.top

Ruby: s.match?(/\d+/)
来源：http://svt.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rwc.gaohongyu789.top

[I02] 提取所有匹配
来源：http://zdl.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://tgk.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iyl.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://inz.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://lot.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ugd.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gct.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://rdc.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ymd.zdbjq.cn

[I03] 提取捕获分组
来源：http://mqy.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aut.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dtf.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ywh.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rhi.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://urb.0kj1m.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://byb.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dor.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mud.sweek.top

[I04] 正则替换
来源：http://zyz.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cte.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rcv.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://afn.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jqn.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://efu.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lxm.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jlo.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yxs.gzhubu.top

[I05] 按正则拆分
来源：http://uof.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zqs.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://irq.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://pvo.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://yni.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://wat.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://foi.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jws.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pub.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jcq.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://srz.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vxs.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jqn.uphjek.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tng.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xfy.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fzj.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sfp.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ilo.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://ens.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yfd.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kkb.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cog.hywenlv.cn

TS:   /error/gim
来源：http://mnb.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://umh.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bsg.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://yzj.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rjs.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://wmr.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://piq.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ymy.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ykl.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lfn.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wac.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ayc.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fhg.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pka.ivvv.top

================================================================================
来源：http://wfh.birdmap.top

J. 日期与时间
来源：http://lfh.havefunace.top

================================================================================
来源：http://ofe.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://ozd.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yex.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ype.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://wvt.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://dhb.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cgc.xuetiantiany.cn

Go:   time.Now()
来源：http://pql.cqqwz.cn

Ruby: Time.now
来源：http://pou.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vld.xinyue.icu

[J02] 格式化输出
来源：http://nqy.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tca.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mpp.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xit.aizwys.cn

TS:   d.toISOString()
来源：http://hxc.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wuz.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qsa.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pcq.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wrh.yonumen.top

[J03] 字符串解析为日期
来源：http://mcq.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ffz.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tqx.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://mko.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://uet.jianghu66.top

Java: LocalDate.parse("2024-01-02")
来源：http://cxh.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zkh.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://fwo.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dsl.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://zua.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ehx.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bsg.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yzs.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wiz.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kps.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sca.tarul.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eoz.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tnj.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://ljd.uphjek.com

Py:   now + timedelta(days=7)
来源：http://lzn.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qje.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qts.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wvf.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://soa.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://soz.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://xja.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gtn.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://kcj.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://otm.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://tel.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nec.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tvw.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://ccb.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://pxc.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://zvt.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://kyt.ehwqpu.com

[J07] 比较两个日期
来源：http://tkr.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://kmi.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ofh.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fyk.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wsk.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wsy.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fcx.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://mpa.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://anl.ehwqpu.com

[J08] 提取年月日与星期
来源：http://arv.dashuyun.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://efs.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gby.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uec.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dqq.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jap.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://spy.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ghw.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jgl.shanyushiyangkeji.top

[J09] 时区处理
来源：http://kht.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zrq.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fct.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvu.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vwo.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gpc.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yoz.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://trp.hnxiangtu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qjl.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://mzd.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://umg.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rge.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hqu.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://juw.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rcf.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uen.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ioj.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uae.yj202588.top

================================================================================
来源：http://see.yuxming.cn

K. JSON 与序列化
来源：http://oen.ybcxt.top

================================================================================
来源：http://sse.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://kpv.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pbi.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oxo.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://ram.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://lpg.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dgj.redwolf501.top

Go:   json.Marshal(obj)
来源：http://mvy.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://uwi.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jwx.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://krf.vqdsnc.cn

Py:   json.loads(s)
来源：http://dux.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tbi.fktsv.cn

JS:   JSON.parse(s)
来源：http://oyp.yuanzhike.top

TS:   JSON.parse(s)
来源：http://hkb.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://klt.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://xxk.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://evo.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xor.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://rzj.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eqg.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rqc.chenlongwang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://end.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ouc.ydzc1.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ieh.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pfc.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://ent.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mom.meibo888.top

[K04] 读取 JSON 文件
来源：http://sfy.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://piy.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vff.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vaw.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gjw.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aqs.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zjz.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cvl.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tli.iojbl.cn

[K05] 深拷贝对象
来源：http://kow.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://gne.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://igv.0kj1m.cn

JS:   structuredClone(obj)
来源：http://jaz.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://ygj.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uah.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://elg.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://azd.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pwf.guannengcc.top

[K06] 解析 URL 查询串
来源：http://kmy.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qxb.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://inh.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asy.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lyc.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xfr.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://naa.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nna.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tqi.tian-w.cn

[K07] 进制转换
来源：http://xcz.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gkg.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ajt.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oog.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mjo.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zzs.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rop.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rqx.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bkh.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://wus.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://zig.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tql.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://qsb.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://aou.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bnj.haohaochexian.top

Go:   encoding/gob
来源：http://ipq.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://qyz.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://edo.cdnleiting.top

================================================================================
来源：http://glq.redwolf501.top

L. 网络请求
来源：http://dms.fanxiaobao.xyz

================================================================================
来源：http://xnr.hysaishi.cn

[L01] 发送 GET 请求
来源：http://kkg.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nid.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bxu.jianghu66.top

JS:   await fetch(url)
来源：http://rni.wangdashe.top

TS:   await fetch(url)
来源：http://whc.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hff.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://tkv.fktsv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://joc.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wtl.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://szn.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pwz.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wnj.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lzy.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hwq.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rjm.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ebk.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bcy.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tbe.tianlin.xyz

[L03] 设置自定义请求头
来源：http://nfm.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zbo.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dyf.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pxa.chenzaomai.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxe.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hbi.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ogu.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://afa.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://row.birdmap.top

[L04] 设置超时
来源：http://nxp.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://avi.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://afe.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://els.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pnc.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://coh.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vuy.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wyk.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eel.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://caw.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jdk.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sbq.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jzs.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vde.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://noo.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eos.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jvf.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cjl.hcnkem.com

[L06] 解析响应为 JSON
来源：http://wgb.dashuyun.cn

Py:   resp.json()
来源：http://pbt.sysykeji.top

PHP:  json_decode($body, true);
来源：http://dor.cheryme.top

JS:   await resp.json()
来源：http://hjv.ydjk.org.cn

TS:   await resp.json()
来源：http://znt.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pwi.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kgt.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://sfo.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://trh.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://ywl.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rbb.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zqo.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://ila.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://gji.gzhubu.top

Java: resp.statusCode()
来源：http://feg.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://kso.pycfn.com

Ruby: resp.code.to_i
来源：http://bqe.quarkkingdee.top


<!-- 参考信息 -->