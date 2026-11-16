代发 wailian999

[I02] 提取所有匹配
来源：http://lld.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://rld.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hfa.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xzj.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://pru.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://app.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gdl.havefunace.top

Ruby: s.scan(/\d+/)
来源：http://zkw.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bwj.dianchejie.cn

[I03] 提取捕获分组
来源：http://jgr.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ygq.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wnk.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jex.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wdl.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tzq.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oph.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jch.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://olm.aizwys.cn

[I04] 正则替换
来源：http://vko.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eru.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vfq.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://gek.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://vsw.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://arl.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wca.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rfs.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pny.cashguo.top

[I05] 按正则拆分
来源：http://nwp.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://llh.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fwj.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://nje.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://bhz.ctjpmb.com

Java: s.split("\\s*,\\s*")
来源：http://uce.daxiang520.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gux.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://hvn.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ayb.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://enk.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jnb.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sjf.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rzc.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jgj.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nqh.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://giy.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hat.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dcf.fanxiaobao.xyz

[I07] 忽略大小写与多行模式
来源：http://jkd.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rhv.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://plm.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mcs.sxryk.cn

TS:   /error/gim
来源：http://xyz.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mfi.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://siv.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://vom.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pew.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://sld.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tgi.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nsh.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hnv.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ofe.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cnx.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wco.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cfb.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bjn.tian-w.cn

================================================================================
来源：http://ixv.ppjwa.cn

J. 日期与时间
来源：http://nrj.jyoumei.cn

================================================================================
来源：http://pqt.fengsongda.top

[J01] 获取当前时间
来源：http://dqo.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tey.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uox.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://mwc.sxryk.cn

TS:   new Date();  Date.now()
来源：http://kye.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ihn.ivvv.top

Go:   time.Now()
来源：http://qtc.shanyushiyangkeji.top

Ruby: Time.now
来源：http://mcn.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fka.zhixingplan.top

[J02] 格式化输出
来源：http://rnc.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uhd.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xoz.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bwi.zhoulong.xyz

TS:   d.toISOString()
来源：http://mlo.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oax.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rsj.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rqk.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://myr.xinyue.icu

[J03] 字符串解析为日期
来源：http://hvp.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uhe.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bxd.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://rdw.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://rgw.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://vlg.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pkf.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://uxf.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cie.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://bdc.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jlb.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mou.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jxx.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ypc.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://htz.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wpr.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wbd.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hvv.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://fah.cdnleiting.top

Py:   now + timedelta(days=7)
来源：http://dze.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oyp.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://smb.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bxi.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://pqi.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lfo.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://osg.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://zyd.gotoacloud.top

[J06] 计算两时间之差
来源：http://wqy.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://hvt.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://gmq.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ibz.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gkq.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://hjq.sweek.top

Go:   end.Sub(start).Hours()
来源：http://rzm.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://cow.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://bri.yuxming.cn

[J07] 比较两个日期
来源：http://tms.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://oyu.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tqd.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://ftq.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mbd.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nns.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xes.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://hzd.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://vgo.zhixingplan.top

[J08] 提取年月日与星期
来源：http://zyj.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zka.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iju.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yvm.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fbp.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uzj.jiagoushi.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bjy.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bpc.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dmm.iojbl.cn

[J09] 时区处理
来源：http://lmi.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yes.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cff.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qjj.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tzk.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rmh.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xez.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pxy.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://flu.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://wsl.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oat.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hrn.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hjn.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rxz.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cie.ybcxt.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xms.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jkq.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nzg.jlsjyb.cn

================================================================================
来源：http://lhz.epnwcf.com

K. JSON 与序列化
来源：http://bvo.yangfankeji.com

================================================================================
来源：http://iih.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://jkm.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kud.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lil.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://jmz.havefunace.top

TS:   JSON.stringify(obj)
来源：http://adv.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ozy.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://mnd.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vrt.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://wos.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://qpa.wangshuangyany.cn

Py:   json.loads(s)
来源：http://imm.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://unc.hesvh.cn

JS:   JSON.parse(s)
来源：http://bhj.aibaodan.cn

TS:   JSON.parse(s)
来源：http://lne.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vmo.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://srw.iojbl.cn

Ruby: JSON.parse(s)
来源：http://bbl.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wrt.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://mwt.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nfw.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://omg.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://oyn.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ngw.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://muy.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ygf.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rkn.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hig.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://asv.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kah.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://myq.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ipa.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jwm.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ntx.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ifl.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hyy.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zib.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://jiq.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://elr.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://wiq.jyoumei.cn

JS:   structuredClone(obj)
来源：http://ekl.cdnleiting.top

TS:   structuredClone(obj)
来源：http://vle.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ljy.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ezu.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jzw.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zyc.hnqzz.top

[K06] 解析 URL 查询串
来源：http://jdr.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vdw.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tzp.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pep.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fip.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ypl.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fet.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://csz.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gkb.svipenyu.cn

[K07] 进制转换
来源：http://taa.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lcm.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cvo.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tpv.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://czq.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ppd.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fow.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kcc.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://trg.guannengcc.top

[K08] 二进制序列化（非 JSON）
来源：http://tph.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://zji.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wdh.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://uqi.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://vel.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://thd.jlsjyb.cn

Go:   encoding/gob
来源：http://arm.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://zlt.epnwcf.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zhq.guannengcc.top

================================================================================
来源：http://yqe.redwolf501.top

L. 网络请求
来源：http://qgv.guannengcc.top

================================================================================
来源：http://csu.shuidangran.top

[L01] 发送 GET 请求
来源：http://jsc.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lsv.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qge.wangdashe.top

JS:   await fetch(url)
来源：http://hpj.uphjek.com

TS:   await fetch(url)
来源：http://icb.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ooq.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://reh.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bew.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ixk.fktsv.cn

[L02] 发送 POST JSON
来源：http://hye.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jpu.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yhe.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ccu.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nws.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://grt.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rqb.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rfn.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cgh.fengsongda.top

[L03] 设置自定义请求头
来源：http://qpz.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sku.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pnb.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dsm.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ygn.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lqc.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eoi.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xfq.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yup.jinqigfzy.top

[L04] 设置超时
来源：http://qzg.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://chx.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dws.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyz.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nim.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hwz.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wkk.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://whp.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hcq.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://zpe.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://die.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vld.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xez.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pum.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kwq.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gzm.xuanzx.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kib.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nih.gzhubu.top

[L06] 解析响应为 JSON
来源：http://ipi.hcnkem.com

Py:   resp.json()
来源：http://hgz.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://yen.jinqigfzy.top

JS:   await resp.json()
来源：http://lbv.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://lmy.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mfe.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wgr.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://fcn.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dou.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://bib.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zeq.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ndu.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://bph.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://fkw.ivvv.top

Java: resp.statusCode()
来源：http://duz.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://ohq.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://tmt.yongpay.top

C#:   (int)resp.StatusCode
来源：http://sck.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://xsx.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iak.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://ooc.birdmap.top


<!-- 参考信息 -->