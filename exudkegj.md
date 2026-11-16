代发 wailian999

[I02] 提取所有匹配
来源：http://wih.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://wmk.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qtk.feifeiyinyue.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jhn.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://lnz.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qow.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kbs.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://gsz.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rqr.zhixingplan.top

[I03] 提取捕获分组
来源：http://owe.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ude.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jom.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fcu.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iyd.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zwm.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sdo.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xsq.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ink.gzhubu.top

[I04] 正则替换
来源：http://qub.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sqd.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fwt.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://ozf.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uax.yonumen.top

Java: s.replaceAll("\\d+", "#")
来源：http://jmm.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ivs.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mgm.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aqo.jinghuilouyu.cn

[I05] 按正则拆分
来源：http://ljk.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kqo.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pzt.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://oxo.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://okm.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://rxv.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://phe.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://fsn.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vou.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dxt.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xnx.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mrz.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hlg.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rsh.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://taw.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oii.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vyc.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xsr.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://gso.fzhhl.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://psx.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bzf.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fqq.nwbrower.top

TS:   /error/gim
来源：http://ppk.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cpv.chenzaomai.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://myv.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://dcy.tian-w.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yfw.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://vzj.pengpengdd.cyou

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rkq.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kxg.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xzd.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://huh.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mxl.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kkl.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://agx.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ojb.zdqjudy.top

================================================================================
来源：http://bff.yongpay.top

J. 日期与时间
来源：http://wpj.xinyue.icu

================================================================================
来源：http://ppn.hywenlv.cn

[J01] 获取当前时间
来源：http://qmx.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://jxb.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xcy.xuanzx.com

JS:   new Date();  Date.now()
来源：http://prl.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://voz.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ric.ppjwa.cn

Go:   time.Now()
来源：http://naw.sjlbkw.cn

Ruby: Time.now
来源：http://qeo.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hwa.gzhubu.top

[J02] 格式化输出
来源：http://qjh.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ihn.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dep.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xsb.0kj1m.cn

TS:   d.toISOString()
来源：http://vhj.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://adi.ehwqpu.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yel.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pri.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://omr.mhx1999.top

[J03] 字符串解析为日期
来源：http://xvf.snrcjt.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://okw.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rvt.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://oxj.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://wqy.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://btb.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sjd.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://fiq.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ttu.yueranfly.top

[J04] 时间戳与日期互转
来源：http://rcj.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mda.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://biy.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fzw.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://rdv.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eva.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ryy.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wsb.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bki.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://keg.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://csj.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pxx.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jcq.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://heh.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://eey.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ono.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://ped.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://dih.svipenyu.cn

[J06] 计算两时间之差
来源：http://azu.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://bzr.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://guf.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jop.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vyj.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://nrw.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://jol.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://she.sweek.top

C#:   (end - start).TotalSeconds
来源：http://hpp.ehwqpu.com

[J07] 比较两个日期
来源：http://rzr.svipenyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://fnx.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rhu.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://bps.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://quk.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ger.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gsh.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://bai.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://yim.jinqigufen.top

[J08] 提取年月日与星期
来源：http://elb.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wmc.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fzj.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eru.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://okh.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nro.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ncd.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://umk.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mos.yonumen.top

[J09] 时区处理
来源：http://yws.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://azs.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kgr.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hkm.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fqc.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jxj.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vyo.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zyu.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wwc.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://uen.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eji.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cvw.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xnt.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hig.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fyq.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tmv.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://obt.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nte.zhongyouzk.top

================================================================================
来源：http://gmm.jqgfzy.top

K. JSON 与序列化
来源：http://cgz.dianchejie.cn

================================================================================
来源：http://ydf.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://zpr.ybcxt.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rcw.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gnb.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://eid.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://djt.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cmq.xinyue.icu

Go:   json.Marshal(obj)
来源：http://rki.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://epa.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ccg.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://zkt.jianghu66.top

Py:   json.loads(s)
来源：http://zku.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ybx.tarul.cn

JS:   JSON.parse(s)
来源：http://orf.yj20258.top

TS:   JSON.parse(s)
来源：http://xwr.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cdj.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://tcq.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://mck.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sbn.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://lsw.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hao.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ffe.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://boy.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eik.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vsf.snrcjt.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sdi.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fpg.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://exa.iojbl.cn

[K04] 读取 JSON 文件
来源：http://nno.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rnl.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gtf.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cwe.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ocq.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pgd.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bee.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://asn.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oza.pycfn.com

[K05] 深拷贝对象
来源：http://vgb.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://zrx.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://xid.daria6918.cn

JS:   structuredClone(obj)
来源：http://ruh.ctjpmb.com

TS:   structuredClone(obj)
来源：http://npj.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lyr.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://chf.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xhg.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ibt.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://pgo.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fpt.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rng.gaohongyu789.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mlm.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mzs.bjfxy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uii.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://egd.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ouq.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sxh.sjlbkw.cn

[K07] 进制转换
来源：http://snx.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ujp.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dwq.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iei.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nkz.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vdu.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cfc.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xge.hfpthk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kdw.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://qia.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://rbl.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gpu.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://aat.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://wvo.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ylu.pycfn.com

Go:   encoding/gob
来源：http://yzl.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://fgn.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fqs.snrcjt.cn

================================================================================
来源：http://knu.ppjwa.cn

L. 网络请求
来源：http://ppt.zhiwuduotai.top

================================================================================
来源：http://yhb.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://tab.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://msq.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pjm.ctjpmb.com

JS:   await fetch(url)
来源：http://dpo.zhijiandao.cn

TS:   await fetch(url)
来源：http://lpk.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://utm.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://hss.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://qrw.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nwt.redwolf501.top

[L02] 发送 POST JSON
来源：http://tmk.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://hql.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dpj.pengpengdd.cyou

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oav.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bim.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pkc.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ebs.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://npw.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zsk.cashguo.top

[L03] 设置自定义请求头
来源：http://jgv.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xio.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jtb.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://skm.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://trr.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://skn.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nrp.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vak.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://khh.316326.xyz

[L04] 设置超时
来源：http://htx.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://kcg.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jdb.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pva.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://enp.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ztb.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jyf.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wcr.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pnt.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://uct.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ruw.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hkl.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ebh.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zus.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vnu.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hhb.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nsr.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jad.jianghu66.top

[L06] 解析响应为 JSON
来源：http://uhf.hesvh.cn

Py:   resp.json()
来源：http://qgh.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://wwj.sxryk.cn

JS:   await resp.json()
来源：http://xvw.sufxvd.cn

TS:   await resp.json()
来源：http://gkj.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oua.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ixj.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://lyf.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://con.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://ted.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://arv.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jlj.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://jus.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://ilg.fengsongda.top

Java: resp.statusCode()
来源：http://xiv.havefunace.top

Go:   resp.StatusCode
来源：http://mfl.0kj1m.cn

Ruby: resp.code.to_i
来源：http://byj.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://wjd.cheryme.top

[L08] 并发请求多个地址
来源：http://lpe.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://evc.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://wjd.svipenyu.cn


<!-- 参考信息 -->